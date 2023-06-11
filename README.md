# Chest X-Ray Pneumonia Detection

This repository contains a simple PyTorch program for classifying chest X-ray images to detect pneumonia. The program uses a Convolutional Neural Network (CNN) architecture and achieves an accuracy of 76% on the test set.

## Dataset

The program uses the "chest-xray-pneumonia" dataset, which is available on Kaggle. The dataset consists of chest X-ray images labeled as pneumonia or not. The dataset is organized into separate training and test sets.

To use this program with the Kaggle dataset, follow these steps:

1. Download the "chest-xray-pneumonia" dataset from Kaggle (provide a link to the dataset).

2. Extract the dataset and place it in the desired location on your local machine.

3. Set the `data_dir` variable in the PyTorch program to the directory path where you extracted the dataset.

## Program Overview

The PyTorch program follows a standard image classification pipeline. Here's a brief overview of the program's structure:

- Data Preparation: The program applies data transformations, including resizing images to (56, 56) pixels and converting them to tensors. It loads the training and test datasets using the `ImageFolder` class from torchvision and creates data loaders for efficient batch loading.

- Model Architecture: The program defines a CNN model using the `torch.nn.Sequential` class. The model consists of a flattening layer, two fully connected layers, and ReLU activations. The final layer has 2 output units for the pneumonia and non-pneumonia classes.

- Training: The program trains the model using the Adam optimizer and cross-entropy loss function. It performs multiple epochs and prints the training loss for each epoch.

- Evaluation: After training, the program evaluates the model on the test set, calculating the accuracy by comparing predicted labels with true labels.

## Usage

To use this program, follow these steps:

1. Clone or download this repository to your local machine.

2. Set up the "chest-xray-pneumonia" dataset directory as mentioned in the Dataset section.

3. Install the required dependencies (PyTorch, torchvision).

4. Run the program using a Python interpreter or an IDE that supports PyTorch.

Note: Adjust the dataset path and program settings according to your specific setup.

## Results

The program achieves an accuracy of 76% on the test set. You can modify the program, tune hyperparameters, or try different model architectures to potentially improve the accuracy.

## License

This project is licensed under the [MIT License](LICENSE).

Feel free to use and modify the code according to your needs.

