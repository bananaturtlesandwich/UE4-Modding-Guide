# Dialogue

This guide will cover using [Kein's serialiser](Tools/UAssetSerialiser.zip) and the [.locres text tool](https://cdn.discordapp.com/attachments/775093920915914794/836699867920859207/unreal_locres_texttool.exe)

***These mods have major compatibility issues but replacement mods in general do anyway***

In the case of Blue Fire, there are no datatables and therefore the serialiser's use only applies for stringtables. The text that is stored in stringtables in Blue Fire includes

- Languages
- Credits
- StringNames (names of characters and voids)
- StringTable (prompts and other stuff)
- TextPopUps (The popups of text that appear next to characters)
- VoidMakerTable(unused due to the voidmaker being standalone)

The serialiser is better to use because it allows entering of data that is not equal to the normal file size

To use the serialiser, reference [this](https://docs.google.com/document/d/1krHKG9T77cfRmIQ90k4H-fy9Vm6vVm8zR6oKAlgDiww/edit) guide by FatihG_.

If the text you want to modify is not contained in these you will have to use the [.locres text tool](https://cdn.discordapp.com/attachments/775093920915914794/836699867920859207/unreal_locres_texttool.exe)

- Run the executable and select the .locres file located in localisation
- This will generate a .txt containing all of the dialogue in the game
- Make any changes you wish 
- Once you are done convert the .txt back to .locres using the executable
- Pack the file with the right file structure and your changes will be saved
