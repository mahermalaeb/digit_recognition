# Digit recoginition using Tensorflow and Keras
Udacity's MLND deep learning project

## Notes:
* To run the jupyter notebook please prepare the datasets as follows:
  * Inside the `./MNIST_data/` folder place the mnist data files which are 4: 
    * train-images-idx3-ubyte.gz
    * train-labels-idx1-ubyte.gz
    * t10k-images-idx3-ubyte.gz
    * train-images-idx3-ubyte.gz
  * Inside the `./SVHN_data/` folder place the svhn data files which are 2:
    * test.tar.gz
    * train.tar.gz
* Deeper consideration should be given to the below snippet from the following [paper](https://arxiv.org/pdf/1312.6082.pdf)
`To train the model, one can maximize on the training set using a generic method like stochastic gradient descent.  Each of the softmax models (the model for and each) can use exactly the same backprop learning rule as when training an isolated softmax layer, except that a digit classifier softmax model backprops nothing on examples for which that digit is not presen`
