---
layout: default
title: Configuration and Packaging in Engine
parent: The Basics
nav_order: 3
---

***While this is an example for a texture mod, the way in which the project is configured is very much the same for each mod***

# Config and packaging

### Content creation
**I will not cover content creation in this. Just examples.**
- For this example I will use my Fara discord shirt mod. Here is the original texture for Fara.
![](Images/FaraTexture.png)

- I have now changed it so that the model will have the desired change
![](Images/Fara_Texture.png)

### Setting up
- Open up your version of Unreal Engine 4 and create a blank game project with no starter content(You can include this if you want it doesn't really matter)
![](Images/UE.PNG) ![](Images/UE2.PNG) ![](Images/UE3.PNG)

- Go into edit > project settings and uncheck use pak file

- Now recreate the folder structure that was obtained from exporting from umodel in Unreal engine. In my case the folders went UmodelExport\BlueFire\NPC\Fara\Textures so I must create the folders like this:
![](Images/UE4.PNG)

### Package
- Now ctrl+shift+S to save all and navigate to file>package project>Windows(64-bit). Select the folder you want to cook the mod into and wait for the mod to package.

# **[Next Step](https://github.com/bananaturtlesandwich/Blue-Fire-Modding-Guide/blob/main/Paking.md)**
