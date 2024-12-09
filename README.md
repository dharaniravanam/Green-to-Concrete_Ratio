# Green-to-Concrete_Ratio
  This project aims to use AI image Segmentation to analyze satellite or drone images and determine the green-to-concrete ratio in urban areas. We will identify and classify areas of vegetation and concrete, calculate their ratio for urban planning, and develop a method that can be easily applied to assess green spaces in cities.

# Project Journey 
Initially, we tried to implement the project using K-means clustering, but we got less accuracy. Then we moved to supervised learning, found data from aerial maps, and started labeling with three classes: buildings, roads, and white spaces. Later, we started working on TensorFlow UNet but were unable to detect proper boundaries, and we did not improve much because of less time. So, for faster training, we moved to the YOLOv8 model.
But Below are code linking if you are interested to improve

# implementation path 
K- means cluster - https://github.com/dharaniravanam/Green-to-Concrete_Ratio/tree/main/K-Cluster

Tensor Flow Unet - https://github.com/dharaniravanam/Green-to-Concrete_Ratio/tree/main/Tensor%20Flow%20UNet

Yolov8 - https://github.com/dharaniravanam/Green-to-Concrete_Ratio/tree/main/Yolov8_main

# guide to execution

# K-cluster :
dataset: SAS.zip

Above SAS.zip is the dataset we used for cluster implementation. These are the images from SAS Planet software. Remaining files are related to the code implementation of K-mean Cluster.

# Tensor Flow Unet:
dataset: Green to Concrete Ratio.v1i.tfrecord.zip

above is the dataset by taking image from openaerialmap and then annotated image in roboflow. Then we downloaded data in the Tfrecord format as seen in folder. and the main file contains all packages you need for the project implementation these packages can also be useful for yolo model also. and then the code for training is present in code file.

# YOLOv8_main:
dataset: Yolov8_main/Green-to-Concrete-Ratio-5.zip

The above is the same custom dataset we used for tensor flow but we have dowloaded in yolov8 format. you can also use code for downloading this in Yolov8_main/mainyolov8.ipynb.
 and please do dowload yolov8s-seg.pt before starting with the training and then you can start implemtation with is present in Yolov8_main/mainyolov8.ipynb. i am not able to add any results to git as then are huge but you can use youtube link to see them.

# our Results
![image](https://github.com/user-attachments/assets/216aaae3-6097-4f75-ae1a-8ff8cdb2f2bb)

![image](https://github.com/user-attachments/assets/74724b6b-049d-452c-b2ad-bb9f28c9d360)

Know more about our work follow the links:

# Our dataset: 
https://app.roboflow.com/green-to-concrete-ratio

# Code we used: 
https://github.com/dharaniravanam/Green-to-Concrete_Ratio

# Want to try it yourself?
Get free aerial images to create your dataset: 
https://openaerialmap.org/

# YouTube 
https://youtu.be/hJ8ItimqNGo?si=vGf1NwpMsie_a666

# Learn about YOLOv8:
Find out how it works here: 
https://docs.ultralytics.com/datasets/segment/#ultralytics-yolo-format
