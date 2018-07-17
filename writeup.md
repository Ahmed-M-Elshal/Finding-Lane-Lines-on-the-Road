# **Finding Lane Lines on the Road** 


---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### The following techniques are used:

* Color Selection
* Canny Edge Detection
* Region of Interest Selection
* Hough Transform Line Detection


My pipeline consisted of 6 steps. First, I select only white and yellow colors in the input images using the RGB channels, then I convert images into gray scaled ones in order to detect shapes, in addation to that i used Gaussian Blur to make the edges smoother because the pixel intensity changes rapidly.


In order to draw a single line on the left and right lanes, I used canny Edge Detection algorithim to detect the edges on images and applying Region of Interest Selection mask to select the region of interestd lane lines, then I used Hough Transform Line Detection to detect lines in the edge images.


If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when there are no lain lines or there color is changed.

Another shortcoming could be founed where there curves on the road.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to detect any lain line one the road.

Another potential improvement could be to make Hough Transform detect the curves on the road.
