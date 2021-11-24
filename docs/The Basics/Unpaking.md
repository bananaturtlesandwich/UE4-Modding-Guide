---
layout: default
title: Decompressing the .pak
parent: The Basics
nav_order: 1
---

***Neither BMS scripts or the CMD method seems to work anymore for blue fire so the last method must be used***

# Unpaking 
**Sections**
- [Fmodel](./Unpaking.md#fmodel)
- [QuickBMS](./Unpaking.md#quickbms)
- [When BMS scripts don't work](./Unpaking.md#using-unrealpak-directly)

# Fmodel

- Install [Fmodel](https://fmodel.app/) by Jetbrains and open the pak directly
- Complete setup
![Fmodel](https://user-images.githubusercontent.com/71292624/144013014-43192799-6647-48db-b908-d8519f444246.png)

- Explore and then export any files you need

### *It is not required to export everything and fmodel provides more functions so the above method is more recommended, however the other methods are listed below*

# QuickBMS
- Download [QuickBMS](https://aluigi.altervista.org/papers/quickbms.zip) by Luigi Auriemma and [unrealtournament.bms](https://aluigi.altervista.org/bms/unreal_tournament_4.bms) and place them into your paks folder
- Drag the bms file onto the exe that corresponds to the file size of the pak file
- Follow the instructions in the application and the files should extract
- if not, then try the next method

# Using UnrealPak directly

*To find the version of UE your game uses hover over the game exe and it will show the version*

[Here's a video detailing the process](https://youtu.be/AElxgCRXF64)

However here's a summary if some things are unclear:
Blue Fire is a game made with unreal engine 4.25 so uses pak files to store data. To access this data you must unpak this pak file. For this, you must have Unreal Engine 4.25.4 installed from the epic games launcher.
Open command prompt and drag unrealpak.exe into command prompt. This .exe should be stored in UE_4.25\Engine\Binaries\Win64\UnrealPak.exe

![unrealpak](https://user-images.githubusercontent.com/71292624/144012916-27e3cd6d-3851-472f-a42f-63d72c7a60f8.PNG)

Then put a space and drag the pak file into command prompt. This file should be located in Steam\steamapps\common\Blue Fire\Blue Fire\Content\Paks assuming you installed it from steam. If you installed in on GOG then this will be in GOG games\Blue Fire\Blue Fire\Content\Paks

![Pakfile](https://user-images.githubusercontent.com/71292624/144012957-18158f5b-b9c8-4d09-b778-4d47b248c0d2.PNG)

Put a space and type -Extract. Finally put a space after that and enter the directory of the folder you want the assets to be extracted to. Press enter and the game files should extract to the folder.

If there is an error, remember that syntax in important- here's mine for reference
`"C:\Program Files (x86)\UE_4.25\Engine\Binaries\Win64\UnrealPak.exe" "C:\Program Files (x86)\Steam\steamapps\common\Blue Fire\Blue Fire\Content\Paks" -Extract C:\modding\BF_Unpaked`

# **[Next step](./UEViewer.md)**
