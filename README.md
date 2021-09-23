[![Discord](https://img.shields.io/discord/707647729043636276?color=%237289da&label=Join%20the%20blue%20fire%20discord%21&style=for-the-badge)](https://discord.gg/q4ydWSG)

# Blue-Fire-Modding
This is a port of the steam guide with more detail and better formatting

**Tools and resources can be found at the bottom**

### The Basics
 - [Decompressing the pak](./Unpaking.md)
 - [Using UEViewer(Umodel) to view and extract assets](./UEViewer.md)
 - [Configuration and packaging in engine](./Engine.md)
 - [Final Paking](./Paking.md)
 
### Specific mod guides
 - [Replacing models]
 - [Replacing textures and UI]
 - [Disabling objects]
 - [Editing materials]
 - 
  All of these can be used in conjunction with each other so feel free to experiment!
  
### Tools and Resources
 ### General modding  
  - [Umodel](https://www.gildor.org/en/projects/umodel) by [Gildor](https://github.com/gildor2) for The viewing and export of game assets
  - [Epic Games launcher](https://www.epicgames.com/store/en-US/download) by Epic Games where you can download Unreal Engine
  - [UnrealPak scripts](./Tools/UnrealPak.zip) By [Fluffyquack](https://github.com/FluffyQuack) used for final paking
 
 ### Models
  - [Blender](https://www.blender.org/download/) by the [Blender foundation](https://github.com/blender) for 3d modelling
  - [PSK and PSA importer](https://github.com/Befzz/blender3d_import_psk_psa) by [Befzz](https://github.com/Befzz) for importing exported meshes and armatures
  
 ### Code/Uasset editing
  - [Fmodel](https://fmodel.app/) by Jet Brains in an alternative to umodel that is stronger than umodel with more text based formats (this may change because fmodel receives regular updates)
  - [UassetAPI](https://github.com/atenfyr/UAssetAPI) by [atenfyr](https://github.com/atenfyr) is an API that can read and modify UE4 game assets via C# scripting
  - [UassetGUI](https://github.com/atenfyr/UAssetGUI/releases) by [atenfyr](https://github.com/atenfyr) is a thin wrapper of UassetAPI with a user interface which is more user friendly than coding with uassetAPI 
### Dialogue/Translation
  - [Unreal locres scripts](Tools/UE4_Locress_Scripts.zip) by swuforce is some scripts that allow editing of localisation files as long as file size is kept
  - [Kein's serialiser](Tools/UAssetSerialiser.zip) which of which use in blue fire is limited to stringtables (*[dotnet 3.0](https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-3.0.0-preview8-windows-x64-installer) is needed for this*). For use reference [this]
