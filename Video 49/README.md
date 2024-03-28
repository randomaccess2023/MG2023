# Conditonal Generative Adversarial Network (`Conditional_GAN`) using PyTorch - Example with `FashionMNIST` dataset

Generative adversarial networks (`GANs`) can be used to generate novel image data from random noise. Typically, the random noise is sampled from a normal distribution and then it goes through a series of transformations to turn into something meaningful (e.g., a new image like the ones on which is it is trained).

However, a _DCGAN_ doesn't let us control the appearance of the samples that are being generated. To be able to control what we want to generate, a conditioning mechanism needs to be utilized such as the **class** of an image.

In this video, `FashionMNIST` dataset images have been used to train a *DCGAN* along with their labels to generate exact output. `FashionMNIST` dataset has 10 classes: __T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot__. Here is a portion of these samples:
![Portion_FashionMNIST_dataset](https://github.com/randomaccess2023/MG2023/blob/main/Video%2049/Portion_FashionMNIST_dataset.png "Portion_FashionMNIST_dataset")
