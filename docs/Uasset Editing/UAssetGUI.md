---
layout: default
title: UassetGUI
parent: Uasset Editing
nav_order: 1
---

# UAssetGUI

- [UAssetGUI](https://github.com/atenfyr/UAssetGUI) is a powerful tool by [atenfyr](https://github.com/atenfyr) that is a wrapper of UAssetAPI
- It allows the editing of unreal engine 4 assets through an intuitive user interface
- This skips having to dummy assets like materials just to change values that are already in the .uasset
- **However for larger-scale mods such as my randomiser, [UassetAPI](https://github.com/atenfyr/UAssetAPI) may be able to suit your needs better**

- First, download the .exe and prerequisite .dlls from [this page](https://github.com/atenfyr/UAssetGUI/releases)(It needs dotnet to run)
- Extract a .uasset and .uexp using Fmodel's export function or umodel's save packages function
- Right-click any .uasset(include the associated .uexp inside the same folder) and click "open with"
- You can then create an association with uassetGUI by finding it in the pop-up and checking the "always open files of this type with" checkbox
- You can now see the exports and their data in the file - such as parameters of a material or the enum index of an item in an enum
- You can now edit these logically and save it to a separate file using save as or ctrl+shift+s or save to the same file using save or ctrl+s
- You can now recreate the file structure and pak and it should work as expected