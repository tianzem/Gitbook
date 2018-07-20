# Plane Refine

When clicking the Plane Refine button, in the Tools tab of Properties, the Machine Learning is going to tweak the location of each vertex. It will save the current wireframe as a Rough wireframe in the qa branch. Once the plane refine process is done, it will save the refined wireframe as a new version named Wireframe-4-Java under the Autogen branch.

If you close the 3D Tool while Plane Refine is running, then when refinement is complete, and you open the qa wireframe, it will automatically load the refined Autogen branch with the Wireframe-4-Java set as the version. If you leave the 3D Tool open while Plane Refine is running, then when refinement is complete you will need to manually switch to the Autogen branch and then select Wireframe-4-Java as the version to load the plane refined wireframe. After that whenever you save, the branch will switch back to qa but will still maintain the refined Wireframe-4-Java as the version.

