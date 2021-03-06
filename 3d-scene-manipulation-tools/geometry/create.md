# Create

![hotkey: hold Alt + left click](../../.gitbook/assets/create-button.png)

Under Create, users are able to create a vertex anywhere within the point cloud. If two vertices are created, then a connecting edge will also form between those 2 vertices. Users can either click the Create button, in the upper toolbar of the 3D tool, or the hotkey can be used.   
  
If the Create button is used, then a new vertex will be created after each left-click of the mouse. To end the string of created vertices/edges, right-click anywhere in the 3D window. This ends the string, but the Create function will still be active. If left-click is used again, then another string of vertices/edges will begin. To get out of Create mode completely, another option must be selected such as [Modify](modify.md) or [Select](select.md); tapping Alt or Shift will set the tool back to Modify mode.

To use the hotkey: Press and hold Alt + left-click anywhere on the point cloud. Then, while still holding Alt, drag the mouse to another location and left-click on the point cloud again. This creates a connecting edge between the two vertices, and will continue to create vertices/edges for as long as these steps are being executed. To end the connection, right-click anywhere in the 3D window. When Alt is released, the Create function will turn off and the tool will default back to Modify. 

{% hint style="info" %}
[Snap mode](../../advanced-function/snap-mode.md) also affects the location, and placement, when creating vertices. 
{% endhint %}

{% hint style="warning" %}
Create only works when the tool is in [Vertex mode](../../mode.md). Nothing will be created when the tool is in [Surface mode](../../mode.md).
{% endhint %}

