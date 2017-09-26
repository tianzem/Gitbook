**Special Case**

**Overhang:**

Typically, it is hard to find the image with the vertex under the overhang, but it might be easier to change the vertex in the 3D view.

1. Find three vertices on that plane and press Space to Lock the plane. If there are less than 3 vertices, Create some.
2. Under modify mode, Drag the vertex in the 3D view. Since the plane has been locked, so all the movements are only allowed in that plane.
3. Turn on the Adjust Vertices panel to see the 2D view of the vertices to help you find the exact location of the vertices.

**Trees:**

Tree shadow will destroy a part of the point cloud, usually, it will be a cornor.

1. Create the two uncompleted edges near the corner.
2. Use Intersect Lines function to intersect the two edges to generate the corner point.
3. Turn on the Edge Dimensions layer to double check the corner location.

**Chimney:**

Chimneys are on the edge of the roof. It is not hard to draw, but if you want to make the GeoJSON looks better, Align function is very useful, just Align the flashing of the chimney with the nearby edges.

**Penetration:**

Penetrations are needed for solar projects.

1. Same as how to deal with the Overhang. Lock the plane - Drag the vertex in the 3D view - Check the vertices location in the 2D view.
2. Always turn on the Edge Dimensions layer and Align the relative edges to make sure the penetration is either a square or rectangle.



