# Green-to-Concrete_Ratio
  This project aims to use AI image Segmentation to analyze satellite or drone images and determine the green-to-concrete ratio in urban areas. We will identify and classify areas of vegetation and concrete, calculate their ratio for urban planning, and develop a method that can be easily applied to assess green spaces in cities.

# Project Journey 
Initially, we tried implementing the project using K-means clustering, but we got less accuracy. Then we moved to supervised learning, found data from aerial maps, and started labeling with three classes: buildings, roads, and white spaces. Later, we started working on TensorFlow UNet but could not detect proper boundaries, and we did not improve much because of the lack of time. So, for faster training, we moved to the YOLOv8 model.
But Below are code links if you are interested in improving

# implementation path 
K- means cluster - https://github.com/dharaniravanam/Green-to-Concrete_Ratio/tree/main/K-Cluster

Tensor Flow Unet - https://github.com/dharaniravanam/Green-to-Concrete_Ratio/tree/main/Tensor%20Flow%20UNet

Yolov8 - https://github.com/dharaniravanam/Green-to-Concrete_Ratio/tree/main/Yolov8_main

# guide to execution

# K-cluster :
Dataset: SAS.zip

Above SAS.zip is the dataset we used for cluster implementation. These are the images from the SAS Planet software. The remaining files are related to the code implementation of the K-mean Cluster.

# Tensor Flow Unet:
Dataset: Green to Concrete Ratio.v1i.tfrecord.zip

Above is the dataset by taking images from openaerialmap and then annotating images in roboflow. Then we downloaded data in the Tfrecord format as seen in the folder. The main file contains all the packages you need for the project implementation these packages can also be useful for the Yolo model. and then the code for training is present in the code file.

# YOLOv8_main:
dataset: Yolov8_main/Green-to-Concrete-Ratio-5.zip

The above is the same custom dataset we used for tensor flow but we have downloaded it in yolov8 format. You can also use the code for downloading this in Yolov8_main/mainyolov8.ipynb.
 And please do download yolov8s-seg.pt before starting with the training and then you can start the implementation of the code from Yolov8_main/mainyolov8.ipynb. I am not able to add any results to git as they are huge but you can use the youtube link to see them.

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
