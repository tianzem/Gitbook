# Penetration

{% hint style="warning" %}
Penetrations are required for Tesla projects only. You will see "label obstructions" in the description field of the intranet for these projects.
{% endhint %}

1. Finish the entire roof first before starting the penetrations.
2. Starting from one of the planes, open the 2D images first and count the total number of penetrations to make sure that you don't miss any penetrations on this plane. Hold `Ctrl+Alt` and hover your mouse on the plane, you will see the primary edge is highlighted \(you could [Set Primary Edge](../tools/set-primary-edge.md) here\). Click your mouse to draw the anchor vertex, drag your mouse to change the size of the cutout and click your mouse again to place the location of the diagonal vertex.

   ![](../.gitbook/assets/penetration1%20%281%29.jpg)

3. The penetration will be attached to the plane automatically and it has a special property called Polygon Shape. All of the parameters under Polygon Shape can be changed.

   ![](../.gitbook/assets/penetration2%20%281%29.jpg)

4. Lock the plane first, pick either one of the corners and adjust the vertex via 2D image using 1 Image + Locked Plane mode. Pick the diagonal vertex and adjust this vertex under the same locked mode. Only two diagonal vertices are needed to be adjusted, and applied, to set the shape of the cutout.

   ![](../.gitbook/assets/penetration3%20%281%29.jpg)

5. Open the [Adjust Vertices](../adjust-vertices/) panel and check every plane, one by one, in the 2D images to make sure there are not any missing penetrations. \(Any immobile obstruction which has a potential affect on setting up a solar panel should be treated as penetration, including the satellite dish and the pipes\)
6. Click [Detect Edge Types](../tools/detect-edge-types.md) and you will see that all of the penetrations will turn to Step Flashing if they are attached correctly. Keep in mind that chimney edges will also be detected as Step Flashing and will need to be manually changed to Flashing.

   ![](../.gitbook/assets/penetration4.jpg)

7. If the roof plane is changed or deleted, you may need to redo the penetrations since they are going to be detached or will have moved with the plane.

{% hint style="info" %}
For penetrations that are the same type, like pipes and vents, you can copy \(ctrl + c\) and paste \(ctrl + v\) an existing penetration and then move the copied version to the new location. You can also drag a penetration from one plane to another without having to remake the same penetration on a different plane.
{% endhint %}

