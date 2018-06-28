# Basic Function

## Save：

![](../.gitbook/assets/save.jpg)

Save the current wireframe into the working branch, generate a new sequential version number, and also save a wireframe.json under s3://pointivo-projects/ProjectID/out/WIREFRAME

## Save As：

![](../.gitbook/assets/saveas.jpg)

Save the current wireframe into the other branch if you change or type the Tag name, generate a new sequential version number, and also save a wireframe.json under s3://pointivo-projects/ProjectID/out/WIREFRAME

![](../.gitbook/assets/save_as.png)

Name: Typically empty but the content will be stored in the database. Description: Typically empty but the content will be stored in the database. Tag: The branch this wireframe going to be stored in. Mark as Done?: Mark it when you finish the project. It will open the latest version of wireframe when the next time you open the project.

## Export：

![](../.gitbook/assets/export.jpg)

Export the current wireframe into local computer.

## Import：

![](../.gitbook/assets/import.jpg)

Import the previous exported wireframe.

## Undo：

![](../.gitbook/assets/undo.jpg)

Undo the last operation. Notes: Some operation may not be undo properly, like [Attach](../tools/#attach)/[Detect Cutouts](../tools/#detect-cutouts).

## Select：

![](../.gitbook/assets/select.jpg)

Under Select mode, you can rotate/pan the entire model. All the objects could be selected but could not be modified. This is the Read Only mode for demo.

## Create：

![](../.gitbook/assets/create.jpg)

Under Create mode, it will create a vertex in the location where you clicked.

## Modify：

![](../.gitbook/assets/modify.jpg)

Under Select mode, you can rotate/pan the entire model. All the objects could be selected and modified if you hold the mouse and drag.

## Delete：

![](../.gitbook/assets/delete.jpg)

Under Delete mode, it will delete the vertex you selected. [Eraser](../advanced-function/#eraser) and [Erase All](../advanced-function/#erase-all) are the other functions could help you delete multiply vertices.

## Align:

![](../.gitbook/assets/align.jpg)

1. \(Optional\) Under [Modify](./#modify) and [Surface Mode](../mode/#surface-mode), select a plane which you would like the edge to fix in and press `Space` to lock it.
2. Under [Modify](./#modify) and [Vertex Mode](../mode/#vertex-mode), select \(or Hold `Ctrl` to multiply select the lines\) you want to align with.
3. Click [Align](./#align) or press `Shift` to change to [Align](./#align) mode, and click the Target edge.
4. The edges you selected on Step 2 will be aligned with the Target you selected on Step 3 and fixed in the plane you selected on Step 1.

![](https://pointivo-drop.s3.amazonaws.com/CheatSheet/align.gif)

