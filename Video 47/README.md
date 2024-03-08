# Generative Adversarial Network (`GAN`) using PyTorch - Example with `MNIST` dataset

In this video, I showed how a Generative Adversarial Network (`GAN`) can be trained using `MNIST` dataset.

GAN is made up of two neural networks: __GENERATOR__ and __DISCRIMINATOR__. The `Generator` is responsible for generating realistic looking _fake data_ and the `Discriminator` tries to distinguish the _fake data_ from the _real data_. Generator wants to fool the discriminator by creating samples as real as possible.

The generator takes a random noise vector as input and outputs another vector having the shape of an image. The discriminator takes an image as input and outputs a probability of that image being real.

#### The expectation is that the `Generator` becomes able to produce data after training which is indistinguishable from real data.

You will find the full code in `GAN.ipynb` file. Besides the code, I added a few `.pdf` files (`Portion of MNIST (training) samples.pdf` __(it shows randomly selected 12 samples from the MNIST (training) dataset)__, `Loss curve.pdf` __(it shows the _discriminator loss_ and the _generator loss_)__ and `Generated samples.pdf` __(which shows 128 MNIST-like samples provided by the generator after training the `GAN`)__).
