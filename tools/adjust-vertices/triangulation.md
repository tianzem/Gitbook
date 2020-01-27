---
description: >-
  There are 3 types of Triangulation in the 3D Tool: 1 Image + Locked Plane, 2
  Images, and 3 Images.
---

# Triangulation

![](../../.gitbook/assets/triangulation-01.png)

* **1 Image + Locked Plane:** Under this Triangulation, only 1 image is needed to adjust the vertex. When AutoLock is on, or a plane is manually locked, then this Triangulation will automatically turn on. The vertex will be fixed on the locked plane, and its location will be changed based on the selected 2D target. This mode ensures that a modified vertex will stay locked onto a reliable plane.
* **2 Images:** This is the default Triangulation of the tool. The vertices have to be adjusted in 2 of the three images, and will be projected onto the third image at the same time. Remember to shuffle through the images to find the best 2.
* **3 Images:** For this Triangulation, all three images are used to adjust the vertex and it requires more precision on the user's end. The user needs to shuffle through the images to make sure the same location of roof is shown in all 3 images. Then the vertex must be moved to the exact same spot in all 3 images. This mode is only used when the projection error is bad, or when the vertex will not adjust to the correct point in the cloud using 1 image or 2 image Triangulation.

**1 image + Locked Plane is the preferred Triangulation mode.**

{% hint style="warning" %}
When Auto Lock is on, 1 image + Locked Plane is automatically set for triangulation
{% endhint %}

