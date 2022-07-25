- Create a folder named `ModName_P` (the `_P` clarifies it as a patch so that it overwrites original game content)
- Create a folder inside this which is the name of the executable in your game folder
- Go into the folder where you packaged your mod and copy the Content folder in `WindowsNoEditor\ProjectName` into this folder
- Folder structure is very important for UE4 modding so make sure spellings of the folders are the same as they were when exported
- Download [Unrealpak](fluffyquack.com/tools/unrealpak.rar) by FluffyQuack and drag the mod folder onto UnrealPak-with-compression.bat
![](../../images/Pak.png)

- This will create a pak file. make sure the pak file contains a _P at the end of its name and create a folder in your Paks folder called ~mods

(The folder is just to ensure proper load order. The folder can be named anything that starts with a letter after the first letter of the game pak) 
- Place the pak file in it and run your game to see if it worked. Hopefully you should find it did.

![](../../images/drip.png)

If the mod worked, give yourself a pat on the back! 