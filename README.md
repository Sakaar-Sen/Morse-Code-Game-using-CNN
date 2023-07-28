# Morse-Code-Game-using-CNN
A game which aims to test your morse code skills. Built using pygame and tensorflow.

# Detailed Description
- Tensorflow is used to create a Model using Convulational Neural Network architecture. It is trained by using data from [kaggle](https://www.kaggle.com/datasets/sachinpatel21/az-handwritten-alphabets-in-csv-format).
- A pygame window initializes with a blank canvas while the terminal displays a Morse Code which the player is supposed to draw on the canvas and press Submit.
- The Model then predicts what alphabet the user drew on the canvas and increases the score if it was correct; this is implemented by the canvas getting saved as an image in the background and using cv2, numpy to preprocess the image before passing it to the model for assessment.

# Demo Video
Note: All images drawn were correct except the last one to showcase how the game reacts in that case.

https://github.com/Sakaar-Sen/Morse-Code-Game-using-CNN/assets/52592149/709069b3-c3e8-490b-bb29-5958f6da6a7a


