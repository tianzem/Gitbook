---
description: No hotkey available.
---

# Register Wireframe

When an imported wireframe does not automatically snap to the point cloud \(due to differing coordinates\), the Register Wireframe feature can be used to automatically move, rotate, and snap the wireframe onto the point cloud.

![](../../.gitbook/assets/register.png)

1. Import the original wireframe into the new project. SAVE the new project!
   * If the wireframe imports in at a far distance from the point cloud:
     * Hit Ctrl + A to select all of the edges, vertices, and planes in the imported wireframe.
     * Change the Snap mode to None.
     * Click and hold one of the edges, vertices, or planes and drag it closer to the point cloud.
2. Create a new edge from one of the vertices on the imported wireframe, and connect it to the same location it should be on in this new point cloud. 
3. Then use [Adjust Vertices](../adjust-vertices/), with [3image triangulation](../adjust-vertices/triangulation.md), to adjust the endpoint on the cloud and ensure it is in the accurate location.
4. Repeat Steps 1 & 2 for each different vertex, until there are at least 4 new edges.
   * There can be more than 4 vertices/edges created.
   * Try to place these new vertices on multiple levels of the point cloud.
     * Connecting them on differing plane levels, will yield better results in the registration.
5. Hold Ctrl and left-click each newly created edge until all new edges are selected.
6. Click the Register Wireframe button, and the wireframe will snap down to the point cloud. \(see warning message below video\)

![](../../.gitbook/assets/register.jpg)

![](../../.gitbook/assets/wireframe-register.gif)

{% hint style="warning" %}
The vertices of the wireframe being registered will already be verified from the original project it was exported from. The vertices will still need to be checked after clicking Register Wireframe to re-verify that they are in the correct location. Adjust Vertices may need to be used to tweak some of the vertex locations to make them more accurate. This is why it is important to ensure that the endpoint vertex location is accurate before clicking Register Wireframe.
{% endhint %}

