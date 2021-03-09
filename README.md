
# Introduction

- The objective of this project is to use the perceptron learning method and
    design an artificial neural network (ANN) to train a simple system (single
    layer perceptron) for the recognition of handwritten digits (0, 1, ..., 9).
- Goal is to design a fully connected network structure of 784 input nodes
    and 10 output nodes.
- The input to your single layer network architecture will be a set of binary
    pixels representing a 28×28 image of handwritten digits. The output should
    indicate which of the digits (0,....,9) is in the input image.

# Project methodology, equations and implementations

Python Packages Used: -

- Idx2numpy
- NumPy
- Matplotlib
- Pandas
- Tabulate

Main Task: -

- Select a subset of the MNIST database consisting around 500 images of
    handwritten digits (0,...,9) for training the system, and use another 100
    images for testing the system. Create binary or bipolar images of
    handwritten digits from gray scale images available in MNIST by simple
    thresholding.
- Plot a learning curve that illustrates the mean square error versus
    iterations.
- Plot the percentage error in testing your handwritten digit recognition
    system as a bar chart.


Sub Tasks: -

- Task #1: Repeat this experiment for different learning rate parameters (at
    least 3 experiments. Start with a large value and gradually decrease to a
    small value).
- Task #2: Repeat Task #1 with a large database. The first 10000 images for
    training (image indexes from 0-10000) and test with another 1000 images
    (image indexes from 20000-21000).
- Task #3: Repeat Task #2 with multilevel data (without thresholding the
    input data, normalize the input data, use sigmoid function for output
    thresholding). What can you note comparing with part 2?
- Compare your results with the SVM results (what you have got from the
    last project).

Methodology and Implementations: -

- First step is to process the data. We have 2 datasets, first is the dataset
    contains 60000 images/array and the other one is the labels for the image
    data, image data contains the digit and label is the true value of that digits.
- Pre-process the data such that, neural network implementation can be
    done over the data, for that first thing is to manipulate the labels data as
    the label data contains the digit from 0 to 9 as per the image and we are
    implementing the single layer neural network and it works best on
    identifying the 0 or 1 data.
- To make the labels data into 0 to 1 from 0 to 9 dataset is to make it
    categorical such that label 6 become the array of [0, 0, 0, 0, 0, 0 , 1, 0, 0, 0].
- Next step is to transpose both the labels data and image data so it will be
    easy to implement the neural network.
- Next step is to make single layer neural network that works for all the part
    and also it has the sigmoid activation function such that the all the
    requirements of the tasks can be fulfilled.


- Next step is to get the graph of mean square error.
- Last requirement is to plot the bar chart of the error percentage on each
    digit.

**Conclusion:**

Sigmoid activation function is getting slightly more accuracy than the
regular one. It also depends on the training and testing size. Also, it depends on
the Learning rate and the iterations to get the lowest mean square error. Best
accuracy so far in this part is 0.9663 which we get by the sigmoid activation
function.

**References:**

NumPy: - https://numpy.org/

Idx2numpy: - https://pypi.org/project/idx2numpy/

Matplotlib: - https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.html

Pandas: - https://pandas.pydata.org/


