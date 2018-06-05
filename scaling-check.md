**Steps to check the scaling issue using Nearmap**

Every time we receive a **DroneDeploy Standard** project, we would need to check whether the scaling is correct or not first before actually QA the project. 

1. Take `9630` as an example, when it becomes `IN_QA`, open the project and create the start&end vertex on a long and clear edge in 3D. Adjust the vertices to get the measurement.
![](/Nearmap/PV Measurement.jpg)

2. Find the address of the project from Intranet.
![](/Nearmap/address.jpg)

3. Open the Nearmap https://go.nearmap.com/ and search the address on the map browser. (Don't abuse the map since we have a data usage limitation)
![](http://pointivo-drop.s3.amazonaws.com/TianzeMedia/Nearmap.gif)

4. Measure the same edge or area in the Nearmap.
![](http://pointivo-drop.s3.amazonaws.com/TianzeMedia/Nearmap%20Measurement.gif)

5. Compare the two measurements and if the difference is more than 6 inches, let us know on the wireframe channel with the compared picture.
![](/Nearmap/comparison.jpg)

6. If the two measurements match with each other, then it is good to QA.
