---
layout: default
title: Disabling Assets
parent: Specific Guides
nav_order: 2
---

**Credits to Dmgvol I basically just rewrote their guide**

*If file extensions aren't showing in file explorer enable them in the view settings*

# Disabling Objects

This is a useful way to disable actors in game - can be used for stuff like removing annoying enemies and effects among other things 

- Open umodel and find the content you would like to disable (In my case the main menu castle)

![Reference](https://user-images.githubusercontent.com/71292624/144016270-aa2de092-89c5-4c6e-98ee-b51e4af77c2a.png)

- Recreate the observed folder structure like you would in final paking (because we are dealing with cooked uassets)

*A useful shortcut for creating new folders is ctrl+shift+n and you can enter the name and press enter to go inside the folder*

- Create a blank text document with the same name as the uasset you want to disable and change the file extension to .uasset
![Structure](https://user-images.githubusercontent.com/71292624/144016288-14d72fd8-2cbf-494f-af5f-4a041d146fb6.png)

- Package the folder, place in mod folder and run the game
![NoCastle](https://user-images.githubusercontent.com/71292624/144016330-f20d14ec-d849-4c81-9eb6-95f4eece6937.png)
