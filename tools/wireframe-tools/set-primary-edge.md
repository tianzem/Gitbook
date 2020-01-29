# Set Primary Edge

Every plane has a Primary Edge that is automatically detected. This edge will be the one that is the most parallel to the ground, in that plane, and it won't necessarily be the largest edge. Any attached penetrations, specifically drawn by the Alt + Ctrl shortcut, are going to be aligned with this defaulted primary edge.

However, in some specific cases, the primary edge might be incorrect or the penetrations may need to aligned with a different edge in the given plane. In those scenarios, the primary edge can be set manually by using the Set Primary Edge button.

1. While in [Surface Mode](../../mode.md), select the plane that contains the desired Primary Edge.
2. Click Set Primary Edge.
3. Select the Edge is going to be set as the primary \(it's not necessary to switch to [Vertex mode](../../mode.md) here\).
4. The selected edge is now set as the Primary Edge for this Plane.

After setting the new primary edge, users will need to go back to Vertex mode in order to create penetrations that will align with that primary edge.

![](../../.gitbook/assets/setprimaryedge_proj18578_11_2018.gif)

**To realign existing penetrations to the new primary edge:**

* In Surface mode, select all of the penetrations that are misaligned to the new primary edge.
* Open the Inspector Panel
* Next to Alignment Edge, click on the Set button and then click on the new primary edge in the plane.
* This will automatically rotate the selected penetrations to be aligned with the new primary edge.

![](../../.gitbook/assets/aligning-existing-penetrations-to-a-new-primary-edge.png)

