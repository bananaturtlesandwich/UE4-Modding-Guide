# Unreal files
- Data is stored in .uasset or .umap files both before and after packaging(.umap files are only used for levels), however after cooking the file structure is different from the structure beforehand
- If the event driven loader is used by the game (introduced around version 4.15) then the cooked file is also split up into the .uasset and the .uexp for faster loading
- In the above case the .uasset/.umap file defines the structure of the asset while the associated .uexp holds the data
- In some cases where more external data is required a .ubulk file is generated which stores this external data such as baked lightmaps for levels