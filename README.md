# A or B Image Classification using Custom Dataset

This repository contains code for a basic image classification task that distinguishes between two classes, A and B, using TensorFlow and Keras. The code demonstrates the creation of a simple convolutional neural network (CNN) to classify images into one of the specified classes.

## Overview

The repository includes Python code that performs the following tasks:

- **Data Preparation**: Utilizes TensorFlow's `ImageDataGenerator` to prepare and preprocess images from a custom directory structure for training and testing.
- **Model Building**: Constructs a basic CNN using Keras' `Sequential` API consisting of convolutional and pooling layers, flattening, and dense layers for classification.
- **Model Training**: Trains the constructed model using the prepared data.
- **Model Evaluation**: Evaluates the trained model on a separate test dataset and calculates accuracy.
- **Visualization**: Displays sample images from the test dataset along with their predicted and true classes.

## Usage

To utilize this code:

1. **Dataset Preparation**: Organize the dataset into separate directories for training and testing. The `flow_from_directory` method requires a specific directory structure where each class has its own subdirectory.

   For example:

   ```
   ├── img-class
   │   ├── A
   │   │   ├── image1.jpg
   │   │   ├── image2.jpg
   │   │   └── ...
   │   └── B
   │       ├── image1.jpg
   │       ├── image2.jpg
   │       └── ...
   └── test
       ├── A
       │   ├── test_image1.jpg
       │   ├── test_image2.jpg
       │   └── ...
       └── B
           ├── test_image1.jpg
           ├── test_image2.jpg
           └── ...
   ```
2. **Adjust Configuration**: Modify the code to match your dataset's specifications, such as directory paths, image size, batch size, number of classes, etc.
3. **Run the Code**: Execute the Python script to train the model and evaluate its performance.

## Dependencies

- TensorFlow
- NumPy
- Matplotlib

## Note

This code serves as a basic demonstration for image classification and might require modifications or enhancements for more complex datasets or specific use cases.

Feel free to modify and adapt the code according to your requirements!
