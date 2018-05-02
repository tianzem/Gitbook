### Save：

![](/icons/save.jpg)

Save the current wireframe into the working branch, generate a new sequential version number, and also save a wireframe.json under 
s3://pointivo-projects/ProjectID/out/WIREFRAME

### Save As：

![](/icons/saveas.jpg)

Save the current wireframe into the other branch if you change or type the Tag name, generate a new sequential version number, and also save a wireframe.json under 
s3://pointivo-projects/ProjectID/out/WIREFRAME

![](/Images/save_as.png)

Name: Typically empty but the content will be stored in the database.
Description: Typically empty but the content will be stored in the database.
Tag: The branch this wireframe going to be stored in.
Mark as Done?: Mark it when you finish the project. It will open the latest version of wireframe when the next time you open the project.

### Export：

![](/icons/export.jpg)

Export the current wireframe into local computer.

### Import：

![](/icons/import.jpg)

Import the previous exported wireframe.

### Undo：

![](/icons/undo.jpg)

Undo the last operation.
Notes: Some operation may not be undo properly, like [Attach]/[Detect Cutouts].

### Select：

![](/icons/select.jpg)

Under Select mode, you can rotate/pan the entire model. All the objects could be selected but could not be modified. 
This is the Read Only mode for demo.

### Create：

![](/icons/create.jpg)

Under Create mode, it will create a vertex in the location where you clicked. 

### Modify：

![](/icons/modify.jpg)

Under Select mode, you can rotate/pan the entire model. All the objects could be selected and modified if you hold the mouse and drag. 

### Delete：

![](/icons/delete.jpg)

Under Delete mode, it will delete the vertex you selected.
[Eraser] and [Erase All] are the other functions could help you delete multiply vertices.

### Align:

![](/icons/align.jpg)

1. \(Optional\) Under [Modify] and [Surface Mode], select a plane which you would like the edge to fix in and press `Space` to lock it.
2. Under [Modify] and [Vertex Mode], select \(or Hold `Ctrl` to multiply select the lines\) you want to align with.
3. Click [Align] or press `Shift` to change to [Align] mode, and click the Target edge.
4. The edges you selected on Step 2 will be aligned with the Target you selected on Step 3 and fixed in the plane you selected on Step 1.


{% em %}Video-Align!{% endem %}





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


