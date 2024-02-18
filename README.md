#  I. Introduction 

##  1. Coordinate system 

 ![avatar]( 20210530101747906.jpg) 

   create_coordinate_frame () function adds a three-dimensional coordinate axis of red, green and blue to the visualization window, red is the X axis, green is the Y axis, blue is Z, and the Z direction is pointing to the screen. Open3D uses a right-hand three-dimensional coordinate system.  

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574446158
  ```  
 Create a coordinate system frame. The coordinate system is centered on origin. The x, y, and z axes will appear as red, green, and blue arrows, respectively. 

#  Code implementation 

 Method one 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574446158
  ```  
 Method 2, see: Open3D custom visualization background color and dot size 



--------------------------------------------------------------------------------

#  Introduction to the algorithm 

##  1. Overview 

   Calculate the Mahalanobis distance from each point to the nearest neighbor, and finally render the color according to the Mahalanobis distance.    

##  2. Main functions 

   compute_mahalanobis_distance function in Open3D calculates the Mahalanobis distance from each point to its nearest neighbor. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574436593
  ```  
#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574436593
  ```  
#  III. Display of results 

 ![avatar]( 7d61818a8b074cbebb1de65e6019c3d8.png) 



--------------------------------------------------------------------------------

Integral image is a method for estimating the discovery of ordered point clouds. The algorithm takes the point cloud as a depth image and creates a certain rectangular area to calculate the normal, taking into account the adjacent pixel relationship without establishing a tree query structure. Therefore, it is very efficient. 

 Code display: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574490079
  ```  
 Effect display: 

 ![avatar]( 20201226184558177.png) 



--------------------------------------------------------------------------------

##  Function prototype 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574471487
  ```  
##  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574471487
  ```  
##  III. Display of results 

 ![avatar]( 20210317093347688.png) 

##  C++ version code 

 Normalized Covariance Matrix and Three-Dimensional Centroid of PCL Point Cloud 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##   1. Overview of the principle 

    Alpha-shape is a generalization of the convex hull algorithm. One can intuitively think of alpha-shape as follows: Imagine a large piece of ice cream containing dots of S chocolate chunks. Using one of these spherical ice cream spoons, we can cut out all the parts of the ice cream chunks, and we can dig holes inside without touching the chocolate chunks (e.g., parts that cannot be reached by just moving the spoon from the outside). We end up with a (not necessarily convex) object, which consists of vertices, arcs, and points. If we now straighten all the round faces into triangles and line segments, we can visually describe the so-called alpha shape. 

##   2. Function analysis 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957449087
  ```  
 Implementing this method in Open3D requires attention to the following two points: 

##   3. References 

>  [1] H.Edelsbrunner and D. G. Kirkpatrick and R. Seidel: On the shape of a set of points in the plane, IEEE Transactions on Information Theory, 29 (4): 551–559, 1983 [2]Alpha shapes 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957449087
  ```  
#  III. Display of results 

 ![avatar]( 20210620195317219.png) 

 ![avatar]( 2020120221295659.png) 

 alpha=0.030  alpha=0.500  alpha=0.136  alpha=0.037  alpha=0.010  

#  C++ code 

 Open3D a-shape surface reconstruction 



--------------------------------------------------------------------------------

#  I. Overview of algorithms 

##  1. Achieve the effect 

 ![avatar]( 860cf8aa54c34eafadfe07917e9aa81c.png) 

##  2. Overview of the principle 

   The implementation process is relatively simple, see the code Linearity.py. 

#  Code implementation 

##  1、main.py 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574470702
  ```  
##  2、Linearity.py 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574470702
  ```  
#  III. Display of results 

 ![avatar]( 5b785fb82f9446a2abfa6ccb2a9fd74a.png) 

#  IV. Test data 

 Link: https://pan.baidu.com/s/1Dd5JkJkZToXlen09VX9rrg Extraction code: cnaf 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Projection density theory and method 

 ![avatar]( 288f96df99374c7bbc708ec89f39a5f8.png) 

    The 3-dimensional coordinate points are directly projected vertically onto the horizontal plane or the value is taken as an arbitrary constant to count and calculate the number of projection points contained at any position on the horizontal plane as (Density of Projected Points). In an ideal state (the target surface is smooth, unobstructed, and all sampling points are valid points), the value is related to the height of the target, the vertical distance from the center of the scanner to the target, and the spatial resolution of the scanner. To simplify the calculation, the measurement area can be divided into regular grids, the grid is uniformly numbered, and the number of projected points on each grid unit is counted and this value is used as the value of the grid unit. This way, the value can be expressed discretely. Values have the following characteristics:  

 1. On the ground, the value is relatively uniform and relatively small as a whole; 2. At the boundary of the building (the gray area in the figure), the value is much larger than that of other areas and forms a continuous band; 3. Inside the building, if the noise is removed, the impact value is 0; 4. Independent point-like features, such as lamp posts, have larger local values and smaller surrounding values; 5. Block-like features, such as trees and cars, are locally larger and occupy a certain area. When the grid area increases to a certain value, the block-like features have the same characteristics as the independent point-like features. Using the above characteristics and selecting a reasonable threshold, the point cloud can be divided according to the following formula:  

##  2. References 

>  Shi Wen, Li Bijun, Li Qingquan. Image segmentation method of vehicle laser scanning distance based on projection point density [J]. Chinese Journal of Surveying and Mapping, 2005 (02): 95-100. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957443673
  ```  
