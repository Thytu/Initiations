# Introduction to Deep Learning with Pytorch

Welcome to this introduction to Deep Learning !

In this workshop you will create your first Deep Learning model with Pytorch.

Pytorch is a python framework wich allows you to create simple deep learning models in a few lines.
Another well known framework is Tensorflow, but due to its simplicity we will avoid using it.

## Live Coding

We presented you a simple [convolutional model](liveCoding.ipynb) to classify the Fashion MNSIT dataset.

Quick recap:

- `torchvision` allows you to fetch well known datasets
- `torch.optim` gives you a whole bunch of optimisation
- `torch.nn` gives you acces to multiple layers such as `Conv2D`, `Dense`, etc.

Feel free to take a look at the notebook as many times as you need.

## Speech command predictions

Now you saw the basics of pytorch, it's time to practice.
You will create a convolutional model using pytorch to predict some speech commands but don't worry, here is some documentation to help you reach this goal.


### Manual

**Goal:** You must reach an accuracy of 80% on the testing set.

**Steps to follow:**

Due to the fact that the dataset is composed of audio, you will need to <ins>preprocess the dataset</ins>.

1. From each audio, create its respective spectrogramme
2. Make shure there is no useless information like scale, padding, etc.
3. Resize those resulting images to a more suitable size.

Few tips:

- Use [scipy](https://docs.scipy.org/doc/scipy/reference/) to create spectrogrammes
- Use [matplotlib](https://matplotlib.org/3.1.1/) to save images
- Use [h5py](https://github.com/h5py/h5py) to easily store and manipulate numerical data

After creating your `hdf5` file you will need to <ins>create your Network</ins>.

1. Create you sequential model
2. Add a Convolutional layers
3. Calculate the necessary reshaping that needs to be done
4. Add Dense layers
5. Create your optimizer and loss function

Now you're good to go !

1. Create your train and test function
2. Display your the accuracie
