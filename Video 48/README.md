# Deep Convolutional Generative Adversarial Network (`GAN`) using PyTorch - Example with `FashionMNIST` dataset

In this video, I showed how a Deep Convolutional Generative Adversarial Network (`GAN`) can be trained using `FashionMNIST` dataset.

Just like GAN, DCGAN is also made up of two neural networks: __GENERATOR__ and __DISCRIMINATOR__. The `Generator` is responsible for generating realistic looking _fake data_ and the `Discriminator` tries to distinguish the _fake data_ from the _real data_. Generator wants to fool the discriminator by creating samples as real as possible. The major difference of __DCGAN__ with __GAN__ is strided _convolution_ layers are used here instead of _linear_ layers. 

The generator takes a random noise (in __BCHW (Batch size, Channels, Height, Width)__ format) as input and provides the output with the shape of an image. The discriminator takes an image as input and outputs a probability of that image being real.

#### The expectation is that the `Generator` will be able to produce data after sufficient training which is indistinguishable from real data.

You will find the full code in `DCGAN.ipynb` file.

This is how 256 randomly generated samples look like after training the `DCGAN` for 50 epochs:

![Generated samples.jpg](https://github.com/randomaccess2023/MG2023/blob/main/Video%2048/Generated%20samples.jpg "image Title")
