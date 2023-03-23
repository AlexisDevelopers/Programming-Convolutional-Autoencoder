This project focuses on the implementation of an autoencoder for the MNIST dataset. To do this, the TensorFlow library is used to build the autoencoder model. The implementation is divided into the following stages:

       Data Loading and Preprocessing: The MNIST dataset is loaded into a numpy array and the image labels are separated into two different arrays: one for the images and one for the labels. The data values are then scaled and the labels are encoded using One-Hot encoding.

       Data partitioning: The Sklearn library function train_test_split is used to split the data into two sets: one for training and one for testing.

       Creating the autoencoder model: The autoencoder model is defined using the TensorFlow functional API. One convolutional neural network is created for the encoder and another for the decoder. The encoder receives as input a grayscale image of size 28x28x1 and transforms it into a latent vector of size 10. The decoder, in turn, receives this latent vector and converts it back to an image of size 28x28x1.

       Model training: The model is compiled and fitted using the Adam optimizer and the MSE loss function over 30 epochs.

       Model evaluation: the results of the model evaluation are plotted, showing an input image, the latent vector, and the output image produced by the autoencoder.

This project can be useful for exploring the use of automatic encoders, for image compression and reconstruction, and for applying machine learning techniques to data analysis.