# Trees

If a tree is too close to the roof, or if the tree's shadow falls across the roof, then the point cloud will probably be broken in that area. This usually occurs at the corner of a structure. There are a couple of options for users to try when wireframing these tree scenarios. The first option is to complete the plane as much as possible, and then add the missing vertices/edges. This is shown in the video below. The second method is to use [Intersect Lines](../advanced-function/intersect-lines.md), as described in the three steps after the video.

**Option 1** -- Form the plane as much as possible:

{% embed url="https://drive.google.com/file/d/1aqEpk\_hU\_BZ1cVnU9IHtdzbgDpsDL8Vd/view?usp=sharing" %}

In the video above, the plane is created using 2 existing vertices and then adding a third vertex to a section of the point cloud that isn't broken in the new plane. Manually lock this new, smaller plane and add extra vertices to account for those that are missing from the plane. Use the 2D images, in the Tools panel, as a guideline to adjust the vertices to their estimated correct location. Turn on the edge dimensions to check if the broken area is relatively symmetrical with its counterpart.

{% hint style="warning" %}
Option 1 is the recommended way to deal with sections of broken point cloud in the wireframe.
{% endhint %}

**Option 2** -- Intersect Lines:

1. [Create](../3d-scene-manipulation-tools/geometry/create.md) the two uncompleted edges near the corner.

   ![](../.gitbook/assets/2.jpg)

2. Use [Intersect Lines](../advanced-function/intersect-lines.md) to intersect the two edges to generate the corner point.
3. Open up the Tools panel, and use the 2D images to adjust the new vertex as far as it can be seen in the images.

{% hint style="info" %}
Be cautious when using Intersect Lines. It is an estimate and won't always produce the expected results. 
{% endhint %}

