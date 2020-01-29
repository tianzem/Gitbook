# Detect Cutouts

The Detect Cutouts button finds all of the dormers in a wireframe and automatically creates the wireframe for the cutout below them. The dormer can consist of one, or two, planes that each have one of their edges connected to part of the surface of another plane.

\*\*Always **SAVE** before using Detect Cutouts.

{% hint style="info" %}
Using Detect Cutouts will turn off [Auto Plane](../../advanced-function/auto-plane.md)! Wait to apply this feature until after the wireframe is verified. 
{% endhint %}

* The example below is of 3 dormers that each have 2 planes with one edge connected to the surface of the larger plane behind them. 
  * These connecting edges must have their vertices adjusted on the manually locked larger plane.
    * AutoLock and Plane Sort will automatically lock the dormers' smaller planes when adjusting those vertices -- **DO NOT** adjust them based on AutoLock, turn it off and manually lock the large connecting plane
* Once those vertices are verifed, the Detect Cutouts button will find/detect all of the dormers in the scene, create a cutout for each, and [Attach](attach.md) those connected dormer cutout planes onto the larger plane.
* It's unnecessary to adjust, or verify, the vertices created from the cutout. They will be correct based on the accuracy of the dormer planes.
* Use [Select Children](select-children.md) to verify the cutouts are attached to the main plane.

![](../../.gitbook/assets/detect-cutout.gif)

{% hint style="warning" %}
If there are extra vertices in the cutout plane, after Detect Cutouts runs, then the Rake edges on each side of the dormer ridge are not symmetrical. This can also be the effect of the end vertex of the dormer's Ridge not being parallel with the end vertices of the dormer's Eave edges.
{% endhint %}

{% hint style="warning" %}
If there are duplicated edges in the dormer cutout, then the dormer vertices were not adjusted on the locked, large plane behind them.
{% endhint %}

**Duplicated edges and/or extra vertices can be fixed two ways:** 

1. Manually delete the extra edges. If the cutout detaches during this process, then reattach it using the [Attach](attach.md) button, or shortcut. 
2. Reload the last saved version. Manually lock the large plane, readjust and re-verify the connected dormer vertices. Save and hit Detect Cutouts to run it again.

