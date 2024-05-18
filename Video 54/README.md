# `Conditional DDPM` using PyTorch - Example with `MNIST` dataset

In this video, `MNIST` dataset images have been used to train a *Conditional_DDPM* along with their labels to conditionally generate the output. `MNIST` dataset has 10 classes: __One - 1, Two - 2, Three - 3, Four - 4, Five - 5, Six - 6, Seven - 7, Eight - 8, Nine - 9, Ten - 10__. Here is a portion of these samples:

![mnist_portion.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2054/mnist_portion.png "mnist_portion.png")

The labels of `MNIST` images were fed to an embedding table with 10 embeddings (for 10 classes), each with an embedding size of 256 (the same as time embeddings). These embeddings were then added with time embeddings to conditionally train the `DDPM`.

I made a video on unconditional DDPM (__Denoising Diffusion Probabilistic Model (`DDPM`) using PyTorch - Example with `MNIST` dataset__) previously (where I typed up the entiore code from scratch) and you can watch it if you want:

[![DDPMs](https://markdown-videos-api.jorgenkh.no/youtube/obYjlH9Z63k)](https://youtu.be/obYjlH9Z63k)
