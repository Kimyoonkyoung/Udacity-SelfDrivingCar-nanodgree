[image1]: ./writeup_images/cannyedge.png "canny"
[image2]: ./writeup_images/houghline.png "hough"
[image3]: ./writeup_images/extrapolate.png "extra"
[image4]: ./writeup_images/result.png "result"

#**Finding Lane Lines on the Road** 

---
---

## Pipeline

###1. canny edge
before find canny edge, Gaussian Blur was performed.

![alt text][image1]

###2. hough line
And then, hough line transform performed on ROI.
 
![alt text][image2]

###3. make_singlelines
One representative line was extracted from the houghline.

* stabilize step
    * averaging slopes at each side
        * if (slope > 0) and (tan30 < slope < tan60) then left side
        * if (slope < 0) and (tan30 < slope < tan60) then right side
    * averaging intercepts at each side
    * compute the value of x. Using the above values

![alt text][image3]

###4. result
![alt text][image4]


## Shortcomings
1. limitations of parameters
    * The parameters are like blur, canny edge, hough lines, etc..
    * If the camera specifications are different, the parameters will also be very different

2. Stablize
    * It is not stable in noise, shadow, etc.

3. Curve
    * It is difficult to extract sharp curves.
    
## Improvement
I will need to use more abundant information throughout the video, rather than just looking for a line depending on the line..
