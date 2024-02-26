# Vector-Quantized Variational AutoEncoder (`VQ-VAE`) using PyTorch - Example with `MNIST` dataset

In this video, I showed how a Vector-Quantized Variational AutoEncoder (`VQ-VAE`) can be trained using `MNIST` dataset.

There are mainly three parts in a `VQ-VAE`: an `encoder`, a `vector-quantizer` and a `decoder`. __Encoder__ extracts features from the original data and then they are provided to the __vector Quantizer__ section. This section learns a codebook (a fixed-size table of embedding vectors) and outputs discretized latent embeddings. Finally, __Decoder__ receates the input samples from these discretized latent embeddings.

There are three loss components in a `VQ-VAE`: `reconstruction loss`, `codebook loss` and `commitment loss`. __Reconstruction loss__ optimizes the encoder and decoder. __Codebook loss__ moves the embedding vectors towards the encoder output. __Commitment loss__ makes the encoder commits to an embedding.

The main difference between `VQ-VAE` and `VAE` is that __VQ-VAE__ learns a discrete representation whereas __VAE__ learns a continuous representation. _VQ-VAEs_ also don't suffer from [posterior collapse](https://datascience.stackexchange.com/questions/48962/what-is-posterior-collapse-phenomenon) issue like the _VAEs_.

You will find the full code in `vqvae.ipynb` file. Besides the code, I added a few `.pdf` files (__portion_of_training_dataset.pdf__, __portion_of_test_dataset.pdf__, __loss_curve.pdf__ and __model_prediction.pdf__) which contain the images that you will be able to see in `vqvae.ipynb`.
