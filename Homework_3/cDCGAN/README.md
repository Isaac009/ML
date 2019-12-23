# Machine-Learning-2019
Assignments repository

# cDCGAN
DCGAN is one of the popular and successful network design for GAN. It mainly composes of convolution layers without max pooling or fully connected layers. It uses convolutional stride and transposed convolution for the downsampling and the upsampling. The figure below is the network design for the generator.

DCGAN Architecture

![](DCGAN.png)

# How to run
### Install 
* [TensorFlow](https://www.tensorflow.org/install/)
* [Matplotlib](https://matplotlib.org/)
* [Imageio](https://imageio.readthedocs.io/en/stable/installation.html)
* [Numpy](https://docs.scipy.org/doc/numpy/user/install.html)

## Train
If you cloned the whole repository 
### Classic MNIST 
### Dataset
* [MNIST](https://github.com/petewarden/tensorflow_ios/blob/master/tensorflow/g3doc/tutorials/mnist/download/index.md)
Dataset contains greyscale 28x28 pixel images of handwritten digits.
### Train The Model from scratch

```bash
python Homework_3/cDCGAN/tensorflow_MNIST_cDCGAN.py
```

## My result for Discriminator and Generator Loss
![](MNIST_cDCGAN_train_hist.png)

## Generator output the following images during the training
![](MNIST_cDCGAN_generation_animation.gif)

### Fashion MNIST 
```bash
python Homework_3/cDCGAN/tensorflow_F_MNIST_cDCGAN.py
```
## My result for Discriminator and Generator Loss
![](HW_F_MNIST_cDCGAN_train_hist.png)

## Generator output the following images during the training
![](HW_F_MNIST_cDCGAN_generation_animation.gif)


### Use Pretrained Model
### Load the model latest checkpoint
```bash
latest = tf.train.latest_checkpoint(checkpoint_dir)

# Create a new model instance
model = create_model()

# Load the previously saved weights
model.load_weights(latest)
``` 
