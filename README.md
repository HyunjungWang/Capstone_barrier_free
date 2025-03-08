# Identifying Barrier-Free Entrance Using CNN and Street View

## Overview

This project aims to identify barrier-free building entrances using Convolutional Neural Networks (CNN) and street view images. It is designed to assist individuals with mobility impairments by providing accessibility information about various locations.

## Background

According to traffic safety data, approximately 30% of the South Korean population consists of transportation-disadvantaged individuals, including the elderly, disabled, and those with young children. However, accessibility issues remain prevalent, with many buildings lacking proper entrance facilities.

To address this issue, our project utilizes street view images from platforms like Naver, Kakao, and Google to analyze and determine whether a building entrance is wheelchair-accessible.

## Methodology

We developed a CNN-based deep learning model to classify building entrances as accessible or inaccessible. The key steps involved in the project are:

#### 1. Data Collection

- Images of building entrances were collected from street view services and manually captured photographs.

- Data was categorized into accessible (ramps, flat entrances) and inaccessible (stairs without ramps) classes.


  

#### 2. Preprocessing

- Image resizing and augmentation techniques were applied to improve training performance.

- Custom augmentation techniques like Cutout Random Erasing and Random Noise were implemented.
  

#### 3. Model Development

- Various CNN architectures, including VGG16, ResNet, and DenseNet, were tested.

- Transfer learning was applied using pre-trained models from Keras.

- Final model selection was based on performance metrics such as accuracy, precision, recall, and F1-score
  

#### 4. Evaluation and Optimization

- K-fold cross-validation was used to ensure generalization.

- Ensemble learning techniques, including Average Ensemble, were implemented to improve accuracy.

- The final model achieved a test accuracy of up to 94%.
  

## System Implementation

The project consists of three main components:

- Model: Trained deep learning model implemented using TensorFlow and Keras.

- REST API: A Flask-based API that receives image inputs and returns accessibility predictions.

- Application: A prototype Android application that allows users to upload images or fetch street view images for accessibility predictions.

## Future Improvements

- Community Mapping Integration: Allow users to contribute accessibility data.

- Additional Accessibility Features: Include information about parking, restrooms, and public transportation accessibility.

- Enhanced Image Processing: Improve model robustness against various lighting and occlusion conditions.
