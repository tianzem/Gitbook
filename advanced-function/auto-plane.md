# Auto Plane

![No hotkey available](../.gitbook/assets/auto-plane-button.png)

Auto Plane is turned on by default. When Auto Plane is on, all of the vertices that satisfy the planar constraint of angle threshold will be detected as a plane. When Auto Plane is off, planes will no longer be automatically detected.

![](../.gitbook/assets/auto-plane_proj18520_11_2018.gif)

The existing geometry in the video is not detected because Auto Plane is turned off. Once Auto Plane is turned on, the geometry is then automatically detected as a plane.

Deleting a surface/plane will turn Auto Plane off.

Manually creating a plane, using Create from Edges, will turn Auto Plane off. 

If you turn Auto Plane back on, after it has been turned off, those changes will revert back to their original states. This can become quite time consuming, and frustrating, because you will have to go back and delete unwanted planes again and/or select all of the edges and create the missing planes again. It becomes a lot of back-and-forth that can be avoided if these steps are saved for the end.

{% hint style="warning" %}
When planes are manually created/deleted, then Auto Plane will turn off. If the project is saved with Auto Plane off, then when the project is later reopened those planes will disappear again due to Auto Plane defaulting back to being on. To remedy this: open the project, turn Auto Plane off, click the drop-down next to Version, and click the most recent version to reload it. This will recreate any of the previous manually created/deleted planes.
{% endhint %}

{% hint style="danger" %}
Performing functions that turn Auto Plane off should be saved for the last steps of a project.
{% endhint %}

