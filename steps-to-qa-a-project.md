**Steps to QA a Real Project**

1. Pick up the project from intranet, click View to open the 3DTool. Click the dropdown menu of Tag to make sure there is not any QA branch.
   ![](/Images/5.jpg)

2. Save a new QA branch and tell everyone on Slack you are going to pick this project, in case of any duplicate work.
3. Delete the redundant vertices and Add the missing vertices to draw the rough wireframe. Remember to draw all the Penetration if it is a DroneDeploy project.
4. Adjust each vertex to finish the Ground Truth wireframe.
5. Open the Properties panel and click the Detect Edge Types to detect all the edge types.
   ![](/Images/6.jpg)

6. Manually check all the edge types one by one and refer to this cheat sheet Common Edge Types to correct the wrong edge type.
7. Save As the project and Mark As Done.
8. Go back to Intranet and click Generate to have the GeoJSON output. Click qa-GEOJSON and View button, then open the Mapbox Studio to check the wireframe layout.
9. When there are missing edges/unusual edges/redundant areas etc, go back to 3DTool to check the relevant vertices. Make sure the vertices should be on a plane are in a plane and there are not any missing edges. Save the Project, Generate the GEOJSON and check the Mapbox Studio again.
10. If the issue is not fixed, then check Kibana logs to see the possible causes. Click Settings to change the parameter threshold in Project Settings.
    ![](/Images/7.jpg)

11. If the point cloud is broken, mark the POINT\_DENSE as PROBLEM, if the point cloud is too bad to draw the wireframe, mark the POINT\_DENSE as UNUSABLE.
    ![](/Images/8.jpg)

12. For Kespry projects, Publish the DXF and GEOJSON. For DroneDeploy projects, Publish the DXF.

13. After click Publish, mark the final project as COMPLETE\_FINAL.



