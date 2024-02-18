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

