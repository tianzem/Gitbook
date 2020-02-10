# Penetrations

{% hint style="warning" %}
For DroneDeploy projects requiring penetrations, you will see "Enterprise" or "Add Obstructions" in the description field/column of the intranet. Please refer to this link for a detailed breakdown of DD description codes: [https://pointivo.atlassian.net/wiki/spaces/CO/pages/187662337/DroneDeploy+Description+Codes](https://pointivo.atlassian.net/wiki/spaces/CO/pages/187662337/DroneDeploy+Description+Codes)

Refer to this link for all other customer requirements on penetrations: [https://pointivo.atlassian.net/wiki/spaces/CO/pages/188907541/Customer+Wireframe+Project+Requirements](https://pointivo.atlassian.net/wiki/spaces/CO/pages/188907541/Customer+Wireframe+Project+Requirements)
{% endhint %}

{% hint style="info" %}
Finish all other wireframing steps before working on the penetrations.
{% endhint %}

#### Detect Penetrations:

One way to start finding all of the penetrations is to use the Detect Penetrations feature. 

## \*Stopped editing right above this line \(special cases at end should stay\)

1. Starting from one of the planes, open the 2D images first and count the total number of penetrations to make sure that none of the penetrations are missed on this plane. Hold `Alt+Ctrl` and hover the mouse on the plane. Notice that the primary edge is highlighted \(if you want to align the penetration with a different edge, then you could [Set Primary Edge](../tools/wireframe-tools/set-primary-edge.md) here to change it\). While holding Alt+Ctrl, Left-click and release to place the anchor vertex, drag the mouse until the penetration is covered on the cloud, and left-click again to place the location of the diagonal vertex.

   ![](../.gitbook/assets/penetrationpage-image1-update_project18479.gif)

2. The penetration will be attached to the plane automatically and it has a special property called Polygon Shape. All of the parameters under Polygon Shape can be changed.

   ![](../.gitbook/assets/penetrationpage-image2-update_project18479%20%283%29.gif)

3. Lock the parent plane first, pick either one of the corners and adjust the vertex via the 2D images using 1 Image + Locked Plane mode. Pick the diagonal vertex and adjust this vertex under the same locked mode. Only two of the diagonal vertices need to be adjusted, and applied, to set the shape of the cutout.

   ![](../.gitbook/assets/penetrationpage-image3-update_project18479.gif)

4. Open the [Adjust Vertices](../tools/adjust-vertices/) panel and check every plane, one by one, in the 2D images to make sure there are no missing penetrations. \(Any immobile obstruction which has a potential affect on setting up a solar panel should be treated as a penetration, including satellite dishes and pipes\)
5. Click [Detect Edge Types](../tools/wireframe-tools/detect-edge-types.md) and and all of the penetration edges will turn to Step Flashing if they are attached correctly. Keep in mind that chimney edges will also automatically be detected as Step Flashing and they will need to be manually changed to Flashing.

   ![](../.gitbook/assets/penetrationpage-image4-update_project18479.gif)

6. If the roof plane is changed or deleted, the penetrations may need to be recreated since they are going get detached or will have moved with the plane.

{% hint style="danger" %}
DO NOT use [AutoLock](../advanced-function/autolock.md) when adjusting penetrations. Manually lock the parent plane, and then adjust using the 2D images with 1 image + Locked Plane triangulation. AutoLock will lock the penetration's plane, not the parent plane that the penetration is attached to.
{% endhint %}

{% hint style="info" %}
For penetrations that are the same type, like pipes and vents, an existing penetration can be copied \(Ctrl + c\) and pasted \(Ctrl + v\). Then the copied version can be moved to the new location. A penetration can also be dragged from one plane to another without having to make the same penetration on a different plane.
{% endhint %}

#### Special Cases:

Flat vent penetrations -- these are hard to see, so pay close attention and double check that they have been included as penetrations:

![Flat Vent Penetrations -- project 52302](../.gitbook/assets/52302-flat-vent-penetrations.png)

![Flat Vent Penetrations -- project 52569](../.gitbook/assets/52569-flat-vent-penetrations.png)

