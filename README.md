## Autonomous Vehicle using Datamining Techniques

Applying datamining techniques, specifically CNN to train Autonomous vehicle, which recognises several traffic signs.

## Assembling the Pi-Car:

The following is the link for the pictures, which shows the assembly and connection establishemnest of the smart car.
https://drive.google.com/open?id=1QxsLuxqOaNv_Lo_0xhgbLtI6Ry0ytPXu

In this project, we are going to use Raspberry Pi 3 model B+ to control servos using Python.

# The car has the following functionalities:

1.Straight lane detection

2.Controlling back wheel servos

3.Controlling front wheel servos

4.Camera module

5.PID Control

## Dataset Characteristics

Image size : 28X28

Approx no.of images for each sign : 200

## CNN Characteristics

Architecture: LeNet Architecture

Optimizer: Adam Optimizer

The CNN has 1 input and 1 output layer, 2 convolutional layers.

In the first set of convolutional layers, we have 20 filters and the size is 5*5. Each convolution layer has an activation function, ReLU which is followed by the pooling layers.

Pool size is 2,2 and the stride is 2,2.

The second set of convolutional layer is followed by another activation function, ReLU and a softmax function. It has 50 filters each of size 5*5.

The model can be optimized by evaluating it against test data and determining the Loss and Accuracy.

Upon evaluating the model and finding out the Loss and Accuracy, we have made the following observations:

loss: 0.0426

acc: 0.9874

val_loss: 0.0197

val_acc: 0.9941

## Training

of epoch = 30

parameter values = Convolutional layer 1- 25 filters of size 5x5, Convolutional layer 2 - 50 filters of 5x5

drop out = 0.2

learning rate: We used Adam optimizer with learning rate le-3. The learning rate decay over each update is le-3/25.


## Entire Video Link





## Areas of scope for Improvement

1. Training the car, by using different types of images with the similar meaning

2. Reliable power supply

   3.Lane Detection for the car can be improved by adjusting our camera angel. The camera should be placed high, so that it can capture the lane easily. By adjusting the camera angel, according to the car, we have found improvement in lane detection.

   4.In order to improve the control of front and back wheels the motor should be flexible. A uniform motor with lower acceleration and deceleration rates gives high precision over extended duration.75mm to 250mm range would be ideal for Servo motor with frames.










