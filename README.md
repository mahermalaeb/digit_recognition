# Digit recoginition using Tensorflow and Keras (THIS IS NOT A WORKING MODEL)
Udacity's MLND deep learning project

## Guidlines for the reviewer:
* To run the jupyter notebook please prepare the datasets as follows:
  * Inside the `./MNIST_data/` folder place the mnist data files which are 4: 
    * train-images-idx3-ubyte.gz
    * train-labels-idx1-ubyte.gz
    * t10k-images-idx3-ubyte.gz
    * train-images-idx3-ubyte.gz
  * Inside the `./SVHN_data/` folder place the svhn data files which are 2:
    * test.tar.gz
    * train.tar.gz
* The Model is not working and the only reasonable predictions it is making is for the length of the synthetic sequnce
* I believe that the problem is coming from the design of the loss function because it is always summing the loss even if there is a blank character. In particular I am refering to the below snippet of the goodfellow paper 
`To train the model, one can maximize on the training set using a generic method like stochastic gradient descent.  Each of the softmax models (the model for and each) can use exactly the same backprop learning rule as when training an isolated softmax layer, except that a digit classifier softmax model backprops nothing on examples for which that digit is not presen`
* I left the 4th part of the project unsolved just to make sure I am on the right track before moving
