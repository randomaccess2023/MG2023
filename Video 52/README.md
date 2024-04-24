# Denoising Diffusion Probabilistic Model (`DDPM`) using PyTorch - Example with `MNIST` dataset  

In diffusion models, the original data distribution is destroyed by gradually adding Gaussian noise over a finite number of time steps to end up with pure noise. This process is called __forward/diffusion process__. Then, a neural network is trained to gradually remove the noise added to the original data and predict a distribution that looks like it came from the original data distribution. This process is called __reverse/denoising process__.

### The idea behind using diffusion models is to generate `realistic-looking images` from `pure noise` only if the model is trained well.

[![DDPMs](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://youtu.be/hpgFQd9xJhA?si=Rdj9DZLtKLk2-4x8 "DDPMs")
