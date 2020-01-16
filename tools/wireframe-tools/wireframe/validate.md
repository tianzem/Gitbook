# Validate

This button is going to trigger an automatic validation to check the quality of the wireframe.

![](../../../.gitbook/assets/validate%20%281%29.png)

Clicking on each condition will select all of the objects with the error in the 3D tool and it will focus the camera view on all of the selected objects at once. Count displays the number of objects for each condition, and the arrows under Count will scroll through each object within the conditions.

Different Errors are as follow:

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
Coincident Vertices/Colinear Adjacent Edges can be ignored for certain specific cases.
{% endhint %}

{% hint style="info" %}
Refer to [Cutout Standard from Kespry](https://pointivo.gitbook.io/user-guide/weekly-updates/jun-29th-2018#cutout-standard-from-kespry) to get more information about Parent/Child Plane Shared Edges. 

For Kespry - Please take this validation as highest priority, and this scenario is illegal in any Kespry projects.  
For other customers - Ignore this validation
{% endhint %}



