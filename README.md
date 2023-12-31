# Morse-Code-Game-using-CNN
A game which aims to test your morse code skills. Built using pygame and tensorflow.

# Description
- Tensorflow is used to create a Model using Convolutional Neural Network architecture. It is trained by using data from [kaggle](https://www.kaggle.com/datasets/sachinpatel21/az-handwritten-alphabets-in-csv-format). 
- A pygame window initializes with a blank canvas while the terminal displays a Morse Code for which the player is supposed to draw the alphabet for on the canvas and press Submit.
- The Model then predicts what alphabet the user drew on the canvas and increases the score if it was correct; this is implemented by the canvas getting saved as an image in the background and using cv2, numpy to preprocess the image before passing it to the model for assessment.
- Game runs until player clicks on quit.
  
# Demo Video
Note: All images drawn were correct except the last one to showcase how the game reacts in each case. Morse code chart is also provided for reference.

https://github.com/Sakaar-Sen/Morse-Code-Game-using-CNN/assets/52592149/a57fb6af-110d-40c1-802b-baa70493ad67


# Overview of the layers used in the Neural Network
- Convolutional Layer: The first convolutional layer has 64 filters with a kernel size of (3, 3) and uses the ReLU activation function. This layer processes the input images, extracting the imp features.

- Max Pooling Layer: A max-pooling layer with a pool size of (2, 2) follows the first convolutional layer. Primary purpose of this layer is to reduce the spatial dimensions of the data and help in capturing important patterns.

- Flatten Layer: The flatten layer converts the 2D feature maps into a 1D vector, preparing the data to be passed to the dense layer.

- Dense Layer: A dense layer with 128 units was using with the ReLU activation function.

- Dropout Layer: A dropout layer with a rate of 0.2 is introduced to prevent overfitting during training.

- Output Layer: The final output layer consists of 26 units(corresponding to the 26 alphabets; one-hot encoding was used for the labels during preprocessing). It uses the softmax activation function to produce probability scores for each class.

# Training 
The model is compiled with the Adam optimizer and uses categorical cross-entropy as the loss function, while monitoring accuracy as the training metric.

# Usage
1. Install the dependencies
   ```
   pip install tensorflow opencv-python numpy pygame
2. Download the dataset from [kaggle](https://www.kaggle.com/datasets/sachinpatel21/az-handwritten-alphabets-in-csv-format)
3. Preprocess data, train and save the model by running cells in Alphabet Detection Notebook.
4. Run MorseCodeGame to start playing!

### Suggestions to improve im too lazy to implement
- A friendlier way to play the game aka UI/System that doesnt require terminal + pygame being opened together. An all in one interface.
- High Scores 

# Contributing
Contributions to improve the model's performance, add new features, or fix any issues are welcomed. 




