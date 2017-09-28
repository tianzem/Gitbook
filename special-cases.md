###Overhang:

>Typically, it is hard to find the image with the vertex under the overhang, but it might be easier to change the vertex in the 3D view.

1. Find three vertices on that plane and press `Space` to Lock the plane. If there are less than 3 vertices, [Create] more.

   ![](/Images/1.jpg)

2. Under [Modify], Drag the vertex in the 3D view. Since the plane has been locked, so all the movements are only allowed in that plane.
3. Turn on the [Adjust Vertices] panel to see the 2D view of the vertices to help you find the exact location of the vertices.

###Trees:

>Tree shadow will destroy a part of the point cloud, usually, it will be a corner.

1. [Create] the two uncompleted edges near the corner.

   ![](/Images/2.jpg)

2. Use [Intersect Lines] to intersect the two edges to generate the corner point.
3. Turn on the Edge Dimensions layer to double check the corner location.

###Chimney:

>Chimneys are on the edge of the roof. It is not hard to draw, but if you want to make the GeoJSON looks better, [Align] function is very useful, just align the flashing of the chimney with the nearby edges. 
 
![](/Images/3.jpg)

###Penetration:

>Penetrations are needed for solar projects.

1. Same as how to deal with the [Overhang]. Lock the plane - Drag the vertex in the 3D view - Check the vertices location in the 2D view.
2. Always turn on the Edge Dimensions layer and [Align] the relative edges to make sure the penetration is either a square or rectangle.

![](/Images/4.jpg)



[Save]: basic-function.md#save
[Save As]: basic-function.md#save-as
[Export]: basic-function.md#export
[Import]: basic-function.md#import
[Undo]: basic-function.md#undo
[Select]: basic-function.md#select
[Create]: basic-function.md#create
[Modify]: basic-function.md#modify
[Delete]: basic-function.md#delete
[Align]: basic-function.md#align
[Set Scale]: advanced-function.md#set-scale
[Eraser]: advanced-function.md#eraser
[Erase All]: advanced-function.md#erase-all
[Intersect Lines]: advanced-function.md#intersect-lines
[Register Wireframe]: advanced-function.md#register-wireframe
[Properties]: basic-function.md#properties
[Layers]: basic-function.md#layers
[Adjust Vertices]: basic-function.md#adjust-vertices
[Vertex Mode]: mode.md#vertex-mode
[Edge Mode]: mode.md#edge-mode
[Surface Mode]: mode.md#surface-mode
[Special Cases]: special-cases.md
[Overhang]: special-cases.md#overhang
[Tree]: special-cases.md#tree
[Chimney]: special-cases.md#chimney
[Penetration]: special-cases.md#penetration
[Flat Roof]: special-cases.md#flat-roof
[Steps to QA a Project]: steps-to-qa-a-project.md
[Edge Types and Example]: edge-types-and-example.md
[Shortcut]: shortcut.md



