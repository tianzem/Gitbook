---
description: 'Hotkey: R'
---

# Region of Interest

The Region of Interest (ROI) is an opaque, grey box outlining the structure that needs to be wireframed on the point cloud. When the point cloud contains multiple structures, users can look at the ROI to determine which structure is intended for processing. In the Layers panel, the ROI can be turned on/off by clicking the eyeball to the left of 'Region of Interest', or by using the hotkey: R

**For non-Sunrun DroneDeploy ROIs:**&#x20;

* The ROI is usually correct and precise.&#x20;
* DroneDeploy's customers get to draw their ROI directly on the structure's point cloud, making them very accurate.&#x20;

{% hint style="warning" %}
**There should only be one ROI with one structure inside for each project.** If there are multiple structures within one ROI, then the project should be put in\_support. If there are multiple ROIs in one project, with no duplicates for each additional ROI, then the project should be put in\_support. Refer to this link for rules about putting projects in\_support: [https://pointivo.atlassian.net/wiki/spaces/CO/pages/170229773/In+Support+Projects](https://pointivo.atlassian.net/wiki/spaces/CO/pages/170229773/In+Support+Projects)
{% endhint %}

![](../.gitbook/assets/roi.gif)

{% hint style="info" %}
Singlefamily Sunrun projects will not have a ROI included
{% endhint %}
