---
layout: default
title: Final Packaging
parent: The Basics
nav_order: 4
---

# Final Paking

- Go into the folder where you packaged your mod and copy the Content folder in WindowsNoEditor\\ProjectName into a new folder which your mod will be contained in, for example FaraDrip_P (the _P will be in the pak name and is so the file gets identified as a patch).
- Now recreate the folder structure outside of content (In Blue Fire's case a folder called Blue Fire)
- Folder structure is very important for UE4 modding so make sure spellings of the folders are the same as they were when exported
- Download [Unrealpak](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Tools/UnrealPak.zip) by FluffyQuack and drag the mod folder onto UnrealPak-with-compression.bat
![](Images/Pak.png)
![Pak](https://user-images.githubusercontent.com/71292624/144015541-6179a4c4-18b5-4187-8f7a-1d8d1e0d80ac.png)

- This will create a pak file. make sure the pak file contains a _P at the end of its name and create a folder in C:\Program Files (x86)\Steam\steamapps\common\Blue Fire\Blue Fire\Content\Paks called ~mods

(The folder is just to ensure proper load order. The folder can be named anything that starts with a letter after the first letter of the game pak) 
- Place the pak file in it and run Blue Fire to see if it worked. Hopefully you should find it did.

![drip](https://user-images.githubusercontent.com/71292624/144015578-fa7e09a5-d641-4f25-9292-323db58763bb.PNG)

Guides on more types of mods are coming and can be found in the main [README](./README.md)

If the mod worked, feel free to submit it to our [nexus mods page](https://www.nexusmods.com/bluefire/mods/) 
