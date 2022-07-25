# UAssetAPI

***Please note that this may be quite complicated for those new to C# or programming in general as this is object oriented programming***

- [UassetAPI](https://github.com/atenfyr/UAssetAPI) is a C# API made by [atenfyr](https://github.com/atenfyr) that allows extensive editing of unreal engine 4 assets
- The main advantage of this API over UAssetGUI is that with a little C# experience, very impressive edits can be made to .umaps and .uassets very quickly
- This will be mostly done through iteration

- First download the [UassetAPI source code](https://github.com/atenfyr/UAssetAPI) using github desktop or as a .zip file
- Then open the .sln in visual studio(Make sure dotnet 4.7.2 SDK and compiler are installed for visual studio) and build UassetAPI
- This will generate some .dlls in UassetAPI's debug folder which we can reference in our visual studio project
- Set up a visual studio project from a template (for applications I use a winforms template and for general .uasset editing I use the command line interface)
- This will generate a simple template in dotnet 4.7.2 that can be used with UassetAPI (if you want to add source control I recommend the github extension by github and then you can add source control from the file dropdown)
- reference the generated .dlls from the project dropdown and you're ready to start
- The basic setup you'll want to start in the namespace with will be something like
```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using UAssetAPI;

namespace WhateverYouCalledYourProject
{
    class Program
   {
      static void Main(string[] args)
      {
        static public void RandTransform(string filepath, string endpath)//I make this a function so it's callable for multiple uassets
        {
            Uasset y=new Uasset(filepath,UE4Version./*Put the corresponding version-intellisense will give you some suggestions*/)
            MessageBox.Show($"Data preserved:{(y.VerifyBinaryEquality() ? "yes" : "no")}");
            //checks if data has been parsed properly. If it has not then report it to atenfyr using his issue templates here:
            //https://github.com/atenfyr/UAssetAPI/issues/new?assignees=&labels=&template=bug_report.md&title=
            //for loop loops through exports(alternatively use a foreach loop)
            for (int i = 0; i < y.Exports.Count; i++)
            {
                Export export=y.Exports[i];
                if (export is NormalExport ex)
                {
                    //loop through subcategories to find whatever you're looking for
                    for (int j = 0; j < ex.Data.Count; j++)
                    {
                        //do whatever you want to the subcategories
                    }
                }
            }
            y.Write(endpath); //remember to do this otherwise your edits will not be saved
        }
      }
   }
}
```
You can do checks for certain exports using if statements

e.g ```if(ex.Data[j].Name.Equals(FName.FromString("Item")) && ex.Data[j] is BytePropertyData byt){}```

And then do things to the the export byt in this example like

```byt.Value = y.AddNameReference(FString.FromString(Items[19]));```

Using this method you can loop through multiple files very quickly to make edits that would have taken ages to do manually with UassetGUI

Below I will include some code snippets for editing common PropertyData types:
### Enums
```csharp
    static public void Enums(string filepath, string endpath, int indexes)//I state the number of indexes because sometimes eh.Count causes an index out of range error
    {
        //Load enum
        UAsset y = new UAsset(filepath, UE4Version.VER_UE4_25);
        //Only one export so for loop isn't needed
        Export baseUs = y.Exports[0];
        if (baseUs is EnumExport us)
        {
            List<Tuple<FName, long>> eh = us.Enum.Names;
            for (int j = 0; j < indexes; j++)
            {
                eh[j] = new Tuple<FName, long>(us.Enum.Names[j].Item1, 2/*Enum index you wish to use*/);
            }
        }
        y.Write(endpath);
    }
```

### Location
```csharp
static public void RandTransform(string filepath, string endpath)
{
    UAsset y = new UAsset(filepath, UE4Version.VER_UE4_25);
    for (int i = 0; i < y.Exports.Count; i++)
    {
        if (y.Exports[i] is NormalExport us)
        {
            for (int j = 0; j < us.Data.Count; j++)
            {
                if (us.Data[j].Name.Equals(FName.FromString("RootComponent")) && us.Data[j] is ObjectPropertyData ob)
                {
                    //MessageBox.Show(y.Exports[Convert.ToInt32(ob.Value.ToString())].ObjectName.ToString());
                    if (y.Exports[Convert.ToInt32(ob.Value.ToString())] is NormalExport egg)
                    {
                        foreach (var data in egg.Data)
                        {
                            if (data.Name.Equals(FName.FromString("RelativeLocation")) && data is StructPropertyData loc)
                            {
                                loc.Value = new List<PropertyData>
                                {
                                    new VectorPropertyData(FName.FromString("Vector"))
                                    {
                                        Value= new FVector(50,50,50)
                                    }
                                };
                            }
                        }
                    }
                }
            }
        }
    }
    y.Write(endpath);
}
```
For rotators replace:
```csharp
if (data.Name.Equals(FName.FromString("RelativeLocation")) && data is StructPropertyData loc)
{
    loc.Value = new List<PropertyData>
    {
        new RotatorPropertyData(FName.FromString("Vector"))
        {
            Value= new FVector(50,50,50)
        }
    };
}
```
with this:
```csharp
if (data.Name.Equals(FName.FromString("RelativeRotation")) && data is StructPropertyData rot)
{
    rot.Value = new List<PropertyData>
    {
        new RotatorPropertyData(FName.FromString("Rotator"))
        {
            Value= new FRotator(50,50,50)
        }
    };
}
```
