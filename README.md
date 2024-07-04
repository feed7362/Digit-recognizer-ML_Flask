# Digit Recognition Using CNN and Flask

# Overview

This project is full-stack app demonstrates a complete pipeline for digit recognition using a Convolutional Neural Network (CNN) model trained on the MNIST dataset. The model is served via a Flask web application, providing a user interface for drawing digits and obtaining predictions. The project covers data preparation, model training, and deployment, integrating both TensorFlow and Flask to create an interactive web app.

# Features

## Data Preparation:

- Combines the MNIST dataset with additional CSV data.
- Normalizes and reshapes the images for CNN input.

## Model Architecture:

- Utilizes several convolutional layers with batch normalization, dropout, and max-pooling.
- Includes zero-padding, activation functions, and dense layers for robust performance.

## Training and Validation:

- Splits the data into training and validation sets.
- Implements callbacks for saving the best model, reducing learning rate, early stopping, and handling NaN values.
- Uses ImageDataGenerator for data augmentation during training.

## Model Evaluation:

- Evaluates the model on validation data.
- Plots training and validation accuracy and loss over epochs.

## Web Application:

- Built with Flask, allowing users to draw digits on a canvas and get predictions.
- Displays a probability graph for the predicted digit.
- Logs application activity for easy debugging.

# Setup Instructions

Clone this repository:

```sh
git clone https://github.com/feed7362/Digit-recognizer-ML_Flask
```
Navigate to the project directory:

```sh
cd Digit-recognizer-ML_Flask
```
Install dependencies:
```sh
pip install -r requirements.txt
```
Train the model:

- Ensure your training data (train.csv) is in the correct directory.
- Run the training script to prepare and train the model.

Run the Flask app:
```sh
python app.py
```

Access the application at http://localhost:5000.

# Usage

- Open the web application.
- Draw a digit on the canvas.
- Click "Submit" to get the predicted digit and probability graph.
- Clear the canvas using the "Clear" button.

# Project Structure

- app.py: Flask application code.
- train.py: Script for data preparation and model training.
- templates: HTML templates for the web interface.
- static: Static files including CSS for the web interface.

## LICENSE
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />All material is available under [Creative Commons BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). You can **use, redistribute, and adapt** the material for **non-commercial purposes**, as long as you give appropriate credit by **citing our paper** and **indicate any changes** you've made.
