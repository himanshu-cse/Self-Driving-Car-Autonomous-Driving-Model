# Self-Driving-Car

In this project a simulator provided by Udacity is used to collect data of a human driving behavior. This data contains images of three different cameras mounted on top of the vehicle, as well as the steering angle. A convolution neural network has been build, that receives the center image as input and predicts a steering angle to drive the car autonomously. 

![](https://github.com/himanshu-cse/Self-Driving-Car/blob/main/behavioral%20cloning.gif)

## To get the model

Run SelfDrivingCar.ipynb on google colab or on local system. Create a dataset using training mode of [Udacity self-driving simulator](https://github.com/udacity/self-driving-car-sim) or download the [dataset on jungle track](https://drive.google.com/file/d/1B3S3mWeDm8zZlF5S7zCoBlyaCY3m2gHu/view?usp=drive_link) which we created. On colab upload this dataset and driving_log.csv file. At the end of all execution, you will get different models saved.

## Requirements
- python
- numpy
- matplotlib
- jupyter
- opencv3
- pillow
- scikit-learn
- scikit-image
- scipy
- h5py
- eventlet
- flask-socketio
- seaborn
- pandas
- imageio
- moviepy
- tensorflow
- keras

## For Autonommous Playing
Run following command for different models trained above.
```
Python3 drive.py model.h5
```
The above command will load the trained model and use the model to make predictions on individual images in real-time and send the predicted angle back to the server via a websocket connection.

Saving a video of the autonomous agent
```
python drive.py model.h5 run1
```

The fourth argument, run1, is the directory in which to save the images seen by the agent. If the directory already exists, it'll be overwritten.

The image file name is a timestamp of when the image was seen. This information is used by video.py to create a chronological video of the agent driving.

Creates a video based on images found in the run1 directory. The name of the video will be the name of the directory followed by '.mp4', so, in this case the video will be run1.mp4.

