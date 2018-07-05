# Detect Cutouts

It is going to detect all the cutouts in the scene and [Attach](./#attach) the cutouts plane into the lower plane.

Although dormer cutouts are automatically detected at the time of geojson generation, they are still **required** to be done in the tool. Again, there might not be any differences between to detect it in the tool or let it get detected automatically during the geojson generation. But if you do it in the tool, you will see how the cutouts will look like and you could check or even adjust the location of the new vertices.

Besides, if you do the cutout detection in the tool, all the new vertices will become red and you need to make sure there is not any extra red vertices after the detection. If there are, go to the settings in the intranet and turn off the "performcutout"

From

```text
"performCutout": true
```

To

```text
"performCutout": false
```

