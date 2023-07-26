# Tropical Fish Object Detection using Ultralytics YOLOv8n

*This project focuses on the detection of five different types of tropical fish (Neon Tetra, Siamese Flying Fox, Ember Tetra, Rummy Nose Tetra, and African Lampeye) from video footage using the YOLOv8 architecture. I have provided a demo video on Youtube, below:*
[![Tropical Fish Object Detection using Ultralytics YOLOv8n](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*k6SX9CvQhLlIBC8qSC9MHw.jpeg)](https://www.youtube.com/watch?v=8jPV7NW326w "[Youtube] Detecting Tropical Fish using Ultralytics YOLOv8n")
- *Demo Video: [https://www.youtube.com/watch?v=fuQepYj_ml0](https://www.youtube.com/watch?v=fuQepYj_ml0)*
- *Full Article: [Tropical Fish Object Detection using Ultralytics YOLOv8n](https://medium.com/@yohmori/real-time-tropical-fish-detector-using-yolov8-f6cd78019f5e)*


## 1. Introduction
In this project, I leverage YOLOv8n to detect five types of tropical fish in real time (both video footage and realtime camera feed). YOLOv8 is a popular state-of-the-art object detection framework by Ultralytics. YOLOv8 follows a multi-scale approach, enabling it to capture objects at different scales and resolutions. For this object detection, I used the YOLOv8 architecture with n scaling. The n scale refers to the size of the Neural Network, where n is the smallest and fastest type.

## 2. Files
- **01_compress.ipynb:** You are bound to find images that are very large in file size. This code compresses any large images.
- **02_move_files:** After using CVAT, you must move images to the images file and labels to the labels file. Furthermore, you should split the data into train and validation. This file does that for you.
- **03_train_model:** Given trained model, trains model and outputs to runs/detect/< here >
- **04_predict.ipynb:** Give test video in data/test_video, predicts and outputs new video in the same directory. You may change the confidence level depending on your preference.
- **05_realtime_predict.ipynb:** Predict using your PC camera. Predicts using live/real-time camera feed
- **config.yaml:** You may specify the exact location of your train and validation datasets. You may also change the classes to be predicted. Here, I have the 5 fish types.
- **data/:** Images and CVAT coordinates for training and validation. Currently has 1000 training images and 300 validation images, with thousands of instances labeled.