# CNN(convolutional neural networks)

## Introduction

**Convolution** refers to a mathematical operation in which a **filter** (also called a kernel or a weight) is applied to an input data matrix to produce a **feature map**.

The convolution operation involves sliding the filter over the input data matrix, element-wise multiplying the filter values with the corresponding input values within the sliding window, summing the products, and storing the result in the corresponding position of the feature map. This process is repeated for every position of the filter sliding over the input data matrix, **producing a feature map that summarizes the presence or absence of certain features in the input data**.

The size of the feature map is determined by the size of the input data and the size of the filter. **Convolutional layers in CNNs typically have multiple filters that convolve over the input data to produce multiple feature maps**, each representing a different feature or pattern in the input data.

Convolutional layers play a key role in learning features from the input data in CNNs and have been shown to be effective in various computer vision tasks such as image classification, object detection, and segmentation.

## Terminology

- **Convolutional layer**: A layer in which a set of filters convolve over the input data to produce a set of feature maps.
- **Kernel/Filter**: A set of learnable weights used in the convolution operation.
- **Stride**: The step size used by the kernel when it convolves over the input data.
- **Padding**: Adding zeros around the edges of the input data to preserve its dimension during convolution.
- **Activation function**: A non-linear function applied to the output of a layer to introduce non-linearity into the network.
- **Pooling layer**: A layer that downsamples the input data by reducing its size using a pooling function.
- **Max pooling**: A pooling function that takes the maximum value of a local region of the input data.
- **Average pooling**: A pooling function that takes the average value of a local region of the input data.
- **Fully connected layer**: A layer in which all neurons are connected to all neurons in the previous and next layer.
- **Dropout**: A regularization technique that randomly drops out neurons during training to prevent overfitting.
- **Batch normalization**: A technique for normalizing the input data to each layer in order to improve training stability.

Loss function: A function used to measure the difference between the predicted output and the true output.

Optimizer: An algorithm used to update the weights of the network during training to minimize the loss function.

Learning rate: A hyperparameter that determines the size of the step taken during weight updates.

Epoch: One complete iteration through the training data.

Backpropagation: An algorithm used to compute the gradients of the loss function with respect to the weights of the network.

## Dimension calculation



## Reference
[1] https://towardsdatascience.com/a-comprehensible-explanation-of-the-dimensions-in-cnns-841dba49df5e
