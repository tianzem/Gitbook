# Lock Mode

![No hotkey available](../.gitbook/assets/lock-mode.png)

Lock Mode is an advanced setting that allows users to lock an edge, or plane, and then modify other vertices, edges or planes at a parallel location, and angle, to the locked edge or plane. This function is useful when dealing with sections of broken/noisy point clouds.

{% hint style="info" %}
Lock Mode is off, by default, every time a project is opened.
{% endhint %}

## Lock Mode - Edge

1. While in [Modify](../3d-scene-manipulation-tools/geometry/modify.md), with [Vertex Mode](../mode.md) on, select an edge for any vertices, or other edges, to lock onto. Press Spacebar to lock the edge. -- _The edge will turn blue to signify that it is locked_
2. While **Lock Mode is off:** 
   1. Click and drag any vertex, or a different edge, in the 3D tool.
   2. The vertex, or edge, snaps onto the locked edge. It can only be moved along the location of that locked edge. \(1st video\) 
3. Turn **Lock Mode on:** 
   1. Click and drag any vertex, or a different edge, in the 3D tool.
   2. The vertex, or edge, stays in its original location. It can only be moved at a parallel direction, and angle, to the locked edge. \(2nd video\)

In the video below, Lock Mode is off and the ridge edge is locked. When the selected vertex is moved, it automatically snaps to the locked edge and can only move along the direction of that locked edge.

![](../.gitbook/assets/lock-mode-off_edge-locked_proj12131_11_2018.gif)

In the video below, Lock mode is on and the ridge edge is locked. When the vertex of the eave edge is modified, it stays at its current location on the point cloud but moves in a parallel direction, and angle, of the locked ridge edge.

![](../.gitbook/assets/lockmodeon_edgelocked_proj12131.gif)

## Lock Mode - Plane

1. While in [Modify](../3d-scene-manipulation-tools/geometry/modify.md), with [Surface Mode](../mode.md) on, select a plane for any vertices, or edges, to lock onto and press Spacebar to lock the plane. -- _The plane will turn blue to signify that it is locked_
2. Switch to [Vertex mode](../mode.md).
   1. While **Lock Mode is off:** 
      1. Click and drag any vertex, or edge, in the 3D tool.
      2. The vertex, or edge, snaps onto the locked plane. It can only be moved along the location of that locked plane. \(1st video below\)
   2. Turn **Lock Mode on:** 
      1. Click and drag any vertex, or edge, in the 3D tool.
      2. The vertex, or edge stays, in its original location. It can only be moved at a parallel direction, and angle, to the locked plane. \(2nd video below\)

In the video below, **Lock Mode is off** and one of the planes is locked. When the selected vertex is moved, it automatically snaps to the locked plane and can only move along the direction of that locked plane.

![](../.gitbook/assets/lockmodeoff_planelocked_proj12131_11_2018.gif)

In the video below, **Lock mode is on** and a plane is locked. When the vertex is modified, it stays at its current location on the point cloud but moves in a parallel direction, and angle, of the locked plane.

![](../.gitbook/assets/lockmodeon_planelocked_proj12131_11_2018.gif)

On certain broken point clouds, there will be underhangs that are visible but may be too noisy to create an accurately sloped plane. If the underhang is supposed to be at the same slope as the plane above it, then Lock Mode will ensure that happens once the underhang plane is roughed. With Lock Mode on, and the upper plane locked, the roughed underhang plane can be modified. It will stay at the lower location and will be snapped at the same slope angle of the locked upper plane. The underhang plane can only be moved in a parallel direction to the locked upper plane.

