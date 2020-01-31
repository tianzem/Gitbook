# Trees

If a tree is too close to the roof, or if the tree's shadow falls across the roof, then the point cloud will most likely be broken there. This usually occurs at the corner of a structure.

1. [Create](../3d-scene-manipulation-tools/geometry/create.md) the two uncompleted edges near the corner.

   ![](../.gitbook/assets/2.jpg)

2. Use [Intersect Lines](../advanced-function/intersect-lines.md) to intersect the two edges to generate the corner point.
3. Turn on the [Edge Dimensions](../layers/edges.md) layer to double check the dimensions of the corner location.

