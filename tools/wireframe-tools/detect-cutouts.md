# Detect Cutouts

This button will detect all of the cutouts in the scene and will [Attach](attach.md) the cutouts plane onto the lower plane.

Although dormer cutouts are automatically detected at the time of geojson generation, they are still **required** to be done in the tool. Again, there might not be any noticeable differences between detecting them in the tool or letting them get detected automatically during the geojson generation. However, when the cutouts are detected in the tool users can see what the cutouts look like before geojson generation. The location of the new vertices will also be able to be checked and adjusted.

Additionally, cutout detection is performed in the tool, all of the new cutout vertices will be red and the user will need to make sure that there are not any extra, unwanted red vertices after the detection. If there are, click on the Settings button in the Actions section of the intranet and turn off the "performcutout" setting.

From

```text
"performCutout": true
```

To

```text
"performCutout": false
```

