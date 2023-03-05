# Hand Gesture - Recognition

This project is to build a different Deep learning models and finalize the best accuracy model to recognise five different gestures performed by the user which will help users control the TV without using a remote . 

The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:

* Thumbs up:  Increase the volume
* Thumbs down: Decrease the volume
* Left swipe: 'Jump' backwards 10 seconds
* Right swipe: 'Jump' forward 10 seconds  
* Stop: Pause the movie

The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use. 

     
## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

## General Information
Required to create best Neural Network to recognise five different gestures performed by the user.

Telecom Users Usage Dataset [here](https://drive.google.com/uc?id=1ehyrYBQ5rbQQe6yL4XbLWe3FMvuVUGiL)

## Conclusions
Created  Convolutional 3D, Simple RNN, LSTM and GRU Models and final inferences are as below

# Final Inferences

| Experiment Number | Model | Result|Decision+Explanation |
| ----------------- | ------- | ------------- | --------------------- | ----------------------- |
                         

## Technologies Used
- numpy - version 1.21.6
- matplotlib - version 3.2.2
- seaborn - version 0.11.2
- sklearn - version 1.0.2
- keras - version 2.9.0

## Contact
Created by [@bhogasena] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->

