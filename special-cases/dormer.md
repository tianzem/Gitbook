# Dormer

1. First, finish the dormer as normal. There is no need to draw the outline of the shadow that is underneath the dormer in the lower plane.

   ![](../.gitbook/assets/dormer1.jpg)

2. Lock the plane and adjust the top three vertices of each dormer.
3. After you save and generate the resources, the QA tool is going to recognize the dormers as cutouts automatically. You need to double check that the dormer cutouts were detected in the GeoJSON.

![](../.gitbook/assets/dormer2.jpg)

Although dormer cutouts are automatically detected at the time of GeoJson generation, they are still **required** to be done in the 3Dtool. Again, there might not be any difference between detecting it in the tool versus letting it get detected automatically during the GeoJson generation. However, if you do it in the 3Dtool, you get to see what the cutouts will look like and you can check, or even adjust, the location of the new cutout vertices.

Furthermore, if you do the cutout detection in the 3Dtool, all of the new vertices will be red and you will need to make sure that there are not any extra unwanted red vertices after the detection. If there are, go to the Settings in the intranet and turn off the "performcutout" setting:

From

```text
   "performCutout": true
```

To

```text
   "performCutout": false
```



