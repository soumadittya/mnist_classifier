# mnist_classifier
In this project handwritten digit classification has been done using Convolutional Neural Networks and the model has been trained on MNIST handwritten digit dataset.
The dataset has been directly taken from the the keras built in datasets.

Libraries and frameworks used:

1. Keras (imported form Tensorflow) - For creating the CNN model and for making predictions
2. Numpy - For simple array manipulation
3. OpenCv - For converting images to sample images (located in 'data_own' folder in the root directory) grayscale and for resizing them.
4. Matplotlib - For displaying images.

There are two jupyter notebooks:

1. mnist_classifier.ipynb:
        This is for training the model and evaluation of the model After that the trained model has been saved as 'mnist_classifier.h5' in the folder 'model' in the root directory.
  
        
2. mnist_cassifier_loading_trained_model.ipynb:
        In this jupyter notebook the trained model has been loaded and then a function named 'predict' has been created which accepts a file path for an image. After the the image link is given to the 
        function does the following operations:
        
        - Image is loaded.
        - Image is converterted to grayscale as the traing data is all in grayscale.
        - Image is resized to 28 x 28 pixel as the traing set contains images of dimensions 28 x 28 pixels.
        - Image array is reshaped to (1, 28, 28, 1) due to the dimensions of the training array.
        - Then the image is passed to the model for predictions using the command ('cnn.predict(<image>)')
        - Then the function prints the predicted digit.
        - The image which has been given to the function is displayed using matplotlib library.
   
  
  There are two folders in the root directory:
  
  1. data_own:
        This folder contains random handwritten digit images.
        
  2. model:
        This folder contains the trained model.
