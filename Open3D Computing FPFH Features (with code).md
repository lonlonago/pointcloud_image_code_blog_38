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

