# Image-tagging-and-road-object-detection
Building a YOLO Model for Object detection in a video

# Problem Statement
In this project we will recognize and detect different objects present in an image or video and label them to classify the objects. Some of the most sought-after research areas in computer vision applications are real-time object tracking.Despite great advances in this field, achieving significant precision and efficacy in tracking objects in real time remains a big issue.

# Project Description
Existing driving datasets are limited in terms of visual content, scene diversity, annotation richness, geographic distribution, and supported tasks, making it difficult to research multitask learning for autonomous driving. Yu et al. published BDD100K, the world's largest driving video dataset, including 100K movies and ten challenges, in 2018 to assess the advancement of image recognition algorithms in autonomous driving. Geographic, environmental, and weather diversity are all present in the dataset, which is important for training models that are less likely to be startled by unexpected situations. For "other vehicle," "pedestrian," "traffic light," "traffic sign," "truck," "train," "other person," "bus," "car," "rider," "motorcycle," "bicycle," and "trailer," there are bounding box annotations of 13 categories for each of the reference frames of 100K videos and 2D bounding boxes annotated on 100.000 images.

Our project's purpose is to use two ways to recognise and classify traffic items in a video in real time. On the Berkeley DeepDrive dataset, we trained the two state-of-the-art models YOLO and Faster R-CNN to compare their performances and attain a similar mAP to the present state-of-the-art on BDD100K, which is 45.7 using a hybrid incremental net. We'll compare the models' performance on a live video while measuring FPS and mAP in the context of autonomous driving.
