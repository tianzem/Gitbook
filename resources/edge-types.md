---
description: >-
  There are a variety of Edge Types available in the 3D tool, and each of them
  are used to distinguish different parts of the roof. This page lists the
  requirements for each edge type.
---

# Edge Types

**Common Edge Types**

|  | Number of Planes | Angle | Parallel to Ground |
| :--- | :--- | :--- | :--- |
| Eave | 1 |  | √ |
| Rake | 1 |  | × |
| Hip | 2 | "Λ" | × |
| Valley | 2 | "V" | × |
| Ridge | 2 |  | √ |
| Flashing | Must be against a wall or chimney | × | √ |
| Step Flashing | Must be against a wall or chimney | √ | × |
| Parapet | Only on flat roofs that are surrounded by, and enclosed in, a low wall/ledge | × | √ |
| Transition | 2 \(This is an edge that represents a pitch change. It will always be parallel to the ground and will be at the intersection of 2 planes, where one plane is above it and the other is below it\) | × | √ |

**Edge Type Example - QA Project: 6573**

![standard singlefamily structure with assigned edge types](../.gitbook/assets/edge-types-update.jpg)

## Special Case Valleys

project 49213

![](../.gitbook/assets/parallel-valleys.jpg)

{% hint style="danger" %}
Although these edges appear parallel to ground, in reality they are slightly sloped to prevent rain water from getting stuck. Therefore, they are Valleys instead of transitions. Another way to know that these are not transition edges is that a transition edge is parallel to ground with one plane above it and one plane below it. These edges have both connected planes above them, so they can't be transition.
{% endhint %}

