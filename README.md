# Brain Tumor Detection Using MRI
In this project, Convolutional Neural Network has been used to classify whether a given MRI scan of a brain is tumorous or not. The dataset has been dowloaded from kaggle and can be found [here](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection).

## About the data
The dataset contains 2 folders: yes and no which contains 253 Brain MRI Images. The folder yes contains 155 Brain MRI Images that are tumorous and the folder no contains 98 Brain MRI Images that are non-tumorous.

## Data Augmentation

Since the dataset is insufficient for training the network, data augmentation has been used to expand the dataset and hence, enhance the training phase.

## Model architecture

The model consists of two Convolutional layers with 32 and 11 filters each, followed by a Batch Normalization and a MaxPooling layer each. The final output neuron has a sigmoidal activation since it's a case of binary clasification. The optimizer used here is 'adam' and the loss function used is 'bindary-cross-entropy'.

## Results

We split the dataset into train and test set in the ratio 80/20 and trained our model using that. The final accuracy achieved on the validation set was of 91.2%. 

