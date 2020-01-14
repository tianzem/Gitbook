---
description: 'Hotkey: R'
---

# Region of Interest

The Region of Interest \(ROI\) is an opaque, grey box that outlines the required structure on the point cloud. When the point cloud contains multiple structures, users can look at the ROI to determine which structure is intended for processing. In the Layers panel, the ROI can be turned on/off by clicking the eyeball to the left of 'Region of Interest', or by using the hotkey: R

{% hint style="warning" %}
There should only be one structure inside of one ROI for each project. If there are multiple structures within one ROI, or if there are multiple ROIs in one project, then the customer will need to be contacted for clarification.
{% endhint %}

![](../.gitbook/assets/roi.gif)

For Kespry projects, the ROI might be a little offset and/or not very accurate. Kespry's ROIs are used to design the flight pattern, and the cloud is created based off of that. Kespry customers do not get to see the cloud while setting the ROI. 

In DroneDeploy projects, the ROI is usually correct. The customers draw the desired ROI around the structure on the point cloud, making them very accurate. 

{% hint style="info" %}
DroneDeploy Enterprise projects will not have a ROI included
{% endhint %}

### How to deal with a missing/inconclusive ROI:

When the ROIs are offset, incorrect, or completely missing, the Cameras layer can be used to clarify its location. Turn the Cameras layer on, in the Layers panel, and a pattern of red cameras will be floating above the intended structure on the point cloud \(image below\). If the Cameras layer does not clarify the ROI, then the customer will need to be contacted.

![](../.gitbook/assets/cameras-for-roi.png)

