## DSM_Challenge_3

# 🚩 Social distancing detection

The main purpose of the Social Distancing Detection System is to enable the process of automating the task of monitoring social distancing using surveillance video. 

Since there are no proper vaccines available for covid-19 complete prevention, social distancing is the only feasible approach to fight against this pandemic.


## 🎥 Demo
 
#### After you run the last line of command,a `final_sdd_output.avi` file will be showing up in your directory like this:
![final_sdd_output.avi : ](https://github.com/saikumarreddykorsapati-source/DSM_Challenge_3/blob/main/Documentation/social%20distance%20detection.gif)

## 👨 Author

- [@saikumarreddykorsapati-source](https://github.com/saikumarreddykorsapati-source)



## 💻 Tech Stack

Python, Numpy, OpenCv, Yolov3, Scipy, CNN, Deepsort, Deeplearning Techniques 

## 📚 Documentation

(HLD) High Level Design : [Link - Click here...](https://github.com/saikumarreddykorsapati-source/DSM_Challenge_3/blob/main/Documentation/HLD_1.0v_Social_Distancing_Detection.pdf)

(LLD) Low Level Design : [Link - Click here...](https://github.com/saikumarreddykorsapati-source/DSM_Challenge_3/blob/main/Documentation/LLD_V01_Social_Distancing_Detection.pdf)

Wireframe : [Link - Click here...](https://github.com/saikumarreddykorsapati-source/DSM_Challenge_3/blob/main/Documentation/Wireframe_Doc_Social_Distancing_Detection_v01.pdf)

Architecture : [Link - Click here...](https://github.com/saikumarreddykorsapati-source/DSM_Challenge_3/blob/main/Documentation/Architecture_Social_Distancing_Detection.pdf)

(DPR) Detailed Project Report : [Link - Click here...](https://docs.google.com/presentation/d/19z3kfPl4pIk2pRyc5znnFydVfobt05TLQil4lpxf_CA/edit?usp=sharing)

As github wont allow us to store files more than 100mb : [Link - Click here to download yolo weights file...](https://drive.google.com/file/d/1YYzLD_hHiAWRmbr1ZzLNP0lBd1NUhrKz/view?usp=sharing)

# For GPU runtime:
You can find my google colab file here : [Social Distancing Detection DSM Challenge 3 colab link](https://colab.research.google.com/drive/16cKgO6UMKrJ2nHBWbL5mBKSimSCxzV_m?usp=sharing)

## Simple Theory
#### Object detection:

We will be using YOLOv3, trained on COCO dataset for object detection.
In general, single-stage detectors like YOLO tend to be less accurate than two-stage detectors (R-CNN) but are significantly faster.
YOLO treats object detection as a regression problem, taking a given input image and simultaneously learning bounding box coordinates and corresponding class label probabilities.
It is used to return the person prediction probability, bounding box coordinates for the detection, and the centroid of the person.

#### Distance calculation:

NMS (Non-maxima suppression) is also used to reduce overlapping bounding boxes to only a single bounding box, thus representing the true detection of the object. Having overlapping boxes is not exactly practical and ideal, especially if we need to count the number of objects in an image.
Euclidean distance is then computed between all pairs of the returned centroids. Simply, a centroid is the center of a bounding box.
Based on these pairwise distances, we check to see if any two people are less than/close to 'N' pixels apart.

## ⌛ FAQ

#### What is Yolo v3?
- YOLOv3 (You Only Look Once, Version 3) is a real-time object detection algorithm that identifies specific objects in videos, live feeds, or images. YOLO uses features learned by a deep convolutional neural network to detect an object.
#### What is Euclidean Distance?
- Euclidean Distance represents the shortest distance between two points. Most machine learning algorithms including K-Means use this distance metric to measure the similarity between observations.
#### What is Opencv ?
- OpenCV (Open Source Computer Vision Library) is an open source computer vision and machine learning software library.
#### What is social distance detection ?
- The detection tool was developed to alert people to maintain a safe distance with each other by 
  evaluating a video feed.


