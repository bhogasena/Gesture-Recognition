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

<table>
     <tr>
          <th>Experiment No</th>
          <th>Model</th>
          <th>Result</th>
          <th>Decision+Explanation</th>          
     </tr>
     <tr><td>1</td><td>Conv3D</td><td>Accuracy: 55</td><td>Used Image resize to 100*100 with Batch Size 10; Epochs - 10</td></tr>
     <tr><td>2</td><td>Conv3D</td><td>Accuracy: 78</td><td>Generator function updated to sort the frames inside each folder and same model got the very good accuracy compared to experiment 1.
So sort=”yes” in generator for remaining experiments below.
</td></tr>
     <tr><td>3</td><td>Conv3D</td><td>Accuracy: 63</td><td>Increased the batch size from 10 to 50 caused the model to take higher number of epochs to get optimal value of loss function. Even after 20 epochs training accuracy is around 70 only.

So used batch 10 for remaining experiments. 
</td></tr>
     <tr><td>4</td><td>Simple RNN</td><td>Accuracy: >97</td><td>Total params: 24,133,797
Trainable params: 24,080,677
Non-trainable params: 53,120
</td></tr>
     <tr><td>5</td><td>LSTM</td><td>Accuracy: >94</td><td>LSTM needs 4 times of SimpleRNN layer params and as Accuracy compared to SimpleRNN has not improved.</td></tr>
     <tr><td>6</td><td>GRU</td><td>Accuracy: >96</td><td>Total params: 24,177,125
Trainable params: 24,124,005
Non-trainable params: 53,120

Accuracy for GRP model is also same as Simple RNN and LSTM.

Among all of these Simple RNN uses less trainable params and so that is final model.
</td></tr>
</table>
                         
# Final Inferences

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

