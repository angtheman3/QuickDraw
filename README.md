# QuickDraw
Developed and trained a 2D CNN using TensorFlow and Keras on
Google's QuickDraw dataset, achieving 92% accuracy, to accurately
recognize and classify real-time hand-drawn images. 

# Doodle Classifier using QuickDraw Dataset

## Overview

This project develops a classifier to recognize and categorize doodles using the QuickDraw dataset provided by Google. The goal is to demonstrate the capability of convolutional neural networks (CNNs) to process and classify images of simple drawings into predefined categories.

## Project Components

### Data Preparation
- **Classes List**: The classifier is trained on a subset of categories. These categories are listed in `mini_classes.txt`, from which the relevant doodle data is downloaded.
- **Download Script**: A Python script automatically fetches the `.npy` format dataset for each category from Google Cloud Storage.

### Data Processing
- **Data Loading**: The data for each class is loaded and limited to a specific number of examples to maintain uniformity and manage computational resources.
- **Data Splitting**: The dataset is shuffled and split into training and testing sets to evaluate the model's performance.

### Model Architecture
- **CNN Model**: The classifier is built using a sequential CNN architecture suitable for image data. The model includes convolutional layers, max-pooling layers, and dense layers, optimized for top-k categorical accuracy.

### Training and Evaluation
- **Model Compilation**: The model is compiled with categorical crossentropy loss and an Adam optimizer.
- **Model Training**: The model is trained using the processed data, with validation splits to monitor performance and avoid overfitting.
- **Model Evaluation**: After training, the model's accuracy is assessed on a separate test set.

### Deployment
- **Model Export**: The trained model is converted to TensorFlow.js format, allowing for easy deployment in web applications.
- **Web Application**: An interactive web application is set up to allow users to draw a doodle in the browser and have it classified in real time.

## Usage

Instructions to run the project locally, including steps to install necessary dependencies, load and preprocess the data, train the model, and deploy the classifier to a web application.

## Technologies Used

- Python for scripting and model training.
- TensorFlow and Keras for building and training the neural network.
- TensorFlow.js for deploying the model to a web application.

## Conclusion

This project showcases the application of deep learning to a fun and interactive problem, demonstrating the power of neural networks in classifying even simple, hand-drawn images effectively.

