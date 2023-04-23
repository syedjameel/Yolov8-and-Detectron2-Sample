# Yolov8 and Detectron2 on Sample dataset

# Task: 
1. Take photos of your environment of two or more objects. (at least 100 instances between all objects) 

2. Annotate them on Roboflow for segmentation. 

3. Train a Mask RCNN model using detectron2

4. Train Yolov8  the smallest size for segmentation

5. Evaluate both models based on mAP and speed and size.

# 1. Take photos

5-Objects pictures were taken. 1. 7-segment-display, 2. buzzer, 3. connector, 4. push-button, 5. ultrasonic-sensor

7-segment-display image :
<p align = "center">
<img src = "images/raw_images/7-segment-display.jpg" height = "240px" style="margin:10px 10px">
</p>

buzzer image:
<p align = "center">
<img src = "images/raw_images/buzzer.jpg" height = "240px" style="margin:10px 10px">
</p>

connector image:
<p align = "center">
<img src = "images/raw_images/connector.jpg" height = "240px" style="margin:10px 10px">
</p>

push-button image:
<p align = "center">
<img src = "images/raw_images/push-button.jpg" height = "240px" style="margin:10px 10px">
</p>

ultrasonic-sensor image:
<p align = "center">
<img src = "images/raw_images/ultrasonic-sensor.jpg" height = "240px" style="margin:10px 10px">
</p>

# 2. Annotate them on Roboflow for segmentation.
<p align = "center">
<img src = "images/raw_images/roboflow.png" height = "240px" style="margin:10px 10px">
</p>

# 3. Train a Mask RCNN model using detectron2
<p align = "center">
<img src = "images/detectron2/mAP_detectron2.png" height = "240px" style="margin:10px 10px">
</p>

# 4. Train Yolov8  the smallest size for segmentation
<p align = "center">
<img src = "images/yolov8/mAP_yolov8.png" height = "240px" style="margin:10px 10px">
</p>

- confusion matrix
<p align = "center">
<img src = "images/yolov8/confusion_matrix.png" height = "240px" style="margin:10px 10px">
</p>

- Losses
<p align = "center">
<img src = "images/yolov8/loss.png" height = "240px" style="margin:10px 10px">
</p>



# 5. Evaluation
### Mean Average Precision (mAP)
- Yolov8: 99.5%
- Detectron2: 62.112%


### Training speed:
Yolov8 trained in ~6 minutes for 20 epochs even thought it is very light weight compared to detectron2 model 
Detectron2 trained in ~20 minutes

### Size:
- The Yolov8 model size: 92.3 Mb
- Detectron2 model size: 805.5 Mb


# References
1. https://roboflow.com/

# Train Yolov8 COLAB Link: [Yolov8](https://colab.research.google.com/drive/13H6rnO3aT0QXi7EgoBBDoX4ekV3oFfaR?usp=sharing)

# Train Detectron2 COLAB Link:[Detectron2](https://colab.research.google.com/drive/1MExbPGe4skrWXtkvHgl6eNaY4Tolm3L-?usp=sharing)