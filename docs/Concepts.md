### Pak files
- Pak files are essentially archive files that store most of the resources that the game in question requires to run
- The game's main pak will always be contained in the `Content/Paks` directory
- Pak files will sometimes be encrypted via AES keys, however these can normally be found easily with GHFear's [AESkeyFinder](https://zenhax.com/viewtopic.php?t=9407&start=20)
- Pak files can also be splitted into chunks for a bit of extra security
- Pak files are normally able to be viewed with [UEViewer](https://www.gildor.org/en/projects/umodel) or [Fmodel](https://fmodel.app/)
### Mod Loading
- Traditional mods are loaded as pak files in the same directory as the main game pak
- These mods will likely need a `_P` at the end of their name to remove the mount point of the pak and clarify it as a patch of sorts
- The mods should be place in a mod folder (`~mods` works for every game) to ensure proper load order (so the mods aren't loaded before the main game pak)
- Paks are loaded alphabetically
- Mods can also be loaded via other methods such as the [Universal Unreal Mod Loader](https://github.com/RussellJerome/UnrealModLoader)
### Cooking
- Before being put in a pak file, assets undergo a process called cooking where the data used by the engine is erased so only the data needed for the game is in the final pak
- Cooked assets are not able to be edited in the engine however they can be edited through the use of programs such as [UAssetGUI](https://github.com/atenfyr/UAssetGUI)
