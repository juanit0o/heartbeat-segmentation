# Heartbeat Data Analysis

## Introduction
In this project, the aim is to analyze heartbeat data and segment it into four distinct phases (S1, Systole, S2, and Diastole). The signals correspond to sound recordings captured at a rate of 4000Hz, resulting in 4000 measurements per second. Three datasets are provided: training, validation, and test. The models will be trained and evaluated for the evolution of error during training and validation. Finally, the trained models will be tested on previously unseen test data to obtain an unbiased estimate of the true model error, as well as accuracy.

Each data file contains the values of the signal and the corresponding true classes ranging from 1 to 4, enabling the evaluation of the model as a supervised learning problem.

## Objectives
The main objective of this work is to segment the signals using various types of neural networks and compare them to determine which provides the best results. The performance of each network will be evaluated based on the accuracy of predictions in segmenting individual sounds rather than processing batches.

Individual evaluation of signals is preferred to avoid zero-padding in batches due to variable signal sizes, which could artificially inflate the model's accuracy.

To handle different signal sizes, a cutting approach was adopted to match the signal size to the smallest size encountered. Subsequently, a more flexible version capable of handling signals of varying sizes as input was implemented.

The used architectures were:
 - Feed-Forward Neural Networks
 - Convolutional Neural Networks
 - Recurrent Neural Networks
 - Transformer

## Detailed Objectives
- Segment cardiac signals into four phases using neural networks.
- Compare the performance of different types of networks.
- Evaluate the accuracy of predictions in segmenting individual signals.
- Handle different signal sizes as input for neural networks.
