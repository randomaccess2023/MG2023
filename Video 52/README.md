# Denoising Diffusion Probabilistic Model (`DDPM`) using PyTorch - Example with `MNIST` dataset  

In diffusion models, the original data distribution is destroyed by gradually adding Gaussian noise over a finite number of time steps to end up with pure noise. This process is called __forward/diffusion process__. Then, a neural network is trained to gradually remove the noise added to the original data and predict a distribution that looks like it came from the original data distribution. This process is called __reverse/denoising process__.

### The idea behind using diffusion models is to generate `realistic-looking images` from `pure noise` only if the model is trained well.

[![DDPMs](https://img.youtube.com/vi/hpgFQd9xJhA/0.jpg)](https://www.youtube.com/watch?v=hpgFQd9xJhA)

#### Forward_process_output:

![Forward_Process_Output.jpg](https://github.com/randomaccess2023/MG2023/blob/main/Video%2052/Forward_process_output.jpg "Forward_Process_Output.jpg")

#### Reverse_process_output:

![Reverse_Process_Output.jpg](https://github.com/randomaccess2023/MG2023/blob/main/Video%2052/Reverse_process_output.jpg "Reverse_Process_Output.jpg")

#### Random_sampling_from_noise:

![Random_sampling_from_noise.jpg](https://github.com/randomaccess2023/MG2023/blob/main/Video%2052/Random_sampling_from_noise.jpg "Random_sampling_from_noise.jpg")
