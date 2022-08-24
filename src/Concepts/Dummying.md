# Dummying
- There is a trick called dummying that can be utilised in many situations
- How it works is that you create an empty asset that is the same name and type as an asset in the original pak file
- Another asset will reference this and will contain references after cooking
- In final mod packaging, you leave out the dummy asset
- This means that in game the asset that was dummied is used instead

## Examples
**Mesh modding**
- If you want the mesh to continue to use the materials it uses normally then you would dummy the materials/material instances that it uses
- In packaging these are removed and the mesh uses the original materials in game

**Blueprint modding**
- You can dummy an actor or function library to use a function from it
- The dummy asset is created and a function is added with the same name, parameters and output as the original one
- Another actor (loaded via some means) calls this function from the dummy
- The dummy is removed and the function is called from the original blueprint in game