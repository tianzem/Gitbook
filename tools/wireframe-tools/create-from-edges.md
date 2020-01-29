# Create from Edges

Create from Edges is used to create planes that did not form automatically with [Auto Plane](../../advanced-function/auto-plane.md). Generally speaking, if a plane does not form on its own, then that's usually a sign that the plane is not planar. This can be due to crooked edges, or vertices pulling the plane in an unnatural direction. Before resorting to using Create from Edges, first check that all of the plane's edges and vertices are aligned along the same angle. Looking at the plane from its side view will point out any obvious vertices that are breaking the planarity. If the plane still doesn't form after fixing those visible issues, then Create from Edges must be used to form the plane.

{% hint style="warning" %}
Do NOT use Create from Edges until after the wireframe has been fully roughed and plane refined \(if necessary\). **Auto Plane will turn off** once Create from Edges is used. Anything added to the wireframe afterward will not form planes automatically.
{% endhint %}

{% hint style="info" %}
If Auto Plane is turned back on after using Create from Edges, then all planes that were manually created, using Create from Edges, will disappear. In order to open a project with a wireframe that has manually created planes: Open the qa branch, turn off Auto Plane, open the Version dropdown menu, click on the most recent Version of the project. This will reload the wireframe to include all of the manually created planes made by Create from Edges.
{% endhint %}

1. [Select](../../3d-scene-manipulation-tools/select.md), or hold `Ctrl` and click to multi-select, all of the edges that should have formed a plane but were not detected as a plane for some reason.

![](../../.gitbook/assets/createfromedges1.png)

2. Click Create from Edges, and the new plane will be created. [Auto Plane](../../advanced-function/auto-plane.md) will also turn off since it was on by default. This step should be performed at the end of creating a wireframe. Since Auto Plane will be turned off, any new planes created in the wireframe after this step will not be automatically detected.

![](../../.gitbook/assets/createfromedges2.png)

![](../../.gitbook/assets/create-from-edges.mp4)

![](../../.gitbook/assets/create-from-edges_proj18520_11_7_18.gif)

{% hint style="warning" %}
Keep in mind that this tool should only be used at the end of wireframe creation, because Auto Plane will be turned off. If Auto Plane is turned back on, after using Create from Edges, the new manually created planes will no longer be detected as planes and this process will have to be repeated.
{% endhint %}

