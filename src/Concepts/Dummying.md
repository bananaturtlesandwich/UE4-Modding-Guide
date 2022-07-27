# Dummying
- There is a trick called dummying that can be utilised in many situations
- How it works is that you create an empty asset that is the same name and type as an asset in the original pak file
- Another asset will reference this and will contain references after cooking
- In final mod packaging, you omit the dummy asset but nothing else
- This means that in game instead of the dummy asset the other asset will use the asset in the pak

- The most notable example of this is in mesh modding
- If you want the mesh to continue to use the materials it uses then you would dummy the materials and material instances that it uses
- In packaging these are removed and the mesh uses the original materials in game

- Another interesting example is dummying an actor or function library to use a function
- The dummy asset is created and a function is added with the same name, parameters and output as the original one
- Another actor calls this function as normal
- The dummy is removed and the function is used as normal in-game