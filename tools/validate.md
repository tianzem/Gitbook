# Validate

This button is going to trigger an automatic validation to check the quality of the wireframe.

![](../.gitbook/assets/validate.png)

Clicking on each condition will select all of the objects with the error and will focus the camera view all of the selected objects at once. Count tells you the number of objects for each condition, and the arrows under Count allow you to scroll through each object within the conditions.

Different Errors are as follow:

| **Condition** | **Intro** |
| --- | --- |
| Isolated Vertex | Vertex is not attached to any edges |
| Isolated Edge | Edge does not belong to any plane |
| Coincident Vertices | Two vertices are too close to one another |
| Colinear Adjacent Edges | Extra vertex in the middle of an edge |
| Missing EdgeTypeProperty | Edge does not have an Edge Type assigned |
| Inconsistent Plane Normals | The Plane Normals do not point in the same direction |

{% hint style="info" %}
Inconsistent Plane Normals can be ignored.
{% endhint %}

{% hint style="info" %}
Coincident Vertices/Colinear Adjacent Edges can be ignored for certain specific cases.
{% endhint %}

