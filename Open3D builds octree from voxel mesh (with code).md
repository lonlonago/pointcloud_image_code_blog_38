#  First, the main function 

##   1. Voxel grid 

   For voxel grids, see: voxelization of Open3D point clouds and triangulation networks 

##   2. Build an octree from a voxel grid 

   Function create_from_voxel_grid (voxel_grid) Constructs an octree from Open3D's VoxelGrid geometry. Each voxel entered into VoxelGrid is treated as a point in 3D space whose coordinates correspond to the origin of that voxel. Each leaf node takes the color of its corresponding voxel. 

##   3. Build a voxel grid from an octree 

   Function to_voxel_grid () converts octree to VoxelGrid 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574436484
  ```  
#  III. Display of results 

##   1. Primitive point cloud 

 ![avatar]( 20210407200155164.png) 

##   2. Voxel grid 

 ![avatar]( 20210407200218641.png) 

##   3. Octree 

 ![avatar]( 20210407200236750.png) 

##   4. Voxel grid 

 ![avatar]( 20210407200254936.png) 

