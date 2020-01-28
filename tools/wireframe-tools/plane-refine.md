# Plane Refine

When clicking the Plane Refine button, in the Wireframe Tools tab of Tools, the Machine Learning system is going to modify the location of each vertex. It will save the current wireframe as a Rough wireframe in the qa branch. Once the plane refine process is complete, it will save the refined wireframe as a new version named Wireframe-4-Java under the Autogen branch.

If the 3D Tool is closed while Plane Refine is running, then when refinement is complete, and the qa wireframe is opened, it will automatically load the refined Autogen branch with the Wireframe-4-Java set as the version. If the 3D Tool is left open while Plane Refine is running, then when refinement is complete the user will need to manually switch to the Autogen branch and then select Wireframe-4-Java as the version in order to load the plane refined wireframe. After that whenever the wireframe is saved, the branch will switch back to qa but will still maintain the refined Wireframe-4-Java as the version.

