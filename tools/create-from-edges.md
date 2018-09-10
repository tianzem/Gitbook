# Create from Edges

[Select](../basic-function/#select), or hold `Ctrl` and click to multi-select, all of the edges that should have formed a plane but were not detected as a plane for some reason.

![](../.gitbook/assets/createfromedges1.png)

Click Create from Edges, and the new plane will be created. [Auto Plane](../advanced-function/#auto-plane) will also turn off since it was on by default. This step should be performed at the end of creating a wireframe. Since Auto Plane will be turned off, any new planes created in the wireframe after this step will not be automatically detected.

![](../.gitbook/assets/createfromedges2.png)

![](../.gitbook/assets/create-from-edges.mp4)

![](../.gitbook/assets/create-from-edges-1.gif)

{% hint style="warning" %}
Keep in mind that this tool should only be used at the end of wireframe creation, because Auto Plane will be turned off. If you turn Auto Plane back on, after using Create from Edges, your new manually created planes will no longer be detected as planes.
{% endhint %}

