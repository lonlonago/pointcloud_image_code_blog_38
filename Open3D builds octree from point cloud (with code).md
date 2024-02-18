#  Octree 

##  1. Build an octree 

>  Octree is a tree-like data structure used to describe three-dimensional space. Each node of the octree represents the volume element of a cube, and each node has eight sub-nodes. The volume elements represented by these eight sub-nodes are added together to equal the volume of the parent node. The general center point serves as the bifurcation center of the node. 

 ![avatar]( 20210522212717363.png) 

 The principle of octree construction: (1) Set the maximum recursion depth. (2) Find the maximum size of the scene and build the first cube with this size. (3) Throw the unit elements into the cube that can be contained and has no sub-node in sequence. (4) If the maximum recursion depth is not reached, subdivide it into eight equal parts, and then divide all the unit elements contained in the cube into eight sub-cubes. (5) If it is found that the number of unit elements assigned to the child cube is not zero and the same as the parent cube, then the child cube stops being subdivided, because according to the space division theory, the subdivided space must be allocated less. If the number is the same, then the number of cuts is still the same, which will cause infinite cuts. (6) Repeat 3 until the maximum recursion depth is reached.  

##  2. Main functions 

   Open3D open3d.geometry. Octree can be used to create, search, and traverse octree with a user-specified maximum tree depth max_depth. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574421144
  ```  
 Building an octree from a point cloud 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574421144
  ```  
#  III. Display of results 

 ![avatar]( 2021033021190590.jpg) 

