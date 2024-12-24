# Handwritten-Digit-Recognition-using-Deep-Learning
This Colab notebook demonstrates building and training a simple Artificial Neural Network (ANN) using TensorFlow and Keras to classify handwritten digits from the MNIST dataset.

Here's a breakdown of the steps:

  1. Data Loading and Preprocessing:

    * Loads the MNIST dataset using keras.datasets.mnist.load_data().
    * Preprocesses the image data by normalizing pixel values to a range of 0-1.
  
  2. Model Building:

    * Creates a sequential model using keras.Sequential().
    * Adds a Flatten layer to convert the 2D images into a 1D vector.
    * Adds a Dense layer with 128 neurons and ReLU activation.
    * Adds an output Dense layer with 10 neurons (for 10 digit classes) and softmax activation.

  3. Model Training:

    * Compiles the model with the Adam optimizer, sparse categorical cross-entropy loss function, and accuracy metric.
    * Trains the model using model.fit() for 10 epochs, splitting the training data into training and validation sets.

  4. Prediction and Evaluation:

    * Predicts on the test set using model.predict().
    * Converts predictions to class labels using argmax().
    * Evaluates the model's accuracy using accuracy_score().
  
  5. Visualization:

    * Plots the training and validation loss and accuracy curves.
    * Displays a sample image from the test set.
    * Predicts the class of the sample image.
In essence, this code creates a neural network to recognize handwritten digits, trains it on a dataset of such digits, and then evaluates its performance on unseen data.
GOOGLE COLAB LINK!!
https://colab.research.google.com/drive/1eVbeoEMM8PhycRqcRwv6LUY5j3ntc2-Y
