---
description: This section shows the various methods for creating penetrations.
---

# Penetrations

There are two primary ways to create penetrations. The first is to manually create them, and the second is to use the Detect Penetrations feature. Instructions, tips, and tricks are listed below for each method.

{% hint style="danger" %}
Finish all other wireframing steps BEFORE completing the penetrations.
{% endhint %}

{% hint style="info" %}
For DroneDeploy projects requiring penetrations, you will see "Enterprise" or "Add Obstructions" in the description field/column of the intranet. Please refer to this link for a detailed breakdown of DD description codes: [https://pointivo.atlassian.net/wiki/spaces/CO/pages/187662337/DroneDeploy+Description+Codes](https://pointivo.atlassian.net/wiki/spaces/CO/pages/187662337/DroneDeploy+Description+Codes)

Some DroneDeploy projects will require Obstruction Heights to be added to each penetration as well as any Trees casting a shadow on the roof. The link above will note which project descriptions require this. The links below show how to add Obstruction Heights and Trees: [https://pointivo.atlassian.net/wiki/spaces/CO/pages/337215515/How+to+add+obstruction+heights](https://pointivo.atlassian.net/wiki/spaces/CO/pages/337215515/How+to+add+obstruction+heights) [https://pointivo.atlassian.net/wiki/spaces/CO/pages/372408321/How+to+add+trees+for+solar+projects](https://pointivo.atlassian.net/wiki/spaces/CO/pages/372408321/How+to+add+trees+for+solar+projects)
{% endhint %}

{% hint style="info" %}
Refer to this link for all other customer requirements on penetrations: [https://pointivo.atlassian.net/wiki/spaces/CO/pages/188907541/Customer+Wireframe+Project+Requirements](https://pointivo.atlassian.net/wiki/spaces/CO/pages/188907541/Customer+Wireframe+Project+Requirements)
{% endhint %}

### Manual Penetration Creation:

When a plane is locked, anything wireframed within that plane's boundaries will become a penetration of that plane. If the penetration is a shape that fits within a square/rectangular polygon, such as pipes, vents, and chimneys, then the penetration shortcut can be used. For oddly shaped penetrations, such as HVAC ductwork, L-shaped chimneys, and conduit the penetration polygon will have to be wireframed by creating vertices around the obstruction. To create oddly shaped penetrations, wireframe around the object while staying within the parent plane. To use the shortcut creation method, the hotkeys must be pressed in a specific order:

* Lock the plane that the penetration will be attached to \(a.k.a the parent plane\)
* Hold Alt + Ctrl
  * With those still held down, left-click at the top left corner of the obstruction and release.
    * this will start the penetration polygon
  * Drag your mouse down to the bottom right corner of the obstruction -- the polygon will get bigger as the mouse moves to the diagonal corner.
    * Left-click again, at the penetration's bottom right corner.
    * A penetration polygon will be created, and attached to, the parent plane.
* Each penetration will need to have 2 of its diagonal vertices adjusted, and verified, using Adjust Vertices. The other two unadjusted vertices will snap to their correct location when the others are adjusted.
  * **Turn off AutoLock when adjusting penetration vertices**.
  * Manually lock the parent plane and then adjust 2 diagonal vertices of the penetration. If AutoLock is on, then the penetration's plane will automatically lock when its vertices are selected. They must be adjusted on the locked parent plane instead.

As a last resort, penetrations can be created by drawing a polygon on, and within, another plane using the Create button. Lock the large/parent plane that the penetration is on, then use Create to place each vertex around the penetration and close off the polygon. That polygon automatically attaches itself to the larger plane and becomes a child/penetration of the parent plane.

{% hint style="info" %}
Use Camera Projection, and/or the 2D images from the Images Panel, to count all of the penetrations on the roof. Ensure that all are accounted for with penetration polygons.
{% endhint %}

### Detect Penetrations:

![](.gitbook/assets/detect-penetrations.png)

One way to start finding all of the penetrations is to use Detect Penetrations in the Wireframe Tools tab of the Tools panel. This feature will find, and wireframe, all of the objects it detects as penetrations. Once the button is clicked, Detect Penetrations will start running, it will create a new branch called "Penetrations", and it will have the wireframe with the penetrations on that branch. When detect penetrations has finished running, open the penetrations branch and use Save As to save the penetration wireframe onto the qa branch.

* Every penetration that is detected needs to be checked to confirm it is actually a penetration. Detect penetrations will sometimes detect things like discolored shingles or random sticks/debris as penetrations, even though they're not.
  * Anything that is not a true penetration must be deleted -- select the surface of the penetration and hit Ctrl+Del to delete it.
* Each penetration will need to have 2 of its diagonal vertices adjusted, and verified using, Adjust Vertices. The other two unadjusted vertices will snap to their correct location with the movements of the adjusted ones.
  * **Turn off AutoLock when adjusting penetration vertices**.
    * Manually lock the parent plane and then adjust 2 diagonal vertices of the penetration. If AutoLock is on, then the penetration plane will automatically lock when its vertices are selected. They must be adjusted on the locked parent plane instead.

### Camera Projection

Camera projection displays one of the point cloud's 2D images onto a plane in the wireframe. This feature is useful when trying to locate all of the penetrations within a plane. Sometimes the images in the Adjust Vertices panel are not large, or clear, enough to see all of the penetrations. With camera projection, the images are displayed onto the actual plane instead of inside a thumbnail. On large Commercial projects that require obstructions, Camera Projection is a huge time-saver. Instructions for camera projection are listed below followed by a brief video of it in the wireframe tool.

**To use Camera projection:**

* **For Residential structures: Leave the tool in 3D mode.**
  * For Commercial structures: Put the wireframe tool in 2D mode, then continue with the following instructions.
* Turn off the point cloud \(hit P\) so that it does not overlap with the image from the camera projection.
* Hold C and move the mouse over one of the planes
* A 2D image will be projected onto the plane covered by the mouse
  * if the image is blurry:  Hold C and Middle Mouse Scroll - this flips through, and projects, the available images of that plane \*occasionally all images will be bad\*
  * Lock the plane and draw out the penetrations like normal
  * Unlock the plane once all of its penetrations are created
* To change planes, rotate the point cloud and Hold C + move the mouse over the new desired plane
  * The 2D image will project onto the new plane
  * \*if a previous plane is still locked, then the image will not project onto the new plane\*
* Hit Alt + C to turn off Camera Projection

{% embed url="https://drive.google.com/file/d/15SIgoWGB67WeMx5k7WK9Fwll8NIx4HMx/view" %}

{% hint style="success" %}
**Hit Alt + C to turn off Camera Projection**
{% endhint %}

**Commercial Structure Example with Camera Projection Off & On:**

**For Commercial structures, put the wireframe tool into 2D mode** instead of 3D. This will project the image straight down onto the flat plane of the commercial roof.

* Sometimes the edges and/or vertices won't be selectable in 2D mode. When this happens, try switching back to 3D mode, zoom out some, rotate the cloud a little bit, and then put it back into 2D mode. If the edges/vertices still aren't selectable, then close the project and reopen it.

![](.gitbook/assets/camera-projection-off.png)

![](.gitbook/assets/camera-projection-on.png)

### **Penetration Edge Types**

All penetration edge types should be Step Flashing, except for those with wall edges that are parallel to ground -- such as chimneys. For chimney penetrations, the edges that are parallel to ground should be Flashing and the edges that are not parallel to ground should be Step Flashing. Detect Edge Types will detect all penetration edges as step flashing. The parallel-to-ground chimney edges will have to be manually changed to Flashing.

![Yellow arrows point to the Flashing chimney edges -- parallel to ground &amp; against a wall](.gitbook/assets/chimney-flashing-edges.png)

### Detached Penetrations

* If a parent plane is broken, or drastically altered, then the pentrations can become detached.
* Always check that all penetrations are attached. This can be done a couple of different ways.
  * The first way is to use [Select Children](tools/wireframe-tools/select-children.md).
    * In surface mode, select the parent plane.
    * Go to the Wireframe Tools tab, in the Tools panel, and click the Select Children button.
    * All of the attached penetrations' planes will turn red -- any that are not red, on that specific parent plane, are not attached.
  * The second way is to turn off the Point Cloud and look at the colors of the penetration planes.
    * If the penetrations have a purple tint to them, then they are attached.
    * If the penetrations have a green tint to them, then they are detached.
  * The third way is to consult the project's Data Package.
    * In the data package if there is a very faint light-grey letter inside a penetration's wireframe, then that penetration is detached. All non-penetration planes will have a light grey letter inside of them, in the data package. Penetrations are meant to be holes in a plane. If they have a letter inside their wireframe, then they are not showing as holes and are forming their own separate plane instead.

### Polygon Shape Properties & Alignment Edge

When a penetration is created, using the shortcut, a Polygon Shape property is assigned to it. This property allows users to alter the rotation, number of sides, and the alignment edge of the penetration polygon.

![](.gitbook/assets/polygon-shape-property.png)

The Alignment Edge behaves similarly to Set Primary Edge. However, Alignment Edge refers to the primary aligning edge of the individual penetration/polygon instead of the entire parent plane. To change a penetration's alignment edge: 

* In surface mode, select the penetration that needs to be realigned.
* In the Inspector panel, next to Alignment Edge, click Set.
* Click on the edge of the parent plane that the penetration polygon should be aligned to -- this will realign/reorient the penetration to be aligned with the desired edge

{% hint style="danger" %}
DO NOT use [AutoLock](advanced-function/autolock.md) when adjusting penetrations. Manually lock the parent plane, and then adjust using the 2D images with 1 image + Locked Plane triangulation. AutoLock will lock the penetration's plane, not the parent plane that the penetration is attached to.
{% endhint %}

{% hint style="info" %}
For penetrations that are the same type, like pipes and vents, an existing penetration can be copied \(Ctrl + C\) and pasted \(Ctrl + V\). Then the copied version can be moved to the new location. They can also be dragged from one plane to another without having to make the same penetration on a different plane.
{% endhint %}

### Special Cases:

**Flat Vent penetrations** -- these are hard to see, so pay close attention and double check that they have been included as penetrations. They usually have different markings than the rest of the non-vent shingles, such as slits in the sides or are slightly misshapen in comparison. They can easily blend in and be missed when they are the same color as the normal shingles/tiles:

![Flat Tile Penetration Closeup - project 63423](.gitbook/assets/flat-tile-penetration-close-up_63423.png)

![Flat Tile Penetration Closeup - project 52569](.gitbook/assets/flat-tile-2-penetration-close-up_52569.png)

![Flat Metal Vent Penetrations -- project 52302](.gitbook/assets/52302-flat-vent-penetrations.png)

![Flat Tile Vent Penetrations -- project 52569](.gitbook/assets/52569-flat-vent-penetrations.png)

\*\*Occasionally there will be Replacement Tiles that can look a lot like the flat vents. The **replacement tiles ARE NOT penetrations**\*\* -- some examples are below:

![Replacement Shingles - project 63928](.gitbook/assets/image-from-ios.jpg)

![Replacement Tiles - project 63412](.gitbook/assets/replacement-tiles_63412.png)

![Replacement Tiles - project 63503](.gitbook/assets/replacement-tiles_63503.png)

![Replacement &amp; Repair Tiles - project 63423](.gitbook/assets/63423-replacement-tiles.png)

**Satellite Dish penetrations** -- The entire outline/footprint of the satellite dish needs to be included in the penetration polygon, not just the small area that penetrates the roof. Correct and incorrect image examples are shown below:

![](.gitbook/assets/satellite-dish-footprint.png)

![](.gitbook/assets/satellite-dish-incorrect.png)

#### Conduit and Pipes/Wires

In addition to the solar panels, the conduit, and any other piping or wiring, needs to be added as penetrations. Depending on the customer, these may also need obstruction heights added to their planes.

![Solar panel conduit - 57301](.gitbook/assets/57301-conduit-penetrations.png)

