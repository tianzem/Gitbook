---
description: >-
  Each edge type is used to distinguish different parts of a roof. This page
  lists the requirements for each edge type, as well as how to handle special
  cases.
---

# Edge Types & Requirements

{% hint style="info" %}
For information on the how to change edge types, and view all of a specific type at once, please refer to the [Edges panel](edges.md) section of the User Guide.
{% endhint %}

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

![Singlefamily structure with assigned edge types](.gitbook/assets/edge-types-update.jpg)

## Special Case Valleys

project 49213

![](.gitbook/assets/parallel-valleys.jpg)

{% hint style="danger" %}
Although these edges appear parallel to ground, in reality they are slightly sloped to prevent rain water from getting stuck. Therefore, they are Valleys instead of transitions. Another way to know that these are not transition edges is that a transition edge is parallel to ground with one plane above it and one plane below it. These edges have both connected planes above them, so they can't be transition.
{% endhint %}

## Special Case Parapets

project 51087

![](.gitbook/assets/small-sloped-parapet-edges_51087_12_6_19.png)

{% hint style="danger" %}
Usually we define a parapet edge as being parallel to ground and surrounded by a parapet wall. However, for cases like the structure above all edges would be Parapets. The 2 sloped edges are only slightly angled and the roof plane is all surrounded by a parapet wall.
{% endhint %}

