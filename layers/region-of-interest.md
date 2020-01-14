---
description: 'Hotkey: R'
---

# Region of Interest

The Region of Interest \(ROI\) is an opaque, grey box that outlines the required structure on the point cloud. When the point cloud is made up of multiple structures, users can look at the ROI to determine which structure is intended for processing. In the Layers panel, the ROI can be turned on/off by clicking the eyeball to the left of 'Region of Interest', or by using the hotkey: R

![](../.gitbook/assets/roi.gif)

In DroneDeploy projects, the ROI is usually correct. The customers get to draw their ROI around the structure on the point cloud, making them very accurate. Occasionally there will be multiple structures included in one ROI. In that situation, the customer would need to be contacted to clarify which structure should be processed. There should only be one structure per ROI per project. 

{% hint style="info" %}
DroneDeploy Enterprise projects will not have a ROI included
{% endhint %}

For Kespry projects, the ROI might be a little offset and/or not very accurate. Kespry's ROIs are used to design the flight pattern, and the cloud is created based off of that. Kespry customers do not get to see the cloud while setting the ROI. 



#### How to deal with a missing/inconclusive ROI:

When the ROIs are offset, incorrect, or completely missing, the Cameras layer can be used to clarify the ROI. The Cameras layer can be turned on, in the Layers panel, and the user can determine the ROI based on which structure the red cameras are floating above in the 3D window. If the Cameras layer does not clarify the ROI, then the customer will need to be contacted.

