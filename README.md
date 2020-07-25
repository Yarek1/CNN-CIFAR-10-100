# CNN-CIFAR-10-100
Convolution neural network with cifar 10 and cifar 100 dataset

In neural networks, Convolutional neural network (ConvNets or CNNs) is one of the main categories for image recognition, 
image classifications, objects detections, recognizing faces etc., are some of the areas where CNNs are widely used.

The CIFAR-10 dataset consists of 60000x32 x 32 colour images divided in 10 classes, with 6000 images in each class. 
There are 50000 training images and 10000 test images.

The CIFAR-10 and CIFAR-100 are labeled subsets of the 80 million tiny images dataset. 
They were collected by Alex Krizhevsky, Vinod Nair, and Geoffrey Hinton.
More information about dataset here: https://www.cs.toronto.edu/~kriz/cifar.html

Convolutional networks are built from several types of layers:

Conv2D — performs convolution

filters: number of output channels

kernel_size: an integer or tuple/list of 2 integers, specifying the width and height of the 2D convolution window

padding: padding=”same” adds zero padding to the input, so that the output has the same width and height

activation: “relu”, “tanh”, etc.

input_shape: shape of input.
Our input image is a tensor whose width is 32 pixels and height is 32 pixels with 3 channels representing RGB( red, green, blue) color intensities. 
Thus we need to define a model which takes (None, 32, 32, 3) input shape.

MaxPooling2D — performs 2D max pooling.

Flatten — flattens the input, does not affect the batch size.

Dense — fully-connected layer.

Activation — applies an activation function.

Dropout — applies dropout.
Dropout layer after every pooling layer will be used to reduce overfitting in the model.
