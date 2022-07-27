# The Basics
This section walks you through the basic creation of a patch mod which includes unpaking of the game's pak file, engine setup and packaging and installation of content

You will need to know:
- The file path to your game - if on steam go to your game in your library and navigate to Properties > Local Files > Browse (By default it is `C:\Program Files (x86)\Steam\steamapps\common\Your game`)
- The name of your game's project file - this is the name of the folder in your game's file path that isn't Engine
![](projectname.png)
- The file path to your game's executable - `Game file path/Game name/Binaries/Win64`
- The file path to where your game's content is stored - `Game file path/Game name/Content`
- the version of unreal your game uses - either hover over the .exe or right-click the .exe > Properties > Details and the version of unreal is the File Version which should be in the format 4.XX.X - we only care abount the 4.XX because minor versions don't fundamentally change how content is configured
![](version.png)