#  III. Display of results 

 ![avatar]( 7518115a5e734e4aa921061bad77705d.jpeg) 

 primordial point cloud  

 ![avatar]( d75738f2f84741758e7d3917c4a7f49f.jpeg) 

 extract result  



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

   In the building point cloud, there is obvious difference between the normal vector of the elevation point and the normal vector of the plane point, and the segmentation of the elevation point and the plane point can be realized by setting the corresponding threshold according to the component of the normal vector in the Z direction. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957443580
  ```  
#  III. Display of results 

 ![avatar]( ef315511dd7341cf96d6450a380d701c.png) 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  First, the code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574419261
  ```  
#  III. Display of results 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574419261
  ```  


--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Formula method 

 ![avatar]( a2663d42c97b4fac99212f113cdd1067.png) 

##  2. Derivation process 

 见：Point-Line Distance–3-Dimensional 

##  3. Triangle method 

 ![avatar]( be9d4ad4e834470b884c3f03ef0d65ef.png) 

  Helen's formula.  

#  Code implementation 

##  1. Formula method 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574478392
  ```  
##  2. Triangle method 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574478392
  ```  
#  III. Display of results 

##  1. Formula method 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574478392
  ```  
##  2. Triangle method 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574478392
  ```  


--------------------------------------------------------------------------------

#  Introduction to the algorithm 

##  1. Overview 

   First, use K-nearest neighbor search to find the nearest neighbor of each point, then calculate the Euclidean distance from each point to the nearest neighbor, and finally color render according to the distance. 

##  2. Main functions 

   compute_nearest_neighbor_distance function in Open3D calculates the Euclidean distance from each point to its nearest neighbor. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574453029
  ```  
##  3. Algorithm source code 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574453029
  ```  
#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574453029
  ```  
#  III. Display of results 

 ![avatar](4423252f282d4b748018bc29a0e78c30.png) 

#  IV. Python detailed process version 

 The code in this article is the Python implementation of the above source code. 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Calculation formula 

    Where, is the length of the three sides of the triangle and the area of the triangle. Can be obtained by Helen's formula. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574429215
  ```  
#  III. Display of results 

 The three points in the code example are relatively simple: you can verify it orally. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574429215
  ```  


--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Algorithm overview 

   SelectionPolygonVolume (__pybind11_builtins pybind11_object): class in Open3D, which realizes the cropping function of point cloud and model, but because the example code given by the official website is to read the cropping range from the json file, the use of the json file restricts the application scope of the algorithm to a certain extent. This article gives the code usage method without json file. 

##  2. JSON content 

   The content written in the JSON file is as follows: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574473842
  ```  
   It mainly includes the vertex coordinates and axis value range of any clipping area. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574473842
  ```  
#  III. Display of results 

##  1. Primitive point cloud 

 ![avatar]( 9f67c851a59d4ef78c63efb01a7acfb0.png) 

##  2. Crop the result 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574473842
  ```  
 ![avatar]( 9be63c6b85c34876bfc05c13197cd071.png) 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

 Test data: Open3D color point cloud registration test data ColoredICP.rar 

##  1. Overview of the principle 

>  Colored point cloud registration【配准论文解读】Color Point Cloud Registration with 4D ICP Algorithm 

##  2. Code analysis 

>  Open3d Learning Project - Advanced Part 2 (Color Point Cloud Registration) Color Point Cloud Registration for Open3d 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574450556
  ```  
#  III. Display of results 

 ![avatar]( 20210202211856363.png) 

 1. Initial position 2. Point-to-plane registration result 3. Color point cloud registration result   



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Calculation formula 

   For any point in the point cloud data, calculate its covariance matrix according to the coordinates of the points in its neighborhood. The calculation formula is as follows:  

   Where is the neighborhood point, which is the neighborhood point and the centroid of the point. 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574414137
  ```  
##  3. Function source code 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574414137
  ```  
