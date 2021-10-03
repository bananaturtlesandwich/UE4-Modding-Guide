# Dialogue

This guide will cover using [Kein's serialiser](Tools/UAssetSerialiser.zip) and the [locres extract scripts](Tools/UE4_Locress_Scripts.zip)

***These mods have major compatibility issues but replacement mods in general do anyway***

In the case of Blue Fire, there are no datatables and therefore the serialiser's use only applies for stringtables. The text that is stored in stringtables in Blue Fire includes

- Languages
- Credits
- StringNames(names of characters and voids)
- StringTable(prompts and other stuff)
- TextPopUps(The popups of text that appear next to characters)
- VoidMakerTable(The base for the WIP Void Editor)

The serialiser is better to use because it allows entering of data that is not equal to the normal file size

To use the serialiser, reference [this](https://docs.google.com/document/d/1krHKG9T77cfRmIQ90k4H-fy9Vm6vVm8zR6oKAlgDiww/edit) guide by FatihG_.

If the text you want to modify is not contained in these you will have to use the [locres extract scripts](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Tools/UE4_Locress_Scripts.zip)

- For use of the .locres extract scripts run the newest executable and select the .locres file in the localisation folder
- This will generate a .txt with what seems like nonsense
- Open the file in HxD and you be able to view all the dialogue in the game
- Search for the dialogue you want to change using ctrl+f
- Make the changes without changing the file size(If you the text is shorter you can fill the space with spaces and it'll work fine)
- Once you are done convert the .txt back to .locres using the other executable
- Pack the file with the right file structure
