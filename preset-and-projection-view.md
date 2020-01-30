---
description: No hotkeys available.
---

# Preset & Projection View

The Preset & Projection View buttons allow users to control the 3D Tool's dimension view and camera type settings.

![](.gitbook/assets/3d-2d-camera-and-ortho-buttons_large.png)

The 3D Preset button is the default preset of the 3D Tool window. Clicking it will set the projection view to Perspective \(camera symbol button\), which is also the default projection view.

The 2D Preset button will switch the preset to 2D in the 3D window, and it will change the projection view to Orthographic. It will lock the point cloud to the true north direction on the grid of the [View Cube](view-cube.md), and the point cloud will be rotated and re-centered to match that direction. The projected view buttons will automatically switch to the Orthographic projection view instead of the Perspective projection view.

{% hint style="info" %}
The 2D Preset button is helpful when wireframing commercial structures. Switching to 2D mode allows users to see an overview of the wireframe's alignment and ensure its vertices aren't going through the walls of the point cloud.
{% endhint %}

The Re-center Button will quickly re-center the point cloud within the 3D Tool window, and will rotate the cloud back to its original angle.

{% hint style="info" %}
The Re-center button is very useful when the point cloud gets zoomed in/out too far, or when the 3D window is panned away from the cloud. It will bring the point cloud back into focus.
{% endhint %}

The Perspective Projection View button \(camera\) is the default projection view for the 3D Tool. When switching from 2D preset to 3D preset, the Perspective projection button will automatically activate as well. This is the view required to fully operate the 3D Tool.

The Orthographic Projection View button \(grid\) is the required projection view for the 2D Preset. Clicking the Orthographic Projection button will re-orient the point cloud to the true north direction in the orthographic view. However, unlike the 2D Preset button clicking the Orthographic Projection button does not lock the view cube to the true north 2D direction. You are still able to rotate the point cloud like normal, but the cloud is now set as an orthographic map.

