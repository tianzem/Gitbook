**Feature Use:**

**\(Red: Button, Blue: Keyboard/Mouse, Purple: Keyword\)**

**Align:**

1. \(Optional\) Under Modify and Surface mode, select a plane which you would like the edge to fix in and press Space to lock it.
2. Under Modify and Vertex mode, select \(or Hold Ctrl to multiply select the lines\) you want to align with.
3. Click Align or press Shift to change to Align mode, and click the Target edge.
4. The edges you selected on Step 2 will be aligned with the Target you selected on Step 3 and fixed in the plane you selected on Step 1.

**Surface:**

1. Under Modify and Surface mode, select a plane which you would like the edge to fix in and press Space to lock it.
2. Under Modify and Vertex mode, Hold and Drag the vertex on 3D view. The vertex can be only moved on the relative plane.

**Lock Edge:**

1. Under Modify and Vertex mode, select a edge which you would like the vertices to fix in and press Space to lock it.
2. Under Modify and Vertex mode, Hold and Drag the vertex on 3D view. The vertex can be only moved on the relative edge.

**Scale:**

1. Click Set Scale and then select either the line you know the measurements.
2. If you want to change the unit, click the dropdown menu to transform between Meter and FT.If you want to scale the point cloud, change the unit first and input the new length.
3. After click Apply, and turn on the Edge Dimensions layer, all the measurements have been changed.

**Intersect Lines:**

1. Click Intersect Lines, and select the two edges you would like to intersect.
2. The two edges will be extended and intersect towards onto one vertex.

**Adjust Vertices:**

1. Open Adjust Vertices panel and click the vertex you would like to adjust.
2. The default triangulation is 2 images, you could change the location of the vertices on either two of the three images to adjust the vertex. The vertex location will be projected on the third image. Remember to Scroll the images to find the clearest one.
3. If you change the triangulation to 3 images, it is going to use all the three images to project the vertex location in the 3D view. And the vertex location can be seen on any other images if you Scroll the images.
4. Besides, if you Drag the vertex on 3D view, the projected location will be changed at the same time on 2D view.
5. After the adjustment, use the Apply button to implement your adjustment and the verified vertex is going to turn from Red to Green.

#Properties
**Properties \(Edge Classification\):**

1. After the rough wireframe, under the Detection tab of Properties, click Detect Edge Types to auto assign the edge type into all the edges.
2. To manually add the Property into the edges, go to the Properties tab, select the edge, click the Edge Type from the Add Property… dropdown menu. Then select the Edge Type whichever you want.
3. To change the Edge Type of the edge has already been assigned, go to the Properties tab, and select the Edge Type from the dropdown menu.

**Wireframe Registration:**

1. When the imported wireframe is not covered on the point cloud \(different coordinates\), this feature can be used to move and rotate the wireframe.
2. Create a new edges from the imported wireframe to the same point in the point cloud. Then Adjust the endpoint to make sure it is in the accurate location.
3. Repeat Step 2 based on different points, until there are 4 new edges.
4. Hold Ctrl to select all the 4 edges and click Register Wireframe.

**Generate Geojson:**

1. After Saving the wireframe, go back to Intranet and click Generate.
2. The qa-DXF and qa-GEOJSON will be generated.

