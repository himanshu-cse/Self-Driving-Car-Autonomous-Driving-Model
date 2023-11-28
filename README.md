# Self-Driving-Car

In this project a simulator provided by Udacity is used to collect data of a human driving behavior. This data contains images of three different cameras mounted on top of the vehicle, as well as the steering angle. A convolution neural network has been build, that receives the center image as input and predicts a steering angle to drive the car autonomously. This is a non-trivial regression tasks, therefore a powerful library was needed to realize it. The solutions is Keras, a Deep learning library that provides a high-level neural networks API, in this case for Tensorflow as a backend.

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
Start up the Udacity [](self-driving simulator), choose a scene and press the Autonomous Mode button. Then, run the model as follows:
```
Python3 drive.py model.h5
```

## Results
