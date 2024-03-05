# **Real-Time-Pose-Estimation**

## **Project Title :** Real Time Pose Estimation

## **Project Introduction :**

The goal of this project is to create a web application and an android application that uses the Mediapipe Holistic Model and WebRTC (Web Real-Time Communication) technology to perform pose estimation and action recognition in real time, which includes body, hand, and face pose estimation. Users of the proposed web application will be able to upload images, record video or use webcam through their web browser and perform pose estimation using the Mediapipe Model, which can quickly and accurately identify poses and actions in an image or video stream.

## **ML Model :** https://github.com/google/mediapipe

## **Background:**

Mediapipe can provide live perception of simultaneous human pose, face landmarks, and hand tracking with accuracy and speed. WebRTC is an open-source project that gives web browsers and mobile applications access to real-time communication features like peer-to-peer dialogue, audio and video streaming, and data transfer. Real-time apps benefit greatly from the ability of WebRTC to interact directly across web browsers without the use of a third-party server.

## **Project Scope:**

The scope of this project is to create a web-based application and also an android application that will use Mediapipe Holistic Model for pose estimation and WebRTC technology for real-time communication. The application will consist of two main components:

### 1. Video capture component:

Users will be able to record video or use live webcam using this component and their web browser's camera. The pose estimation component will receive a real-time stream of the webcam or the recorded video.

### 2. Pose estimation component:

This component will use Mediapipe Holistic Model to detect pose estimation in the captured video stream. The detected poses will be highlighted in real-time and the results will be displayed to the user.

## **Project Objectives:**

Develop a web-based application and an android app that can perform pose estimation using Mediapipe Holistic Model and WebRTC technology.
Provide users with an interactive and user-friendly interface that allows them to capture video in real-time through their web browser and perform pose estimation. Deploy Mediapipe Model for pose estimation and integrate it with WebRTC technology. Display the results of pose estimation in real-time to the user.

## **Architecture you intend to use**

This project will be based on client-server architecture

![architecture](https://dltlabsweb-media.s3.amazonaws.com/images/Unshrouding%20WebRTCDivya%20Singh%20Creative%202-3b3477ce-c531-4206-a63c-f73714464d88.png)
Image source : https://www.dltlabs.com/blog/what-is-webrtc-why-is-it-useful-789565

### Mediapipe Holistic model prediction sample:

![mediapipe output](https://mediapipe.dev/images/mobile/holistic_sports_and_gestures_example.gif)

Image source : https://google.github.io/mediapipe/solutions/holistic.html

### Packages required to run the project

mediapipe==0.9.1.0 \
streamlit==1.21.0 \
streamlit-webrtc==0.45.0 \
numpy==1.24.2 \
opencv-python-headless==4.7.0.72

### For https communication

By default the streamlit server will run on http and if we want to run to https then we should add the ssl certificates to config.toml file in ~/.streamlit/ folder.\
add following configuration in ~/.streamlit/config.toml for https communication.\
[server]\
sslCertFile = path-to-pem-file \
sslKeyFile = path-to-key-file

### Run the project

1. Clone this repository
2. Run the command `streamlit run main.py`
