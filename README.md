# vSLAM

## Installation requirements

download [iriun webcam](https://iriun.com/) on both phone and pc.

```pip install opencv-python```

## FAST (Features from Accelerated Segment Test) Algorithm

#### FAST algorithm
- Choose one pixel and let $I_p$ be its pixel value and let $t$ be the threshold value.
- Create a Bresenham circle of radius 3 around the pixel
- Check if there are 3 or more pixels from pixels 1, 5, 9, 13 with pixel value greater than $I_p+t$ or 3 or more pixels with pixel values less than $I_p-t$
- Check if there are 12 or more pixels from the circle with a pixel value greater than $I_p+t$ or 12 or more pixels with pixel values less than $I_p-t$
- Append to a list of corners
- Repeat for all pixels of the image

<div style="width:400px ; height:400px">
     
     ![image](https://github.com/alexmrin/vSLAM/assets/131604147/0f856173-c817-424c-8ee2-c41678a8aa88)

     
<div>


### Corner detection vs. threshold

<img
     src = "/fastexperiment/fastcorner_threshold(5).jpg"
     alt = "threshold5"
     title = "Fast Coner Detection (threshold = 5)"
     width = "300"
     height = "300">
<img
     src = "/fastexperiment/fastcorner_threshold(10).jpg"
     alt = "threshold10"
     title = "Fast Coner Detection (threshold = 10)"
     width = "300"
     height = "300">
<img
     src = "/fastexperiment/fastcorner_threshold(15).jpg"
     alt = "threshold5"
     title = "Fast Coner Detection (threshold = 15)"
     width = "300"
     height = "300">
<img
     src = "/fastexperiment/fastcorner_threshold(20).jpg"
     alt = "threshold5"
     title = "Fast Coner Detection (threshold = 20)"
     width = "300"
     height = "300">
<img
     src = "/fastexperiment/fastcorner_threshold(25).jpg"
     alt = "threshold5"
     title = "Fast Coner Detection (threshold = 25)"
     width = "300"
     height = "300">
<img
     src = "/fastexperiment/fastcorner_threshold(30).jpg"
     alt = "threshold5"
     title = "Fast Coner Detection (threshold = 30)"
     width = "300"
     height = "300">
