# Calculate `Inception Score (IS)` using PyTorch

In this video, I tried to explain how __Inception Score (IS)__ can be calculated using PyTorch. Inception score is a metric that is often used for evaluating the quality of synthetic images provided by generative models.

Inception score estimates the quality of a collection of synthetic images based on how well the pretrained _InceptionV3_ model classifies them as one of 1000 known objects. Inception score combines the confidence of the conditional class distribution (`quality`) and the integral of the marginal class distribution (`diversity`). In other words, conditional class distribution should have a low entropy and marginal class distribution should have a high entropy.

However, the inception score is limited by what the _InceptionV3_ model can detect. If the generated images are not present in the model's training data, the score will be low despite generating high-quality images since the image doesn't get recognized as a distinct class.

I generated 60000 MNIST images by an unconditional DDPM model after training it for 50 epochs. I saved all the images in `.jpg` format and stored them in the `gen` folder.

### The full code is available at `Inception_Score.ipynb` file. 

### Generated Images can be found here: [Video 53.zip](https://drive.google.com/file/d/18Umq0cES93dM4EjYXrbnoD0V8UCJuEwW/view?usp=drive_link)

If you download this zip folder (__Video 53.zip__), you will see a folder named `Video 53` after extracting it. Inside `Video 53` folder, you will see two folders:
- `src` - contains source images
- `gen` - contains generated images

You only need to use the `gen` folder for calculating __Inception Score (IS)__ because `IS` does not capture how synthetic images compare to real images like __FID distance__. Put this folder in the same working directory with `Inception_Score.ipynb`. By running the `Inception_Score.ipynb` file, inception score can be easily calculated.

After calculating the inception score, I obtained a score of 2.418, which is very low. A good inception score will output a high finite value (ideally, 1000 as the ImageNet dataset has that many classes but practically more than 100). But, we obtained a very low value because the ImageNet dataset does not possess the MNIST images and these images are unknown to the _InceptionV3_ model.

For this reason, FID distance was proposed as an improvement over the inception score metric. FID score metric was proposed to evaluate the quality of the synthetic images by comparing to that of the real images from the target domain.

The video on __FID distance__ is avilable on the channel:

[![FIDscore](https://markdown-videos-api.jorgenkh.no/youtube/8vWIvcFAWUc)](https://youtu.be/8vWIvcFAWUc)
