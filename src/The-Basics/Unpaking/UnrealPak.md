# Using UnrealPak directly

**This method will extract all of the raw assets out of the pak file so if you don't have space then I suggest [umodel](UEViewer.md) or [fmodel](FModel.md)**

**The advantage of this is immediate access to a file system with correct folder structure**

**With this method you will need to extract models and textures from the raw assets using [umodel](UEViewer.md) or [fmodel](FModel.md)**

**With this method you will also need the version of unreal engine installed that your game uses - you will need this later on anyway**

**This method does not support extracting all pak chunks at once**

[Here's a video detailing the process](https://youtu.be/AElxgCRXF64)

However here's a summary if some things are unclear:
- Open command prompt and drag unrealpak.exe into command prompt. This .exe should be stored in UE_4.XX\Engine\Binaries\Win64\UnrealPak.exe
![](unrealpak.png)

- Then put a space and drag the pak file into command prompt

- Put a space and type -Extract

- Put a space after that and enter the directory of the folder you want the assets to be extracted to

- Press enter and the game files should extract to the folder

- If there is an error, remember that syntax in important - here's mine for blue fire as reference
`"C:\Program Files (x86)\UE_4.25\Engine\Binaries\Win64\UnrealPak.exe" "C:\Program Files (x86)\Steam\steamapps\common\Blue Fire\Blue Fire\Content\Paks" -Extract C:\modding\BF_Unpaked`

- If your game is incompatible, try a different method