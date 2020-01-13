# Align

![hotkey: hold Shift](../../.gitbook/assets/align-button.png)

1. Under [Modify](modify.md), and [Surface Mode](), select the plane that the edge will be fixed to and press `Space` to lock it. \(this step is optional, but it ensures the edges are aligned on a fixed plane\)
2. Under [Modify](modify.md), and [Vertex Mode](), select the edge \(or Hold `Ctrl` to select multiple edges\) requiring alignment.
3. Click the Align button, or press and hold `Shift` to change to Align mode, then click on the Target edge.
4. The edges you selected in Step 2 will be aligned with the Target edge you selected in Step 3. They will also be fixed to the plane you locked in Step 1.

To get out of Align mode, the user must either click on the Modify button or tap Alt or Shift to switch back to Modify mode.

![](../../.gitbook/assets/align_proj12131_11_7_18.gif)

In the video above, Surface Mode is turned on, then the plane is selected, and Spacebar is hit to lock the plane. Then, in Vertex Mode, the bottom horizontal edge is clicked, the Align button is selected, and the top horizontal edge is clicked on. The lower edge aligns with the upper edge. For the perpendicular edges, the Align hotkeys are used. Note that the plane/surface is still locked. In Vertex Mode the right perpendicular edge is selected, then Shift is held while the left edge is selected. Shift is released and the two perpendicular edges are aligned.

{% hint style="info" %}
Using Align, without locking the plane, will affect the planarity of any planes connected to the edge that is being aligned. If Plane Refine has been used, then it will negate those results too. It will also alter the connected vertices/edges, which can be damaging if the vertices have already gone through the Adjust Vertices process. Use Align with caution.
{% endhint %}

{% hint style="danger" %}
If [Lock Mode](../../advanced-function/lock-mode.md) is on, Alignment may not perform as expected.
{% endhint %}

