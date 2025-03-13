# Notes

## Setup
https://hterrain-plugin.readthedocs.io/en/latest/
1. Create a new Forward+ project in Godot 4.4
1. Select "AssetLib"
1. Search for "Height"
1. Select "Heightmap terrain" and then "Download"
1. Select "Project" > "Project Settings..."
1. Select "Plugins"
1. Select the box to enable "Heightmap Terrain"
1. Create a new 3d Scene
1. Rename the scene "Main" and save as `scenes/main.tscn`
1. Select "Add Child Node..." > "HTerrain" 
1. In the Inspector for the HTerrain, select the folder icon next to "Data Directory"
1. Create a new folder named `data` and select that folder
	1. Data directory should now be set as "res://data"
	1. You should now have a white sqaure in your scene, orginating at (0, 0, 0)

## Textures
https://youtu.be/Af1f2JPvSIs?t=178
</br>https://github.com/Arnklit/TutorialResources/blob/main/Simple%20Terrain/grass.png
1. In the root of the project, create a new folder named `assets`
1. Download the 1K-JPG.zip for:
	- https://ambientcg.com/view?id=Ground037
	- https://ambientcg.com/view?id=Rocks006
	- https://ambientcg.com/view?id=Rocks007
	- https://ambientcg.com/view?id=Rock028
1. Unarchive the zip files in the assets directory
1. Select "3D"
1. Select the HTerrain node from the scene tree
1. Select "Import..." next to "Textures"
1. Set the Resolution to `1024`
1. Select "..." for Import Directory
1. Create a new folder named `textures` and select that folder
	- Import Directory should now be "res://textures"
1. Select "+" to add "Texture 0"
1. Select "Load..." under "Albedo"
1. Navigate to and select "assets\Ground037_1K-JPG\Ground037_1K-JPG_Color.jpg"
1. For the "Normal" texture, find the "...NormalGL.jpg" and select "Flip Y"
1. Select "+" to add "Texture 1"
1. Select "Load..." under "Albedo"
1. Navigate to and select "assets\Rocks006_1K-JPG\Rocks006_1K-JPG_Color.jpg"
1. For the "Normal" texture, find the "...NormalGL.jpg" and select "Flip Y"
1. Select "+" to add "Texture 2"
1. Select "Load..." under "Albedo"
1. Navigate to and select "assets\Rocks007_1K-JPG\Rocks007_1K-JPG_Color.jpg"
1. For the "Normal" texture, find the "...NormalGL.jpg" and select "Flip Y"
1. Select "+" to add "Texture 3"
1. Select "Load..." under "Albedo"
1. Navigate to and select "aassets\Rock028_1K-JPG\Rock028_1K-JPG_Color.jpg"
1. For the "Normal" texture, find the "...NormalGL.jpg" and select "Flip Y"
1. Select "Import to TextureSet"
1. Select "OK" and then "Close"
1. In the Inspector for the HTerrain, navigate to "Rendering" > "Shader Params" "U Tile Reduction"
1. Set the values to `1.0`


</br>Classic4 shader limits the textures to 4, with the 4th being earmarked for cliff faces.
</br>Changing to 16 but I was unable to create a Texture Array.

## Models
- [SketchUp Residency Title Stonehenge](https://sketchfab.com/3d-models/sketchup-residency-title-stonehenge-b045d1987a2e44388a9c1431fe6db55e) - SKETCHUP RESIDENCY
