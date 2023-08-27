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
![FaraTexture](https://user-images.githubusercontent.com/71292624/144013420-4a950ba0-0815-47ed-90da-7796aae2a46c.png)

- I have now changed it so that the model will have the desired change
![FaraTexture](https://user-images.githubusercontent.com/71292624/144013468-f53bd02f-390e-438d-ba8d-af243066a69d.png)

### Setting up
- Open up your version of Unreal Engine 4 and create a blank game project with no starter content(You can include this if you want it doesn't really matter)
![UE](https://user-images.githubusercontent.com/71292624/144013512-cecb0828-7078-4e27-91e4-b3a3e04d6396.PNG)
![UE2](https://user-images.githubusercontent.com/71292624/144013508-530a25ba-d00a-448e-8ba2-59e2edd06a00.PNG)
![UE3](https://user-images.githubusercontent.com/71292624/144013511-4952b92b-2490-4d79-bca7-10f0a0cfe8dc.PNG)

- Go into edit > project settings and uncheck use pak file

- Now recreate the folder structure that was obtained from exporting from umodel in Unreal engine. In my case the folders went UmodelExport\BlueFire\NPC\Fara\Textures so I must create the folders like this:
![UE4](https://user-images.githubusercontent.com/71292624/144013559-8313cc9c-8440-48f6-a284-e7bb62a47bc4.PNG)


### Package
- Now ctrl+shift+S to save all and navigate to file>package project>Windows(64-bit). Select the folder you want to cook the mod into and wait for the mod to package.

# **[Next Step](./Paking.md)**
