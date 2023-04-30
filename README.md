# RoadSignDetection

Live Demo Link: https://youtu.be/RIfUsiInJf8
Presentation Link: https://docs.google.com/presentation/d/1wTwnWInB-suYqqb9yOQRB8C-GE_f8bLLGntWDE2JnRg/edit?usp=sharing

# Abstract
This report presents the development and evaluation of a machine learning model for road sign detection.
The model was trained using the Single Shot Multibox Detector (SSD) architecture and the TensorFlow
Object Detection API. A dataset of 100 road sign images, consisting of 5 categories (Stop, Yield, Danger,
Deadend, and Parking), was collected and manually labeled. The dataset was split into a training set of 90
images and a testing set of 10 images.
The labeled dataset was preprocessed using Python scripts, and the SSD model was trained using the
Stochastic Gradient Descent (SGD) optimizer with a batch size of 4, a learning rate of 0.079999, and a total
of 10,000 training steps. The model achieved an average precision (AP) of 0.89 and an average recall (AR)
of 0.900 on the testing set.
The model was evaluated using precision and recall metrics on the testing set, and it correctly predicted all
road signs in the images except for one, where it misclassified a turn sign as a parking sign. The model’s
performance can be further improved by collecting more images of the parking sign category.
Overall, the developed machine learning model for road sign detection achieved high accuracy and can be
further improved with more data and training. The model has the potential to be integrated into real-world
applications for driver assistance and safety.

# Introduction
Road signs play an important role in ensuring safety on the roads. The ability to detect and recognize road
signs is a crucial aspect of autonomous driving, which has the potential to greatly reduce the number of road
accidents caused by human error. In recent years, object detection has become a popular field of research,
and many different models have been developed to accurately detect objects in images and videos.
One such model is the Single Shot Detector (SSD), which has been shown to achieve state-of-the-art results
in object detection tasks. The SSD model is a type of convolutional neural network (CNN) that is capable
of detecting objects at different scales and aspect ratios, making it well-suited for detecting road signs of
various sizes and shapes.
In this project, we aim to apply the SSD model to the task of road sign detection. Specifically, we will train
the model on a dataset of labeled road sign images and evaluate its performance on a separate test set.
Overall, we believe that the SSD model has great potential for improving the safety of autonomous driving
systems by enabling them to accurately detect and recognize road signs. By using advanced computer vision
techniques such as object detection, we can take important steps towards a future where roads are safer for
everyone.

# Background
Road sign recognition is an essential task for safe driving. With the advancement of computer vision technologies, it is possible to automate road sign recognition with the help of object detection models. This
project aims to explore the potential of using the Single Shot Multibox Detector (SSD) model to detect road
signs in real-time.
Being able to identify road signs with object detection could benefit drivers and road users in different ways.
Contemporary vehicles nowadays typically incorporate several cameras installed from different parts of the
vehicle body. These peripherals, together with the relevant objection and motion detection solution, enable
and empower the delivery of some creative value-added features such as 360-bird-eye-view parking view,
lane-deviation and lane-changing warning, and collision warning, among others.
The use of such technologies could make driving safer and more convenient for drivers. Imagine a road
condition with low visibility due to weather and night-time or a situation where the driver has demonstrated
a certain level of fatigue during driving or is driving on an unfamiliar road. If there is a device or vehicle
feature that could detect crucial road signs (e.g., speed limit, rail crossing, construction, etc.) and give
appropriate warnings to the drivers, it may potentially reduce traffic accidents and casualties.
While object detection has shown promising results in various applications, it still faces several challenges,
especially in road sign detection. One of the primary issues is the diversity of road signs. Road signs can have
different shapes, sizes, and colors, and can be partially occluded, rotated, or distorted. Therefore, training
a model that can recognize all types of road signs is a challenging task.
Another issue is the real-time performance of the model. Road sign detection should be done in real-time
to ensure timely warnings to the driver. Hence, the model should be optimized to provide accurate results
while being computationally efficient.
This project is therefore tasked to carry out a preliminary study of potentially useful and applicable models,
evaluate and assess the performance and accuracy of the resulting model. Due to the project scope and
timeframe, we have focused on a few most commonly selected road signs. We hope that our findings could
provide a good starting point and shed some light on the readiness and feasibility of the road sign detection
idea, its effectiveness, application constraints and considerations, and its generalization possibilities.
![image](https://user-images.githubusercontent.com/61757423/235373476-e7a7de14-6a41-4539-9962-9eaadcc63322.png)
![image](https://user-images.githubusercontent.com/61757423/235373495-79b955ec-c6f9-48dd-a77b-8d182639876d.png)
![image](https://user-images.githubusercontent.com/61757423/235373466-8d912ce7-76dc-4e2a-bc0e-97016fbcb0e2.png)
