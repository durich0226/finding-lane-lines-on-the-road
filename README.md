# finding-lane-lines-on-the-road
Project 1

Finding Lane Lines on the Road

Reflection:
1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.
In this project, Python3 and OpenCV are used to detect the lane lines on the road. The procedure for this project is as following:

    1) transformation to grayscale
    
    2) image smoothing using Gaussian filter
    
    3) edge detection using Canny detector
    
    3) adding lanes to edges image
    
    4) excluding everything out of region of interest's polygon
    
    5) applying hough transformation
    
    6) combining initial image with results

2. Identify potential shortcomings with your current pipeline

One shaortcoming for this project is that detecting lines for curved lanes seem oscillate with a relative larger magnitude in vertical direction. 

3. Suggest possible improvements to your pipeline

In most of the cases excluding the continous curved lanes, different set of parameters can mask the lane lines well. But it seems more advanced algorithm or methodology should be used in optimising the curved lanes. 
