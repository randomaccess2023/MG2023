# Calculate FID (`Frechet Inception Distance`) using PyTorch

In this video, I tried to explain how `Frechet Inception Distance (FID)` can be calculated using PyTorch. I used 60000 training images of MNIST as the source or original images and I generated 60000 images using an unconditional DDPM model after training it for 50 epochs. I saved all the images in `.jpg` format. I stored the source images in the `src` folder and generated images in the `gen` folder.

__FID__ metric calculates the distance between the feature vectors of source and generated images, obtained by using a pre-trained InceptionV3 model. __FID__ measures the similarity between the features extracted from the source images and the generated images. A lower __FID__ score points out that the feature distributions of generated images
are close to source images; therefore, suggesting that the generator captures the data distribution of the source images very well. A higher __FID__ score indicates that the generated images do not have high similarity with the source images.

The full code is availble in the file `FID_Distance.ipynb`. `FID_Distance.ipynb` uses _InceptionV3_ function from the custom module `INCEPTION.py`.

### Source and Genrated Images can be found here: [Video 53.zip](https://drive.google.com/file/d/18Umq0cES93dM4EjYXrbnoD0V8UCJuEwW/view?usp=drive_link)

If you download this zip folder (__Video 53.zip__), you will see a folder named `Video 53` after extracting it. Inside `Video 53` folder, you will see two folders:
- `src` - contains source images
- `gen` - contains generated images

Put these two folders in the same directory with `FID_Distance.ipynb` and `INCEPTION.py`. By using `FID_Distance.ipynb` file only, you can calculate __FID distance__.
