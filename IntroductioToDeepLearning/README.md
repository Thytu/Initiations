# Introduction to Deep Learning with Pytorch

Welcome to this introduction to Deep Learning !

In this workshop you will create you first Deep Learning model with Pytorch.

Pytorch is a python framework wich allow you to create simple deep learning model in few lines.
Another well known framework is Tensorflow, but due to its simplicity we will not present it more than that.

## Live Coding

We presented you a simple convolutional model to classify the Fashion MNSIT dataset.

Quick recap: 

- torchvision allow you to fetch well known dataset
- torch.optim give you a whole bunch of optimizer
- torch.nn let you acces to multiple layers as Conv2D, Dense, etc.

Feel free to read the notebook every time you need.

## Speech commands prediction

Now you saw the bases of pytorch, it's time to practice.

You will create a convolutional model using pytorch to predict few speech commands.
But don't worry here is a manual to help you reach this goal.


### Manual

**Goal:** You must reach a accuracy to 80% on the testing set.

**Step to follow:**

Due to the fact the dataset is composed of audio you will need to **preprocess** the dataset.

1. From each audio create it respective spectrogramme
2. Make shure there are no useless informations like scale, padding, etc.
3. Resize those resulting image to a more feetable size.

Few tips:

- Use scipy to create the spectrogrammes
- Use matplotlib to save the images
- Use h5py to create a more handleable

After creating your *hdf5* file you need to create your **Network**.

1. Create you sequential model
2. Add Convolutional layers
3. Calculate the reshaping to do
4. Add Dense layers
5. Create your optimizer and loss function

Now you'r ready to go ! 

1. Create your train and test function
2. Display your accuracies