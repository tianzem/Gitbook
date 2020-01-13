# Snap Mode

![](../.gitbook/assets/snap.png)

Snap mode affects vertex, edge, and plane manipulation in the 3D window. For vertices, all 3 snap modes affects vertex manipulation. For edges and surfaces, only Locked Geometry affects the edge and/or surface manipulation. If Locked Geometry is off, leaving either None or Point Cloud snap on, then the surfaces and edges can be moved in any direction without being snapped to the cloud.

## None:

None mode is the only snap mode that allows full control over vertex movement. Newly created vertices will still be placed on the cloud, wherever they are clicked, but they will not stay snapped to the cloud when moved in the 3D window. None snap mode allows the user to manipulate a vertex, in all directions, without concern for the point cloud. This mode is useful when a vertex needs to be moved to a spot on the cloud that is covered in noise, or is broken. With None snap on, the vertex can be manually pulled to any spot in the 3D window.

## Point Cloud:

Point Cloud is the default snap mode for the 3D tool. It is the snap mode used when creating a new wireframe. Any vertex that is created, or selected, will be dropped onto the nearest point in the point cloud. Users will not be able to place a vertex in the black area of the viewport, where there is no point cloud. All vertex movements will be snapped to the cloud. This snap mode only affects vertices. Planes and edges are not affected by Point Cloud snap mode.

## Locked Geometry:

This mode is only active, and automatically activated, when a plane or edge is locked. All movements will be fixed on the locked plane/edge, or on the co-planar of the locked plane/edge. If a horizontal edge is locked, and a perpendicular edge is moved, then the perpendicular edge will automatically snap horizontally onto the original horizontal edge.

{% hint style="warning" %}
Locked Geometry is the most important snap mode when adjusting the vertices of a wireframe. Locked Geometry allows the users to manipulate the vertices, edges, and planes while still being locked to the desired edge or plane. When adjusting vertices, Locked Geometry helps keep the plane intact by forcing any wireframe movements to be locked onto that plane. Without Locked Geometry on, the plane would break once one of its vertices snaps to part of the cloud outside of the plane's boundaries.
{% endhint %}

