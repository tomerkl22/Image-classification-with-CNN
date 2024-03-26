I executed image classification using Convolutional Neural Networks (CNNs) by implementing a model with PyTorch. 
The classification task was performed on the OCTMNIST dataset, showcasing the effectiveness of CNNs in handling image data.


To download the dataset you can run : 

python download_octmnist.py

Implemented with the following structure:
    
    • A convolution layer with 8 output channels, a kernel of size 3x3, stride of 1, and padding chosen to preserve the original image size.
    • A rectified linear unit activation function.
    • A max pooling with kernel size 2x2 and stride of 2.
    • A convolution layer with 16 output channels, a kernel of size 3x3, stride of 1, and padding of zero.
    • A rectified linear unit activation function.
    • A max pooling with kernel size 2x2 and stride of 2.
    • An affine transformation with 320 output features (to determine the number of input features use the number of channels, width and height of the output of the second block.
    • A rectified linear unit activation function.
    • A dropout layer with a dropout probability of 0.7.
    • An affine transformation with 120 output features.
    • A rectified linear unit activation function.
    • An affine transformation with the number of classes followed by an output LogSoftmax layer.
