---
description: >-
  Lock Mode is an advanced setting that allows the user to lock a specific edge,
  or plane, then edit/create any vertices, edges, or planes in a location that
  is parallel to the locked edge or surface.
---

# Lock Mode

![No hotkey available](../.gitbook/assets/lock-mode.png)

Lock Mode is an advanced setting that allows users to lock an edge, or plane, and then modify other vertices, edges, or planes in a location that is parallel to the locked edge or plane. This function is useful when dealing with broken/noisy point clouds. Lock Mode is off, by default, when a project is opened.

On certain broken point clouds, there will be underhangs that are visible but may be too noisy to create an accurately sloped plane. If the underhang is supposed to be at the same slope as the plane above it, then Lock Mode will ensure that happens. With Lock Mode engaged, and the upper plane locked, the underhang plane can be created at the lower location and it will have the same slope as the locked upper plane. See example videos below.

## Lock Mode - Edge

1. While in [Modify](../3d-scene-manipulation-tools/geometry/modify.md), with [Vertex Mode](../mode.md) on, select an edge for the vertices to lock onto and press Spacebar to lock the edge.
2. Click and drag any vertex in the 3D tool. 
3. When Lock Mode is off, the vertex can be only moved on the locked edge. \(1st video\)
4. When Lock Mode is on, the vertex can be only moved in a parallel direction and angle to the locked edge. \(2nd video\)

In the video below, Lock Mode is off and the ridge edge is locked. When the selected vertex is moved, it automatically snaps to the locked edge and can only move along the direction of that locked edge.

![](../.gitbook/assets/lock-mode-off_edge-locked_proj12131_11_2018.gif)

In the video below, Lock mode is on and the ridge edge is locked. When the vertex of the eave edge is modified, it stays at its current location on the point cloud but moves in parallel with the direction, and angle, of the locked ridge edge.

![](../.gitbook/assets/lockmodeon_edgelocked_proj12131.gif)

## Lock Mode - Surface

1. While in [Modify](../3d-scene-manipulation-tools/geometry/modify.md), with [Surface Mode](../mode.md) on, select an edge for the vertices to lock onto and press Spacebar to lock the edge.
2. Click and drag any vertex in the 3D tool. 
3. When Lock Mode is off, the vertex can be only moved on the locked plane. \(1st video below\)
4. When Lock Mode is on, the vertex can only be moved in a parallel/co-planar direction to the locked plane. \(2nd video below\)

![](../.gitbook/assets/lockmodeoff_planelocked_proj12131_11_2018.gif)

In the video above, Lock Mode is off and one of the planes is locked. The selected vertex snaps to the locked plane when you modify it. The vertex can only be moved in the direction of the locked plane.

![](../.gitbook/assets/lockmodeon_planelocked_proj12131_11_2018.gif)

In the above video, Lock Mode is on and one of the planes is locked. When you the vertex is modified it moves in the parallel direction of the locked plane. Users can put the vertex anywhere on the point cloud but once a plane is locked, and Lock Mode is turned on, the vertex will only move in a parallel/co-planar direction to the locked plane.

