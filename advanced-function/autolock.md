# AutoLock

![No hotkey available](../.gitbook/assets/autolock-button.png)

Upon opening a project, Autolock is turned off by default. Users can manually turn it on by clicking the white box next to it. AutoLock will also automatically turn on when [Plane Sort](../tools/adjust-vertices/plane-sort.md) is selected.

When AutoLock is on, each time a vertex is selected, the biggest plane connected to the selected vertex will be locked. The triangulation mode will switch to 1 Image + Locked Plane. This operation allows users to adjust each vertex in only one of the three 2D images, and have it reflected in the other two 2D images. The plane will lock when a vertex is selected on the wireframe, and it will lock when a vertex is selected from the vertices list in the Adjust Vertices panel.

{% hint style="info" %}
It is very important to use AutoLock, or locked planes, when adjusting vertices. Without a plane locked, the vertex adjustment may cause the plane to break and/or will affect the plane's slope accuracy.
{% endhint %}

If AutoLock is being used to adjust a vertex, then the plane must be accurate. This can be done manually when cleaning up the rough, or automatically when running plane refine. 

A locked plane can be unlocked by pressing Spacebar. However, this only unlocks the plane temporarily. AutoLock does not turn off completely when spacebar is hit. Once another vertex is selected, or if the same vertex is re-selected, then the plane will lock again.

{% hint style="danger" %}
To remove AutoLock completely, the box next to AutoLock must be manually unchecked.
{% endhint %}

![](../.gitbook/assets/autolock_proj12131_11_2018.gif)

