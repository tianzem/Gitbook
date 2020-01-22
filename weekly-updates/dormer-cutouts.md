# Dormer Cutouts

```text
Re Adnan's 
2) Dormer cutouts are not required to be done in the wireframe. 
They are automatically detected at the time of geojson generation.
```

Although dormer cutouts are automatically detected at the time of GeoJson generation, they are still **required** to be done in the 3Dtool. Again, there might not be any difference between detecting it in the tool versus letting it get detected automatically during the GeoJson generation. However, if you do it in the 3Dtool, you get to see what the cutouts will look like and you can check, or even adjust, the location of the new cutout vertices.

Besides, if you do the cutout detection in the 3Dtool, all of the new vertices will be red and you will need to make sure that there are not any extra unwanted red vertices after the detection. If there are, go to the Settings in the intranet and turn off the "performcutout" setting:

From

```text
   "performCutout": true
```

To

```text
   "performCutout": false
```

## 

