# How to Deal with a Broken Point Cloud

Kespry is doing testing flights on site by the pilot sometimes, and they are not expecting any results from this kind of testing projects. There is no need to put these broken point cloud to `IN_REVIEW` or `IN_SUPPORT`, since they could be done easily.

**Case 1:** Ground/Dirt/Grass/Rubble without any structures.

**Example:** `12243, 21658, 147800`

**Solution:** Typically, the autogen is empty since no structures are detected. So please draw a rectangle on the ground and publish. If there are outlier vertices on trees or neighboring structures, then delete all of those and then draw the rectangle on the ground. There is no need to worry about the edge types or verify the vertices since they do not make any sense.

![12243](../.gitbook/assets/12243-ug.gif)

![21658](../.gitbook/assets/burned-structure-example.png)

![147800](../.gitbook/assets/image%20%2829%29.png)

**Case 2:** Most of the roofing is not captured.

**Example:** `12198, 11872, 58972`

**Solution:** Typically, there will be an autogen branch, although the autogen wireframe might be broken or messy. Save the autogen wireframe to the qa branch and publish that. If there isn't an autogen wireframe, then put a rough wireframe around the structure. Again, there is no need to verify vertices or worry about the edge types since they do not make any sense.

![12198](../.gitbook/assets/11872-ug.gif)

![11872](../.gitbook/assets/12198-ug.gif)

![58972 - This would also get marked as Defective Reconstruction &amp; Smoothed Point Cloud](../.gitbook/assets/broken-unusable-smoothed-cloud_58972.PNG)

**Case 3:** Part of the roofing is not captured and broken in the point cloud.

**Example:** `140843`

**Solution:** Take it as a regular project, but ignore the incomplete/broken planes. Detect edge types, and verify vertices, like normal. However, do not waste your time verifying the vertices where the point cloud is broken. Instead, put a rough wireframe on it and then ignore during verification.

![140843](../.gitbook/assets/image%20%2831%29.png)

{% hint style="danger" %}
Always remember to check the _**Broken Point Cloud**_ before you publish the project.
{% endhint %}

![](../.gitbook/assets/project-issues-broken-cloud.gif)

For **Case 1 and Case 2** where there are not any completed planes, change the `POINT_DENSE` to `UNUSABLE`.

![](../.gitbook/assets/image%20%2828%29.png)

For **Case 3** where there are portions of broken and completed planes, change the `POINT_DENSE` to `PROBLEM`.

![](../.gitbook/assets/image%20%2830%29.png)

{% hint style="warning" %}
For projects with Unusable POINT\_DENSE, do not waste time assigning/detecting edge types.
{% endhint %}

{% hint style="success" %}
For projects with Problem POINT\_DENSE, extend the edges as far as you can see in the 2D images. Assign the edge types based on the images, but Do Not spend too much time on this. The point cloud is still broken, and bad quality, and should not yield accurate results.
{% endhint %}

