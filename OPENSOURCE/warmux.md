# Warmux

Warmux is a Worms-like game where the players fight on a 2D map with funny weapons.

## Maps

To make your own map, you need to have files and create new folder with map name:

- config.xml (XML configuration map file)
- map.png (PNG transparent image map file)
- sky.png or sky.jpg (static image file of sky background)
- preview.jpg (preview thumbnail, must be at 300x225 JPEG compressed image file)

config.xml template in data/map/example folder:

```xml
<?xml version="1.0" encoding="utf-8"?>
<!DOCTYPE resources SYSTEM "../map.dtd" []>
<resources>
	<author>
		<name>[your name]</name>
		<nickname>[nickname]</nickname>
		<email>[your email, make sure you replace @ by AT, just in case]</email>
		<country>[like where are you from]</country>
	</author>

	<description>Sample description.</description>
	<surface name="sky" file="sky.png" />
	<surface name="map" file="background.png" />
	<surface name="preview" file="preview.jpg" />

	<name>[title artwork]</name>
	<water>no</water> <!-- you can specify no to disable it, water or lava to activate it -->
	<nb_mine>10</nb_mine>
	<is_open>1</is_open> <!-- if it's 0, then it's closed. Otherwise it's open -->

	<music_playlist>woodlux</music_playlist> <!-- see the data/music/ingame folder, reads the woodlux.m3u as music playlist for example -->
</resources>
```

- Martin Eesmaa
