[![Discord](https://img.shields.io/discord/707647729043636276?color=%237289da&label=Join%20the%20blue%20fire%20discord%21&style=for-the-badge)](https://discord.gg/q4ydWSG)

# Blue Fire Modding
This is a port of the steam guide with more detail and better formatting. This guide is intended to be for the benefit of other modding communities as well (Blue Fire doesn't have a big enough modding scene to fascilitate this anyway)

**Tools and resources can be found at the bottom**

### The Basics
 - [Decompressing the pak](./Unpaking.md)
 - [Using UEViewer(Umodel) to view and extract assets](./UEViewer.md)
 - [Configuration and packaging in engine](./Engine.md) (example given is for UI or textures)
 - [Final Paking](./Paking.md)
 
### Specific mod guides
 - [Replacing models]()
 - [Disabling objects]
 - [Editing materials]
 - [Text and Dialogue]
 - [Replacing levels] (custom maps)
 - [Asset editing]
 ^ All of these can be used in conjunction with each other so feel free to experiment!
 - [Blueprint modding]
# Tools and Resources
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
  - [Heilos's](https://github.com/kaiheilos) [Asset editor](https://github.com/kaiheilos/Utilities) is an alternative to UassetGUI
  - [HxD](https://mh-nexus.de/en/downloads.php?product=HxD20) is a free hex editor that allows viewing, editing and searching through unreal engine assets
### Dialogue/Translation
  - [Unreal locres scripts](Tools/UE4_Locress_Scripts.zip) by swuforce is some scripts that allow editing of localisation files as long as file size is kept(a hex editor like HxD is needed)
  - [Kein's serialiser](Tools/UAssetSerialiser.zip) which of which use in blue fire is limited to stringtables (*[dotnet 3.0](https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-3.0.0-preview8-windows-x64-installer) is needed for this*). For use reference [this](https://docs.google.com/document/d/1krHKG9T77cfRmIQ90k4H-fy9Vm6vVm8zR6oKAlgDiww/edit)
### Blueprint modding
  - The [modloader](https://github.com/RussellJerome/UnrealModLoader) is a program by [RusselJ]() that allows injection of custom blueprints at runtime - V2 releasing very soon
  - [DRG Parser](https://github.com/Buckminsterfullerene02/DRG-Modding/tree/main/DRGParser) allows parsing of uasset and uexps to make dummying easier

# Guides
  - My [steam guide](https://steamcommunity.com/sharedfiles/filedetails/?id=2564366174) on Blue Fire modding which some sections were copied from(formatting is horrible)
  - [Dmgvol's](https://github.com/Dmgvol) [GRGuides](https://github.com/Dmgvol/GR_Guides) which covers a lot of what is covered here (this guide was based on this)
  - [atenfyr's](https://github.com/atenfyr) [astroneer modder's guide](https://docs.google.com/document/d/193p6thlTOWffF-JIeTGrLUHg9Um5i6gwMJaK4kzy9Ik) which is relevant ignoring the astroneer specific parts
  - [Buckminsterfullerine's](https://github.com/Buckminsterfullerene02) BP tutorials for DRG - relevant from 3 onwards
  - [DRG modding](https://github.com/Buckminsterfullerene02/DRG-Modding/) is a collection of DRG guides and tools by [Buckminsterfullerine](https://github.com/Buckminsterfullerene02)
  - [GHFear's](https://www.youtube.com/channel/UCRg7RCAoE_3jjibix9Ggwaw/featured) BP guides - specific to RusselJ's modloader
  - [Satisfactory modding](https://docs.ficsit.app/satisfactory-modding/latest/index.html) is in some places better than UE documentation
### Discords
 *in order of relevance*
  - [Blue Fire](https://discord.gg/q4ydWSG) is the official server for blue fire! There is a modding channel and a tolls and resources channel which is basically this
  - [UE modding](https://discord.gg/zVvsE9mEEa) is a small server aiming to pull together and gather tools and knowledge of UE modding - good if you want extra tools or more code related questions
  - [Ghostrunner modding](https://discord.gg/eZRz3Q5) is the combined modding and speedrunning server for Ghostrunner. Ghostrunner is made in the same version of unreal so is very relevant
  - [Deep Rock Galactic modding](https://discord.gg/3EVUQjz8N5) is the modding server for DRG - also made in the same version of UE
  - [Code Vein and Scarlet nexus modding](https://discord.gg/VvfvWn9) is very useful for guides
  - [Bloodstained modding](https://discord.gg/b9XBH4f) is the modding server for the Bloodstained games
  - [Illusory](https://discord.gg/JVgD2w3Npj) is useful for blueprint modding
  Extra discords can be found in [UE modding](https://discord.gg/zVvsE9mEEa)
  
### Credits
  - FatihG_ for making cool cosmetic stuff and being patient with me at the start
  - [Buckminsterfullerine](https://github.com/Buckminsterfullerene02) for making the UE modding discord 
  - [Dmgvol](https://github.com/Dmgvol) for making cool mods like an enemy randomizer and guides
  - [atenfyr](https://github.com/atenfyr)/adolescent for making UassetAPI and GUI 
  - [RusselJ](https://github.com/RussellJerome) for making the [modloader](https://github.com/RussellJerome/UnrealModLoader)
  - [Fluffyquack](https://github.com/FluffyQuack) for making tools
