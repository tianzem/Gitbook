# Vertical Planes

```text
Re Adnan's 
1) Please always remember to delete the vertical planes
```

A Vertical Plane is defined as a plane whose slope is greater than 80 degrees. You can select the plane in the tool and go to the properties to check the Slope number, and see if it will be detected.

Vertical Planes are going to be **neglected** automatically during the Detect Edge Types and Generate GeoJson. So you can imagine that there is not going to be any difference between you deleting the planes in the 3Dtool, or just leaving them to be neglected in the GeoJson generation.

But, we still highly recommend to Delete the Vertical Planes in the 3Dtool since our workflow may not delete a plane with 79 degrees, even though you definitely want it to be deleted. It is always much safer to visualize everything in the tool instead of assuming something will be fixed automatically.

