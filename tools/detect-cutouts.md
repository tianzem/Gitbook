# Detect Cutouts

This button will detect all of the cutouts in the scene and will [Attach](./#attach) the cutouts plane onto the lower plane.

Although dormer cutouts are automatically detected at the time of geojson generation, they are still **required** to be done in the tool. Again, there might not be any noticeable differences between detecting them in the tool or letting them get detected automatically during the geojson generation. However, when you detect them in the tool you will see what the cutouts look like before geojson generation. You will also be able to check, or even adjust, the location of the new vertices.

Additionally, if you do the cutout detection in the tool, all of the new cutout vertices will be red and you need to make sure that there are not any extra unwanted red vertices after the detection. If there are, go to the settings in the intranet and turn off the "performcutout" setting.

From

```text
"performCutout": true
```

To

```text
"performCutout": false
```

