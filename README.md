# Neural Network for Sobel Filter Learning

## Overview
This project develops a neural network that learns to apply the Sobel filter to images. The Sobel filter is a popular edge detection technique used in image processing. The goal is to train a model that replicates the Sobel-filtered output from given input images.

## Getting Started
### Prerequisites
Ensure you have the following installed:

-Python 3.7+    
-TensorFlow 2.x    
-TensorFlow Addons   
-scikit-image   
-NumPy   
-Matplotlib   

## Dataset Preparation  
Prepare your dataset by running the corresponding cells of `model.ipynb` .
This will apply the Sobel filter to the images in `natural_images` and save the results in `sobel_filtered_dataset`.

## Model Development
The model architecture is defined in `model.py`.
This Convolutional Neural Network (CNN) is designed to apply the Sobel filter to images, replicating the edge detection process traditionally performed by classical image processing techniques. The model consists of several convolutional layers that extract and refine features from the input images, followed by upsampling layers that reconstruct the filtered image at its original resolution. Batch normalization and dropout layers are incorporated to stabilize training and prevent overfitting. The final output layer uses a sigmoid activation function to generate a Sobel-filtered version of the input image, effectively learning to perform edge detection in a data-driven manner.

## Results
After training, the results are visualized using matplotlib. The notebook includes side-by-side comparisons of original, predicted, and Sobel-filtered images. The model weights have been saved as `sobel_filter_model_weights.h5` in the repo.
