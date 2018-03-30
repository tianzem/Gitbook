###Camera:

You should be able to view all the camera location by clicking the camera icon besides each image.

![](/icons/camera.jpg)

All the camera locations will be viewable above the 3D model in the Camera layer and if you select the red camera, the relative camera view will be updated in the 2D view.

![](/Images/camera project.jpg)

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

>Penetrations are needed for Tesla projects, and you will see "label obstructions" in the description field of the projects.


1. Finish the entire roof first and get ready for the penetrations.
2. Start from one of the planes, open the 2D images first to count the total numbers of the penetrations to make sure you won't miss any penetrations in this plane. Lock this plane, go to [Vertex Mode] and draw a small square which covers the penetration.

   ![](/Images/penetration1.jpg)

3. Change to [Surface Mode] and hold `Ctrl` to multiply select all the squares in this plane and [Attach] all the penetrations onto the big plane. You will see the penetrations turn to blue and all the operations related to the penetration are fixed in the plane.

   ![](/Images/penetration2.jpg)

4. Then same as how to deal with the [Overhang]. Lock the plane first, then you could either open the [Adjust Vertices] and adjust every corner one by one, or drag the vertex in the 3D view and check the vertices location in the 2D view at the same time, until all the vertices in this plane are adjusted.

5. Turn on the Edge Dimensions layer and [Align] the relative edges to make sure the penetration is either a square or rectangle.

6. Open the [Adjust Vertices] and check every plane one by one in the 2D images to make sure there is not any missing penetrations.(Any obstruction which will affect the setup of solar panel should be treated as penetration) 

   ![](/Images/penetration3.jpg)
   
7. If the roof plane is changed or deleted, you may need to redo the penetrations since it is going to be detached or moved with the plane.

   ![](/Images/penetration3.jpg)

###Flat Roof:

>Typically, it is hard to select the corner of the flat roof because of the texture and the parapet.

   ![](/Images/flat roof corner.jpg)

1. Outline the flat roof as close as the actual corner, do not need to perfect it on the corner but need to make sure the plane is correct.

   ![](/Images/flat roof.jpg)

2. [Select] and lock the flat plane and then open [Adjust Vertices] to change Triangulation to 1 Image + Locked Plane.
3. Scroll all the viewable images to find the best one and only use that image to adjust the vertex into the correct location.
4. Repeat Step 3 to adjust every vertices.

###Dormers:





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
[Lock Mode]: advanced-function.md#lock-mode
[Auto Plane]: advanced-function.md#auto-plane
[Set Scale]: advanced-function.md#set-scale
[Eraser]: advanced-function.md#eraser
[Erase All]: advanced-function.md#erase-all
[Intersect Lines]: advanced-function.md#intersect-lines
[Register Wireframe]: advanced-function.md#register-wireframe
[Properties]: advanced-function.md#properties
[Layers]: advanced-function.md#layers
[Adjust Vertices]: advanced-function.md#adjust-vertices
[Attach]: tools.md#attach
[Detach]: tools.md#detach
[Create from Edges]: tools.md#create-from-edges
[Delete]: tools.md#delete
[Detect Edge Types]: tools.md#detect-edge-types
[Detect Cutouts]: tools.md#detect-cutouts
[Finalize]: tools.md#finalize
[ML Refine]: tools.md#ml-refine
[Validate]: tools.md#validate
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
















