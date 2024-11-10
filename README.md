# Football Analysis Project

## Introduction
The goal of this project is to detect and track players, referees, and footballs in a video using YOLO, one of the best AI object detection models available. We will also train the model to improve its performance. Additionally, we will assign players to teams based on the colors of their t-shirts using Kmeans for pixel segmentation and clustering. With this information, we can measure a team's ball acquisition percentage in a match. We will also use optical flow to measure camera movement between frames, enabling us to accurately measure a player's movement. Furthermore, we will implement perspective transformation to represent the scene's depth and perspective, allowing us to measure a player's movement in meters rather than pixels. Finally, we will calculate a player's speed and the distance covered. This project covers various concepts and addresses real-world problems, making it suitable for both beginners and experienced machine learning engineers.

![Screenshot](output_videos/screenshot.png)

## Modules Used
The following modules are used in this project:
- YOLO: AI object detection model
- Kmeans: Pixel segmentation and clustering to detect t-shirt color
- Optical Flow: Measure camera movement
- Perspective Transformation: Represent scene depth and perspective
- Speed and distance calculation per player

## Trained Models
- [Trained Yolo v5](https://drive.google.com/file/d/1DC2kCygbBWUKheQ_9cFziCsYVSRw6axK/view?usp=sharing)

## Sample video
-  [Sample input video]([https://drive.google.com/file/d/1t6agoqggZKx6thamUuPAIdN_1zR9v9S_/view?usp=sharing](https://drive.google.com/file/d/11FHKzJoATnOR_rF5-rU3mmul1X7KqJGX/view?usp=sharing))

## Output video
-   [Output video]([[https://drive.google.com/file/d/1t6agoqggZKx6thamUuPAIdN_1zR9v9S_/view?usp=sharing](https://drive.google.com/file/d/11FHKzJoATnOR_rF5-rU3mmul1X7KqJGX/view?usp=sharing)](https://drive.google.com/drive/folders/1FN0pP2imafIyNgGUM2p4n-bvdqxn-IsK?usp=sharing))


## Sequential Steps:-
- [Sequential steps]
1.	Trained Simply for object detection on the Yolov8 auto detection.
2.	Trained for object detection using the data set available on the Roboflow and then used that outcome for more clear object detection.
3.	Tracking of the players and other entities across different frames using the next bounding box and previous bounding box using OpenCV (also based on the basis of the t-shirt colour across different frames).
4.	Show the players in the circle and the color of the tracked circle.
5.	Assigning the Marker on the each of the player who gets the ball
6.	Team ball Acquisition analysis
7.	Player bounding box movement with the camera movement(like zoom and left and right movement). (Just camera Movement Tracking)
8.	Perspective transformation (means how to consider the whole field into the rectangle viewed form top so that distance and speed can be calculated easily).
We have taken the actual football field dimensions and then mapped that to the perspective view of the camera or video so that it calculate the exact distance in meters.
9.	Final Speed and Distance Calculation.

## Requirements
To run this project, you need to have the following requirements installed:
- Python 3.x
- ultralytics
- supervision
- OpenCV
- NumPy
- Matplotlib
- Pandas
