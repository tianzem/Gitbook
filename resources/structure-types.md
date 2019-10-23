---
description: >-
  Generally, the structure type listed will need to be changed by the user upon
  opening the project. The default selection is not always correct, and the
  price difference is quite significant!
---

# Structure Types

{% hint style="info" %}
If you are unsure what type of structure is shown on the cloud, then use Google Maps to look up the address. You will be able to see if the structure is part of a neighborhood or if it's surrounded by a parking lot/spaces. A lot of times commercial structures will already be labeled on the map. 
{% endhint %}

## Special Cases

Some point clouds will be extremely broken, to the point of being unusable, but you are still able to tell what structure type is being shown. In these cases, you would select the structure type that it should be if it wasn't broken. Examples below:

![Special Case - SINGLEFAMILY - driveway to the right](../.gitbook/assets/unknown-or-singlefamily_49053.png)

![Special Case - SINGLEFAMILY - walkway to the front door; deck in the back](../.gitbook/assets/unknown-or-singlefamily_49046.png)

![Special Case - SINGLEFAMILY](../.gitbook/assets/unknown-or-singlefamily_49048.png)

## SINGLEFAMILY

A single structure that houses 1 family. These structures can be small or large \(mansions\), and may have a detached garage or pool house nearby. A good sign for Singlefamily is that they generally only have one driveway. Sometimes they will have a fence around the backyard, or be separated by a privacy fence from the surrounding structures.

![SINGLEFAMILY - Large house/mansion](../.gitbook/assets/single-family-1.gif)

![SINGLEFAMILY - standard size with fenced in backyard](../.gitbook/assets/single-family-2.gif)

![SINGLEFAMILY - standard size with detached garage in back](../.gitbook/assets/single-family-3.gif)

## MULTIFAMILY

A structure that houses more than 1 family. This can be anything from a condominium, or duplex, to a large apartment complex. Look for shared parking areas, multiple balconies/patios, more than 1 backyard. Condos and townhouses may look smaller \(like a singlefamily\), but they will have more than one driveway.

![MULTIFAMILY- small](../.gitbook/assets/multifamily_duplex_49106.png)

![MULTIFAMILY - large](../.gitbook/assets/multifamily-1.gif)

![MULTIFAMILY - small](../.gitbook/assets/multifamily_condos_49105.png)

![MULTIFAMILY - large](../.gitbook/assets/multifamily-2.gif)

![MULTIFAMILY - large](../.gitbook/assets/multifamily_apartments_unknown-project-number.png)

{% hint style="info" %}
Occasionally there will be a point cloud of a multifamily structure \(like the one above\), but the ROI is only around one individual section/'house' of the structure. In this case the structure type would follow the ROI and become singlefamily instead of multifamily. The ROI would be around a single family portion of the multifamily structure.
{% endhint %}

## MIXED

{% hint style="warning" %}
IGNORE this type - deprecated
{% endhint %}

## COMMERCIAL

Factories, churches/cathedrals, hotels, warehouses, restaurants, malls, offices, schools, neighborhood clubhouses, covered picnic areas, parking garages. Look for structures surrounded by a parking lot or with marked parking spaces. Sometimes smaller commercial structures, such as a neighborhood clubhouse, have outdoor seating surrounding it \(picnic tables, several chairs surrounding a pool, etc.\). A lot of large commercial structures will have HVAC units on the roof.

![COMMERCIAL - small - Golf Course Clubhouse](../.gitbook/assets/commercial_small_49109.png)

![COMMERCIAL - School](../.gitbook/assets/commercial-1.gif)

![COMMERCIAL - Golf Course Picnic Area - used Google Maps to identify this one](../.gitbook/assets/commercial_clubhouse_49108%20%281%29.png)

![COMMERCIAL - Shed with a metal roof - used Google Maps to confirm on commercial property](../.gitbook/assets/commercial-or-unknown_48540.png)

![COMMERCIAL - Restaurant](../.gitbook/assets/commercial-2.gif)

![COMMERCIAL - Covered mailboxes in multifamily neighborhood](../.gitbook/assets/commercial-or-unknown_48331.png)

![COMMERCIAL - Small Store - used google maps to confirm](../.gitbook/assets/commercial_small_48468.png)

![COMMERCIAL - School](../.gitbook/assets/commercial-3.gif)

![COMMERCIAL - Church](../.gitbook/assets/commercial_small_48429.png)

## UNKNOWN

A structure is included but the point cloud of the structure is extremely broken, and the intended structure type is unrecognizable.

![UNKNOWN](../.gitbook/assets/unknown-or-none_49071.png)

![UNKNOWN](../.gitbook/assets/none-or-unknown_49073.png)

![UNKNOWN](../.gitbook/assets/none-or-unknown2_49072.png)

## NONE

No structure in the scene or within the Region of Interest.

![NONE - No structure - grass field](../.gitbook/assets/none-1.gif)

![NONE - No structure - broken grass area](../.gitbook/assets/none-2.gif)

![NONE - No structure - parking lot](../.gitbook/assets/none-3.gif)

