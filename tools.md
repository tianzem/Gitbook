### Attach:
1. Under [Surface Mode], [Select] or hold `Ctrl` to multi select the upper surfaces you want to attach.

 ![](/Images/attach1.png)

2. With all the surfaces selected, click Attach and then click the lower surface which you would like the surfaces to attach to.
3. All the upper surfaces will be flat and attached to the lower surface. The attached surfaces will turn to blue.

 ![](/Images/attach2.png)

### Detach:

[Select] all the surfaces which have been attached and click Detach.

### Create from Edges:
1. [Select] or hold `Ctrl` to multi select all the edges which should be on the same plane but not detected for any reasons.

 ![](/Images/createfromedges1.png)

2. Click Create from Edges, then the new plane will be created. And it will also turn off the Auto Plane which is on by default.

 ![](/Images/createfromedges2.png)

### Delete:

1. Under [Surface Mode], [Select] or hold `Ctrl` to multi select the planes you want to delete.
2. Click Delete, then the selected planes will be deleted. And it will also turn off the Auto Plane which is on by default.


### Detect Edge Types:

It will add a new Property "Edge Type" into each edge and assign the detected edge type to this property.

Note: It is not going to overwrite any assigned edge type property. To redetect all the edge types, you need to select all the edges and delete all the edge types first.

### Detect Cutouts:

It is going to detect all the cutouts in the scene and attach the cutouts plane into the lower plane.

### Finalize:

Finalize is going to Detect Cutouts and Detect Edge Types

### ML Refine:

Machine learning is going to tweak the location of each vertices. It will save the current the current wireframe as a Rough wireframe in the current branch. And once it is done, it will save the refined wireframe as a new Wireframe-3-Java version under Autogen branch.

### Validate:

This button is going to trigger an automatic validation to check the quality of the wireframe. 
 ![](/Images/validate.png)
Clicking the each condition will select all the objects with the error and focus the camera into all these objects at the same time. The arrows under Count could scroll all the objects.

Different Errors are as follows:

| **Condition** | **Intro** |
| --- | --- |
| Isolated Vertex | Vertex does not belong to any edges|
| Isolated Edge| Edge does not belong to any plane|
| Coincident Vertices | Two vertices are too close with each other|
| Colinear Adjacent Edges | Extra vertex in the middle of the edge |
| Missing EdgeTypeProperty | Edge does not have edge type |


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






