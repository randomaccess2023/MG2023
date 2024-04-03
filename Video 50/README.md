# DDPMs - Denoising Diffusion Probabilistic Models

In simple terms, two processes happen in denoising diffusion probabilistic models (`DDPMs`):

- The data structure is destroyed by gradually adding Gaussian noise over a finite number of time steps to end up with pure noise (`forward/diffusion process`)
- A neural network is trained to gradually denoise the data starting from pure noise and predict a distribution that looks like the original distribution (`reverse/denoising process`)

#### This is how it looks like in practice:

![Forward_Reverse.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2050/Forward_Reverse.png "Forward_Reverse.png")

### DDPM Training Process:

![DDPM_Training_Process.png]( "DDPM_Training_Process.png")

- Source image **$𝑥_0$** is randomly sampled from the original data distribution **$𝑞(x_0)$**
- **$𝑡$** (time step) is sampled uniformly between **$1$** and **$𝑇$**
- Actual noise **$𝜀$** is sampled from a normal distribution
- A neural network is trained via gradient descent to predict the noise **$𝜀_𝜃$**

### DDPM Sampling Process:

![DDPM_Sampling_Process.png]( "DDPM_Sampling_Process.png")

- Sampling starts from **$𝑥_𝑇$** which is an _isotropic Gaussian distribution_
- Neural network gradually denoises it until **$𝑡 = 1$**
- A slightly less denoised image **$𝑥_𝑡−1$** can be obtained using this equation
- An image **$𝑥_0$** is returned that looks similar to the original data distribution

### Reverse Process Output

![Reverse_Process_Output.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2050/Reverse_Process_Output.png "Reverse_Process_Output.png")

The final output from the reverse process should look like it came from the original data distribution.

### Random Sampling

![Random_Sampling.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2050/Random_Sampling.png "Random_Sampling.png")

DDPM models will be able to generate actual images from noise only if trained well.
