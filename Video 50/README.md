# DDPMs - Denoising Diffusion Probabilistic Models

In simple terms, two processes happen in denoising diffusion probabilistic models (`DDPMs`):

- The data structure is destroyed by gradually adding Gaussian noise over a finite number of time steps to end up with pure noise (`forward/diffusion process`)
 
- A neural network is trained to gradually denoise the data starting from pure noise and predict a distribution that looks like the original distribution (`reverse/denoising process`)

#### This is how it looks like in practice:

![Forward_Reverse.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2050/Forward_Reverse.png "Forward_Reverse.png")
