 ### ***Neither BMS scripts or the CMD method seems to work anymore for blue fire so the last method must be used***

# Unpaking 
**Sections**
- [BMS scripts](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Unpaking.md#bms-scripts)
- [When BMS scripts don't work](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Unpaking.md#when-bms-scripts-dont-work)
- [Fmodel](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Unpaking.md#when-neither-of-these-methods-work)

# BMS scripts
- Download [BMS scripts](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Tools/BMS%20scripts.zip) by Luigi Auriemma and place them into your paks folder
- Drag the main pak file onto extract-all.bat 
![](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Images/BMS.png)
- If this doesn't work try running the .exes and following the instuctions and it may work
- if not, then try the next method

# When BMS scripts don't work

*To find the version of UE your game uses hover over the game exe and it will show the version*

[Here's a video detailing the process](https://youtu.be/AElxgCRXF64)

However here's a summary if some things are unclear:
Blue Fire is a game made with unreal engine 4.25 so uses pak files to store data. To access this data you must unpak this pak file. For this, you must have Unreal Engine 4.25.4 installed from the epic games launcher.
Open command prompt and drag unrealpak.exe into command prompt. This .exe should be stored in UE_4.25\Engine\Binaries\Win64\UnrealPak.exe
![](Images/unrealpak.PNG)

Then put a space and drag the pak file into command prompt. This file should be located in Steam\steamapps\common\Blue Fire\Blue Fire\Content\Paks assuming you installed it from steam. If you installed in on GOG then this will be in GOG games\Blue Fire\Blue Fire\Content\Paks

![](Images/Pakfile.PNG)

Put a space and type -Extract. Finally put a space after that and enter the directory of the folder you want the assets to be extracted to. Press enter and the game files should extract to the folder.

If there is an error, remember that syntax in important- here's mine for reference
"C:\Program Files (x86)\UE_4.25\Engine\Binaries\Win64\UnrealPak.exe" "C:\Program Files (x86)\Steam\steamapps\common\Blue Fire\Blue Fire\Content\Paks" -Extract C:\modding\BF_Unpaked


# When neither of these methods work

- Install [Fmodel](https://fmodel.app/) by Jetbrains and open the pak directly
- Complete setup
![](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Images/Fmodel.png)
- Export all directories you need

*It is not recommended to export everything as it takes ages and some folders like audio are useless for Blue Fire*

# **[Next step](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/UEViewer.md)**
