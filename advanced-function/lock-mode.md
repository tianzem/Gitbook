---
description: >-
  Lock Mode is an advanced setting that allows the user to lock a specific edge,
  or plane, then edit/create any vertices, edges, or planes in a location that
  is parallel to the locked edge or surface.
---

# Lock Mode

![](../.gitbook/assets/lock-mode.png)

Lock Mode is an advanced setting that allows users to lock an edge, or plane, and then edit/create an vertices, edges, or planes in a location that is parallel to the locked edge or plane. This function is useful when dealing with broken/noisy point clouds. 

On certain broken clouds there will be underhangs that are visible, but may be too noisy to create an accurately sloped plane. If the underhang is supposed to be at the same slope as the plane above it, then Lock Mode will ensure that happens. With Lock Mode engaged, and the upper plane locked, the underhang plane can be created at the lower location while and stay locked to the slope of the upper plane. See example videos below.

## Lock Mode - Edge

1. Under [Modify](../basic-function/geometry/modify.md) and [Vertex Mode](../mode.md), select an edge for the vertices to lock onto and press `Space` to lock the edge.
2. Under [Modify](../basic-function/geometry/modify.md) and [Vertex Mode](../mode.md), Click and Drag a vertex in the 3D tool. 
3. When Lock Mode is off \(default\), the vertex can be only moved on the locked edge.
4. When Lock Mode is on, the vertex can be only moved in a parallel direction to the locked edge.

![](../.gitbook/assets/lock-mode-off_edge-locked_proj12131_11_2018.gif)

In the video above, Lock Mode is off \(default\) and one of the edges is locked. The selected vertex snaps to the locked edge when the user modifies it. The vertex can only move in the direction of the locked edge.

![](../.gitbook/assets/lockmodeon_edgelocked_proj12131.gif)

In the above video, Lock Mode is on and one of the edges is locked. When the vertex is modified it moves in the parallel direction of the locked edge. The vertex can be placed anywhere on the point cloud but once an edge is locked, and Lock Mode is turned on, the vertex will only move in a parallel direction to the locked edge.

## Lock Mode - Surface

1. Under [Modify](../basic-function/geometry/modify.md) and [Surface Mode](../mode.md), select a plane to lock a vertex onto and press `Space` to lock the plane.
2. Under [Modify](../basic-function/geometry/modify.md) and [Vertex Mode](../mode.md), Hold and Drag the vertex in the 3D tool. 
3. When Lock Mode is off \(default\). The vertex can be only moved on the locked plane.
4. When Lock Mode is on. The vertex can be only moved in a parallel/co-planar direction to the locked plane.

![](../.gitbook/assets/lockmodeoff_planelocked_proj12131_11_2018.gif)

In the video above, Lock Mode is off \(default\) and one of the planes is locked. The selected vertex snaps to the locked plane when you modify it. The vertex can only be moved in the direction of the locked plane.

![](../.gitbook/assets/lockmodeon_planelocked_proj12131_11_2018.gif)

In the above video, Lock Mode is on and one of the planes is locked. When you the vertex is modified it moves in the parallel direction of the locked plane. Users can put the vertex anywhere on the point cloud but once a plane is locked, and Lock Mode is turned on, the vertex will only move in a parallel/co-planar direction to the locked plane.

