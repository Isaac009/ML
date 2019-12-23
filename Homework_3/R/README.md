# Machine-Learning-2019
Assignments repository

# DCGAN
DCGAN is one of the popular and successful network design for GAN. It mainly composes of convolution layers without max pooling or fully connected layers. It uses convolutional stride and transposed convolution for the downsampling and the upsampling. The figure below is the network design for the generator.

DCGAN Architecture
![](DCGAN.png)

![](imgs/vanilla_gan_detailed_arch.png)

# How to run
### Install 
* [TensorFlow](https://tensorflow.rstudio.com/installation/)
* [Keras](https://tensorflow.rstudio.com/reference/keras/install_keras/)
* [Tfdatasets](https://tensorflow.rstudio.com/guide/tfdatasets/introduction/)

## Train
If you cloned the whole repository 
### Classic MNIST 
```bash
Select session then set a working directory where the generated images will be saved.
Then, on r studio just select the line to execute and click run otherwise select all file scipt and click run
```
## My result for Discriminator and Generator Loss

## Generator Output after 150 training iteration steps
![](mnist.gif)

## Generator Output after 300 training iteration steps
![](r_f_mnist.gif)

## Use Pretrained Model
### Load the model 


