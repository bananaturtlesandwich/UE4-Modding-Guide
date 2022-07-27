# Mod Loading
- Traditional mods are loaded as pak files in the same directory as the main game pak (these pak files are created using a tool such as [unrealpak](https://fluffyquack.com/tools/unrealpak.rar))
- The content inside these paks files will just be content that has been created and then cooked using the same version of unreal as the game in question
- These mods will likely need a `_P` at the end of their name to remove the mount point of the pak and clarify it as a patch so that it overwrites original game content
- The mods should be place in a mod folder (`~mods` works for every game) to ensure proper load order (so the main game pak doesn't overwrite the mod's content)
- Paks are loaded alphabetically in each directory
- Mods can also be loaded via modloader frameworks such as the [Unreal Mod Loader](https://github.com/RussellJerome/UnrealModLoader) (a tool that allows the execution of any arbitrary blueprint code) and [UE4SS](https://github.com/UE4SS/UE4SS) (a tool that allows Lua scripting via reflection)