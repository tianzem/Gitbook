**Steps to QA a Real Project**

1. Pick up the project from intranet, click View to open the 3DTool. Click the dropdown menu of Tag to make sure there is not any QA branch.  

   ![](/Images/5.jpg)

2. Save a new QA branch and tell everyone on Slack you are going to pick this project, in case of any duplicate work.

3. Check all the Autogen versions and find out the best one. [Delete] the redundant vertices and [Eraser] the missing vertices to draw the rough wireframe. Remember to draw all the [Penetration] if it is a DroneDeploy project.

4. [Adjust Vertices] to finish the Ground Truth wireframe.

5. Open the Tools panel and click [Detect Edge Types] to detect all the edge types.  

   ![](/Images/tools.png)

6. Manually check all the edge types one by one and refer to [Edge Types and Example] to correct the wrong edge type.

7. [Save As] the project and Mark As Done.

8. Go back to Intranet and click Generate to have the different outputs. 

   ![](/Images/generate resources.jpg)
   
   Branches: Select the branch you would like to generate the output. Typically, it should be qa.
   Resource Types:
      `GEOJSON: The main output file which needs to be checked on Mapbox.`
      `DXF: DXF file.`
      `ORTHO: Ortho image with the wireframe.`
      `ORTHO_REPORT:`
      `DATA_PACKAGE: All the output data including the pictures and JSON file.`

9. Click the View button besides qa-GEOJSON, then open the Mapbox Studio to check the wireframe layout

10. When there are missing edges/unusual edges/redundant areas etc, go back to 3DTool to check the relevant vertices. Make sure the vertices should be on a plane are in a plane and there are not any missing edges. [Save] the Project, Generate the GEOJSON and check the Mapbox Studio again.

11. If the issue is not fixed, then check Kibana logs to see the possible causes. Click Settings to change the parameter threshold in Project Settings.  

    ![](/Images/7.jpg)

12. If the point cloud is broken, mark the POINT\_DENSE as PROBLEM, if the point cloud is too bad to draw the wireframe, mark the POINT\_DENSE as UNUSABLE.  

    ![](/Images/8.jpg)

13. For Kespry projects, Publish the DXF and the GEOJSON. 
    For DroneDeploy projects, Publish the DXF, the GEOJSON and the DataPackage.
    For PrecisionHawk projects, Publish the DXF, the GEOJSON and the DataPackage.
    
    ![](/Images/resources.jpg)

14. After click Publish, mark the final project as COMPLETE\_FINAL.
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



















