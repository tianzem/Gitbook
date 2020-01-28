# Validate

The Validate button will evaluate the current view of the wireframe and list all of the conditions \(issues\) found within it. When the project is saved, Validate is automatically triggered. However, the project can be validated without saving too. 

Using the Validate button, in either the Wireframe Tools panel or the Project Validations panel, is a quick way to check for errors without saving the project. 

![](../../../.gitbook/assets/validate%20%281%29.png)

Clicking on each condition's name will select all of the objects with that error in the 3D window. Every item with that condition will be selected on the point cloud. and it will focus the camera view on all of the selected objects at once. 

Count displays the number of objects for each listed condition. To the right of the condition name, the count number is shown with white arrows on each side. When an arrow is clicked, the 3D view will rotate and highlight one object at a time.

#### List of Conditions:

| **Condition** | **Intro** |
| :--- | :--- |
| Isolated Vertex | Vertex is not attached to any edges |
| Isolated Edge | Edge does not belong to any plane |
| Coincident Vertices | Two vertices are too close to one another |
| Colinear Adjacent Edges | Extra vertex in the middle of an edge |
| Missing EdgeTypeProperty | Edge does not have an Edge Type assigned |
| Inconsistent Plane Normals | The Plane Normals do not point in the same direction |
| Parent/Child Plane Shared Edges | The edge of a cutout is shared with its parent plane |

{% hint style="info" %}
Inconsistent Plane Normals can be ignored.
{% endhint %}

{% hint style="info" %}
Coincident Vertices/Colinear Adjacent Edges can be ignored for certain cases -- i.e. For chimneys that barely enter the edge of a plane, the vertices outlining the chimney will be shown as "Coincident Vertices". For structures with curved edges, the multiple vertices used to curve the edge will trigger the condition "Colinear Adjacent Edges". Those are ok to ignore.
{% endhint %}

\*Fix the warning below this. The "cutout standard from kespry" links to a page in the weekly updates section. Add a section here for: Instructions on how to handle Parent/Child Plane Shared Edges and example images

{% hint style="info" %}
Refer to [Cutout Standard from Kespry](https://pointivo.gitbook.io/user-guide/weekly-updates/jun-29th-2018#cutout-standard-from-kespry) to get more information about Parent/Child Plane Shared Edges. 

For Kespry - Please take this validation as highest priority, and this scenario is illegal in any Kespry projects.  
For other customers - Ignore this validation
{% endhint %}



