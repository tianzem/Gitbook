# Project Issues

## Reprojection Error

A Reprojection Error \(RPE\) occurs when there is an error in aligning cameras during the reconstruction process, thereby causing one or more of the 2D images to display an inaccurate location of a vertex.

![Project 13210](../.gitbook/assets/rpe_project13210.gif)

## Noisy Point Cloud

A Noisy Point Cloud occurs when the point cloud structures are not crisp, and the edges/corners of the structures are unclear.

![Project 13097](../.gitbook/assets/noisy-point-cloud_project13097.gif)

## Broken Point Cloud

A Broken Point Cloud is typically caused by occlusion, like tree coverage or a lack of enough image overlap. The structure may still be correct, but missing portions of it.

![Project 13184](../.gitbook/assets/broken-point-cloud_project13184.gif)

## Wrong Region of Interest

The Wrong Region of Interest \(ROI\) issue occurs when the ROI is specified but the structure is unclear, incomplete, or the ROI is in the wrong location altogether.

![Project 10737](../.gitbook/assets/wrong-roi_project10737.gif)

## Blurry Frames

Blurry Frames is when one or more of the 2D images have blurriness and are unclear.

![Project 7511](../.gitbook/assets/blurry-frames_project7511.gif)

## Image Illumination

Image Illumination means that one or more of the 2D images were over or underexposed, making it more difficult to accurately verify the location of a vertex. This is typically due to shadows, glare, or a very bright/dark time of the day during drone capture.

![Overexposed\_Project 13004](../.gitbook/assets/image-illumination_bright_project13004.gif)

![Shadow\_Project 13176](../.gitbook/assets/image-illumination_dark_project13176.gif)

## Partial Occlusion

Partial Occlusion is the result of part of the structure being occluded/covered on the point cloud and in the 2D images. This causes the structure, and resulting vertices, to be estimated and inaccurate. Occlusion is usually the result of trees or overhangs.

![Partial Occlusion Tree\_Project 13124](../.gitbook/assets/partial-occlusion_tree_project13124.gif)

![Partial Occlusion Overhang\_Project 13263](../.gitbook/assets/partial-occlusion_overhang_project13263.gif)

## Indeterminate Region of Interest

An Indeterminate ROI means that the ROI is unclear. This can be the result of the ROI not being specified, no structure in the ROI at all, or more than one significant structure \(outside of the customer's request\) is being included in the ROI.

![Project 11697](../.gitbook/assets/indeterminate-roi_project11697.gif)

## Unsupported Geometry

Unsupported Geometry means that part of the structure cannot be represented, often because of a conical or curved structure.

![Project 10793](../.gitbook/assets/unsupported-geometry_project10793.gif)

## Low Point Cloud Density

Low Point Cloud Density is when the density of the point cloud is below the recommended levels \(2,500 points per square meter\)

![Project 13159](../.gitbook/assets/low-point-cloud-density_project13159.gif)

## Defective Reconstruction

Defective Reconstruction means that the project was unable to be processed because of partial, or completely wrong, image alignment. It causes the point cloud to no longer be geometrically sound.

![Project 9143](../.gitbook/assets/defective-reconstruction_project9143.gif)

## Large Structure Sample Distance

Large Structure Sample Distance \(SSD\) occurs when the camera is too far from the structure or has low resolution. This results in the pixel size on the structure being large, and/or the 2D images loading from a far distance and becoming blurred when zooming in on them. The accuracy of the wireframe will not meet expectations.

![Project 13159](../.gitbook/assets/large-ssd_project13159.gif)

## Smoothed Point Cloud

A Smoothed Point Cloud is often the result of meshing, and will cause the surfaces to be blended and the point cloud to have edges that are not crisp.

![Project 13004](../.gitbook/assets/smoothed-point-cloud_project-13001.gif)

## Project Type Mismatch

This Project Issue is only for Standard DroneDeploy project.

When the actual project structure type does not match the input structure type, please mark this project issue and at the same time, change the structure type to what it should be.

For example, we receive a huge Commercial building but it was detected as SingleFamily. Please check this project issue and change the structure type to Commercial.

![](../.gitbook/assets/2018-09-13_14-11-59.jpg)

Refer to Structure Types page to understand the definition of different structure types.

{% page-ref page="structure-types.md" %}

