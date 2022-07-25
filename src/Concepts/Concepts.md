# Core UE4 Modding Concepts

### .pak files
- Pak files are essentially archive files that store most of the resources that the game in question requires to run (think differently structured .zip files)
- The game's main pak will always be contained in the `Content/Paks` directory
- Pak files will sometimes be encrypted via AES keys, however these can be easilyfound  with [AESkeyFinder](https://zenhax.com/viewtopic.php?t=9407&start=20)
- Pak files can also be splitted into chunks for a bit of extra security
- Pak files are normally able to be viewed with [UEViewer](https://www.gildor.org/en/projects/umodel) or [Fmodel](https://fmodel.app/)
### Mod Loading
- Traditional mods are loaded as pak files in the same directory as the main game pak (these pak files are created using a tool such as [unrealpak](https://fluffyquack.com/tools/unrealpak.rar))
- The content inside these paks files will just be content that has been created and then cooked using the same version of unreal as the game in question
- These mods will likely need a `_P` at the end of their name to remove the mount point of the pak and clarify it as a patch so that it overwrites original game content
- The mods should be place in a mod folder (`~mods` works for every game) to ensure proper load order (so the main game pak doesn't overwrite the mod's content)
- Paks are loaded alphabetically in each directory
- Mods can also be loaded via modloader frameworks such as the [Unreal Mod Loader](https://github.com/RussellJerome/UnrealModLoader) (a tool that allows the execution of any arbitrary blueprint code) and [UE4SS](https://github.com/UE4SS/UE4SS) (a tool that allows Lua scripting via reflection)
### Cooking
- Before being put in a pak file, assets undergo a process called cooking where the data used by the engine is erased so only the data needed for the game is in the final pak
- Cooked assets are not able to be edited in the engine however they can be edited through the use of programs such as [UAssetGUI](https://github.com/atenfyr/UAssetGUI) or [Asset Editor](https://github.com/kaiheilos/Utilities)
### .uasset,.umap,.uexp and .ubulk files
- Data is stored in .uasset or .umap files both before and after packaging(.umap files are only used for levels), however after cooking the file structure is different from the structure beforehand
- If the event driven loader is used by the game (introduced around version 4.15) then the cooked file is also split up into the .uasset and the .uexp for faster loading
- In the above case the .uasset/.umap file defines the structure of the asset while the associated .uexp holds the data
- In some cases where more external data is required a .ubulk file is generated which stores this external data such as baked lightmaps for levels
