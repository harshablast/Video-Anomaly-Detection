# Anomaly-Detection

This project is the implementation of our Approach towards the Deep Learning national competition - TCS Geek AI Mania 2018. We chose the Computer Vision track which was "Anomaly Detection in Videos".

## Problem Statement

In this problem statement, we had to use the UCSD Anomaly Detection in Videos dataset and train a model which was able to pick up anomalies from video frames. The dataset consisted of several videos in two scenes and there were labelled pixel masks indicating anomaly areas in each frame. We had to train a model which could take a video as it's input and output a sequence of binary pixel masks indicating the location and movement of anomalies in the video.

## Our Approach

We designed an LSTM+CNN based neural network which takes both original frame data and the optical flow frame data into separate branches and concatentating the filters at an intermediate stage to feed them into a common deep network.

![Model Diagram](/images/model_diagram.png)

## Results

We trained the network against Binary Cross Entropy Loss and it trained till 99% accuracy without overfitting. We won the overall 2nd Prize during the contest.
![2nd Prize Winners](/images/prize_presentation.jpeg)
