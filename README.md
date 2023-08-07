# Vehicle Detection & Tracking using YOLOV7::::
Abstract :The importance of real-time vehicle detection tracking and counting system based on YOLOv7 is an important tool for monitoring traffic flow on highways. Highway traffic management, planning, and prevention rely heavily on real-time traffic monitoring technologies to avoid frequent traffic snarls, moving violations, and fatal car accidents. Three crucial duties include the detection, tracking, and counting of cars on urban roads and highways as well as the calculation of statistical traffic flow statistics (such as
determining the real-time vehicles flow and how many different types of vehicles travel). Important phases in these systems include object detection, tracking, categorizing, and counting. The YOLOv7 identification method is presented to address the issues of high missed detection rates of the YOLOv7 algorithm for vehicle detection on urban highways, weak perspective perception of small targets, and insufficient feature extraction. This system aims to provide real-time monitoring of vehicles, enabling insights into traffic patterns and facilitating informed decision-making. In this Model, vehicle detecting, tracking, and counting can be calculated on
real-time videos based on modified YOLOv7 with high accuracy.

Requirnments : IDLE: Google Colab to run notebook on GPU..
               Annotations tool : LabelImg

Steps to run the code: For Vehicle Detection...
1. clone the respository  https://github.com/WongKinYiu/yolov7.git

2.Go to Cloned Folder:  %cd /content/yolov7

3.Install the Required Dependies:  pip install -r requirements.txt

4.Download the weights file from the respository: https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt

5.Test the weights of YOLOV7.pt with  the sample images which is stored with YOLOV7 folder:  

! python /content/yolov7/detect.py --weights /content/yolov7.pt --conf 0.25 --img-size 640 --source /content/yolov7/inference/images/zidane.jpg

6. Train the Yolov7 code with our custom dataset: 1) create custom yaml file..
                                                  2) upload the custom yaml in Yolov7/ data folder..

7.Test the our own vedios with Trained weights...

! python /content/yolov7/detect.py  --source /content/yolov7/inference/images/ScooterCar.mp4 --weights /content/yolov7/runs/train/vehicledetection2/weights/best.pt --conf 0.25 --name Vehicledetection

8.Results:

resulted vedio uploaded in above E:\Protfolio Projects\Machince Learning\Vehicle Detection and Tracking\vehicle detection & Tracking\Result vedios

               