#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574414137
  ```  
#  III. Display of results 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574414137
  ```  


--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Overview of the principle 

   Mean, variance, and standard deviation in statistics. 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574497865
  ```  
 Calculates the arithmetic mean along the specified axis. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574497865
  ```  
   Calculates the variance along the specified axis. Returns the variance of an array element, which is a measure of the distribution. By default, the variance is calculated for a flattened array, otherwise it is calculated on the specified axis. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574497865
  ```  
   Calculates the standard deviation along the specified axis. Returns the standard deviation of an array element, which is a measure of the distribution distribution. By default, the standard deviation is calculated for flattened arrays, otherwise it is calculated on the specified axis. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574497865
  ```  
#  III. Display of results 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574497865
  ```  
#  C++ version 

 PCL Calculation Point Cloud Mean and Standard Deviation 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Overview of the principle 

##  2. Specific process 

 ![avatar]( 20210529115939219.png) 

   Assuming that there are points in the three-dimensional point cloud, the complexity of computing the feature histogram is to represent the number of points within the neighborhood radius of any query point in the point cloud data. In practical applications, due to the large number of point cloud data points, it usually takes a long time to calculate the feature histogram of the point cloud. In order to improve the computational efficiency, simplify the process and reduce the complexity of the algorithm, an algorithm is proposed. The main flow of the algorithm is as follows: (1) For each point required, calculate a group between the point and its neighborhood points. The result of this step is called a simplified feature histogram. (2) Re-determine the neighborhood points of each point, and use the neighboring ones to calculate the final histogram (called). The formula is as follows: In Equation (6), the weight is expressed, which is measured according to the distance between the points within its neighborhood. Figure 3 helps us understand this weighting method.  

   In Figure (3), it can be seen that the algorithm is mainly divided into two steps. First, for any query point, the calculated value is based only on the corresponding point pair between its neighbor points (the red line segment in Figure 3). The second step is to calculate the weighted values of the nearest neighbor points (,,, and in Figure 3) and accumulate them. The accumulated results are obtained by adding the SPFH values. In summary, the algorithm is based on the algorithm, and there are differences between them, mainly in the following aspects: (1) The algorithm does not connect all points in the neighborhood of the query point, so there is a possibility of losing some values, and these values may have some clear geometric characteristics; (2) The scope of the algorithm is only within the neighborhood radius of the query point, and the algorithm includes not only the neighborhood range with the center radius, but also the radius r centered on the adjacent points; (3) Different from the descriptor, it divides each dimension into 11 intervals and counts the number of points on each dimensional interval, thus replacing the way of dividing the entire high-latitude space and superimposing only on three dimensions, so that the final description The sub has only 33 dimensions, which greatly reduces the dimension of the descriptor; (4) Compared with the sub, the overall complexity is greatly reduced and the calculation speed is faster, so it has high real-time application value. 

##  3. References 

>  [1] Rusu, Radu Bogdan, Nico Blodow, and Michael Beetz. "Fast point feature histograms (FPFH) for 3D registration." In 2009 IEEE International Conference on Robotics and Automation, pp. 3212-3217. IEEE, 2009. [2] Han Yifei, Yang Ziqian, Zheng Fu, Wang Yanqiu, Sun Zhibin. Improved point cloud registration algorithm based on FPFH and normal vector [J/OL]. Semiconductor optoelectronics: 1-6 [2021-08-26]. https://doi.org/10.16818/j.issn1001-5868.2021.04.001. 

#  Code implementation 

##  1. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574416985
  ```  
##  2. Complete code 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574416985
  ```  
#  III. Display of results 

>  Open3D doesn't seem to support histogram visualization. Here are the histogram visualization results of matlab 

 ![avatar]( f104d70a7b634718b08ebb3610d2adda.png) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

   Different sampling devices and different distances from the scene will cause differences in point cloud density. Existing methods for estimating point cloud density include distance-based methods and block-based methods. The distance-based average distance density representation is to estimate the distribution density of point clouds by calculating the average distance of each point in the point cloud. The distance of the point is generally a certain point in the point cloud 

     The larger d is, the sparser the point cloud distribution and the smaller the density. Therefore, it is feasible to estimate the point cloud density by the average distance. 

##  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461813
  ```  
##  III. Display of results 

 ![avatar]( 20210302195807773.png) 

##  C++ version of the calculation results 

 ![avatar]( 20210302200048192.png) 

  Consistent result 



--------------------------------------------------------------------------------

