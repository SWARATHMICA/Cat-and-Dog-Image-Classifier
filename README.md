# Cat-and-Dog-Image-Classifier
This project demonstrates how to build and train a CNN to classify images of cats and dogs. The model's performance is evaluated and visualized using accuracy and loss plots. Additionally, a function to predict and display the classification of a single image is included.
This project demonstrates how to build and train a Convolutional Neural Network (CNN) to classify images of cats and dogs. The CNN is built using TensorFlow and Keras and trained on a dataset of images stored in local directories. The model's performance is evaluated and visualized using accuracy and loss plots. Additionally, a function to predict and display the classification of a single image is included.

# Project Structure
train_data_dir: Directory containing the training images.
validation_data_dir: Directory containing the validation images.
IMAGE_WIDTH: Width of the input images.
IMAGE_HEIGHT: Height of the input images.
BATCH_SIZE: Number of images processed in one iteration.
EPOCHS: Number of times the entire dataset is passed through the network.

# Steps Involved
Import Necessary Libraries:

TensorFlow and Keras for building and training the CNN.
Matplotlib for plotting accuracy and loss graphs.
NumPy for numerical operations.
ImageDataGenerator for data augmentation and preprocessing.
Data Preprocessing:

Images are resized to 150x150 pixels.
Training images are augmented with random transformations (rescale, shear, zoom, horizontal flip) to enhance model generalization.
Validation images are rescaled.
Build the CNN Model:

Four convolutional layers with ReLU activation and max pooling.
Flattening layer to convert 2D data to 1D.
Fully connected dense layer with 512 units and ReLU activation.
Output layer with a single neuron and sigmoid activation for binary classification.
Compile the Model:

Optimizer: Adam.
Loss Function: Binary Crossentropy.
Metrics: Accuracy.
Train the Model:

The model is trained for a specified number of epochs.
Training and validation accuracy and loss are plotted to monitor performance.
Visualize Model Performance:

Plots showing training and validation accuracy and loss over epochs.
Predict and Display Classification of a Single Image:

A function to load, preprocess, and classify a single image.
The prediction is displayed along with the image.
