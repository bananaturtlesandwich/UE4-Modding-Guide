For this example I will use my Fara discord shirt as an example. Here is the original texture for Fara. https://steamuserimages-a.akamaihd.net/ugc/1709664850606837319/94421BCF13CCF62057D68B2F34BBB63B582692BC/?imw=256&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false
I have now changed it so that the model will have the desired change
https://steamuserimages-a.akamaihd.net/ugc/1709664850606856675/0000A84B4B6DB8DA36FFAC47A1767A0F4392A2D5/?imw=256&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false

Open Unreal Engine 4.25.4 and create a blank game project with no starter content
https://steamuserimages-a.akamaihd.net/ugc/1709664850606866461/8CA8A3C66DB648342384313F659199657E023B61/?imw=256&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false

Go into project settings and uncheck use pak file
https://steamuserimages-a.akamaihd.net/ugc/1709664850606950196/09F243EA9A7635579600DDBFD3F2B4C519B12801/?imw=256&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false
https://steamuserimages-a.akamaihd.net/ugc/1709664850606950638/89E34EA0B9EE88A52F5EFC0FCA838885F82FBDB7/?imw=256&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false
Now recreate the folder structure that was obtained from exporting from umodel in Unreal engine. In my case the folders went UmodelExport\BlueFire\NPC\Fara\Textures so I must create the folders like this:
https://steamuserimages-a.akamaihd.net/ugc/1709664850606873773/B80DD86973DC9CECFC0378515BC2AD1AA12E8BD2/?imw=256&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false
Now ctrl+shift+S to save all and navigate to file>package project>Windows(64-bit). Select the folder you want to cook the mod into and wait for the mod to package.
Final Paking Edit
Go into the folder where you packaged your mod and copy the BlueFire folder in Cooked\WindowsNoEditor\*insert project name*\Content into a new folder which your mod will be contained in. Create a folder called Content and a folder called Blue Fire. Place BlueFire into Content and place content into Blue Fire. Folder structure is very important for UE4 modding so make sure spellings of the folders are the same as they were when exported. Extract unrealpak and drag the mod folder onto UnrealPak-with-compression.exe
https://steamuserimages-a.akamaihd.net/ugc/1709664850606994005/70457718BB7914DA005A6BAC424150C2E3B7F075/?imw=256&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false

This will create a pak file. Rename the pak file with a _P at the end and place it in C:\Program Files (x86)\Steam\steamapps\common\Blue Fire\Blue Fire\Content\Paks and run Blue Fire to see if it worked. Hopefully you should find it did.
https://steamuserimages-a.akamaihd.net/ugc/1709664850606911512/45048623DB665CF9F0DF09F0A7D596E4A1552090/?imw=256&&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=false
