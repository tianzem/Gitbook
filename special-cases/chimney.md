# Chimneys

Chimneys can be placed in many different ways/places on a given structure. Whether or not a chimney needs to be wireframed, is based on the customer's standards. The chimney's location on a plane is the determining factor for its inclusion in the wireframe.

There are two types of chimney placement: Chimneys that break an Edge, and Chimneys that are in the middle of a Plane. The table below displays the customer wireframing requirements for chimneys based on their placement type. Example images are included, after the table, to show both types. 

| Customer | Include if Chimney breaks an Edge | Include if Chimney is in the middle of a Plane |
| :--- | :--- | :--- |
| Kespry | Yes | No |
| DroneDeploy \(all types\) | Yes | Yes |
| BetterView | Yes | No |
| Airbus Aerial | Yes | No |
| FairFleet | Yes | No |
| KittyHawk | Yes | No |

* The first 2 images below are examples of a Chimney breaking an Edge -- all customers require this type of chimney to be wireframed:

![](../.gitbook/assets/chimney-breaks-an-edge.png)

![](../.gitbook/assets/chimney-breaks-a-ridge.png)

* The image below is an example of a Chimney in the middle of a Plane:

![](../.gitbook/assets/chimney-in-the-middle-of-plane.png)

{% hint style="info" %}
The chimney's edges that are parallel to ground should always be Flashing. The angled edges against the chimney should always be Step Flashing. The example images show the correct edge types. Detect Edge Types usually does not correctly detect all of a chimney's edges.
{% endhint %}

For certain DroneDeploy customers, chimneys are required to have obstruction heights. Instructions on how to add heights to chimney edges can be found here: 

[https://pointivo.atlassian.net/wiki/spaces/CO/pages/408027137/How+to+indicate+chimney+height](https://pointivo.atlassian.net/wiki/spaces/CO/pages/408027137/How+to+indicate+chimney+height)

