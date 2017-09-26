# Pointivo Cheat Sheet {#pointivo-cheat-sheet}

**Common Edge Types**

|  | Number of Planes | Angle | Parallel to Ground |
| --- | --- | --- | --- |
| Eave | 1 |  | √ |
| Rake | 1 |  | × |
| Hip | 2 | "Λ" | × |
| Valley | 2 | "V" | × |
| Ridge | 2 |  | √ |
|  |  | Flashing | Only around the Chimney |
|  |  | Step Flashing | Only connects towards the Wall |

**Shortcuts**

| **Shortcut** | **Operation** |
| --- | --- |
| Ctrl + Scroll Mouse | Change the size of Vertices and the Width of the Line |
| Ctrl + Shift + Scroll Mouse | Change the size of Dimensions |
| 1 | Vertex Mode |
| 2 | Surface Mode |
| Alt | Create Mode |
| Shift | Align Mode |
| Ctrl | Multiple Selection |
| Alt + Shift | Delete Mode |
| Space | Lock Surface |
| Ctrl + Z | Undo |
| Ctrl + S | Not working, Shortcut Conflict |



**Edge Type Example - QA Project: 6573**

![](/edge_classification.jpeg)

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

**Steps to QA a Real Project**

1. Pick up the project from intranet, click View to open the 3DTool. Click the dropdown menu of Tag to make sure there is not any QA branch.
2. Save a new QA branch and tell everyone on Slack you are going to pick this project, in case of any duplicate work.
3. Delete the redundant vertices and Add the missing vertices to draw the rough wireframe. Remember to draw all the Penetration if it is a DroneDeploy project.
4. Adjust each vertex to finish the Ground Truth wireframe.
5. Open the Properties panel and click the Detect Edge Types to detect all the edge types.
6. Manually check all the edge types one by one and refer to this cheat sheet Common Edge Types to correct the wrong edge type.
7. Save As the project and Mark As Done.
8. Go back to Intranet and click Generate to have the GeoJSON output. Click qa-GEOJSON and View button, then open the Mapbox Studio to check the wireframe layout.
9. When there are missing edges/unusual edges/redundant areas etc, go back to 3DTool to check the relevant vertices. Make sure the vertices should be on a plane are in a plane and there are not any missing edges. Save the Project, Generate the GEOJSON and check the Mapbox Studio again.
10. If the issue is not fixed, then check Kibana logs to see the possible causes. Click Settings to change the parameter threshold in Project Settings.
11. If the point cloud is broken, mark the POINT\_DENSE as PROBLEM, if the point cloud is too bad to draw the wireframe, mark the POINT\_DENSE as UNUSABLE.
12. For Kespry projects, Publish the DXF and GEOJSON.

For DroneDeploy projects, Publish the DXF.

1. After click Publish, mark the final project as COMPLETE\_FINAL.



