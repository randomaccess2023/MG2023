# Feature to image representation using Matplotlib

t-Distributed Stochastic Neighbor Embedding (t-SNE) is a non-linear dimensionality reduction technique which allows us to visualize high-dimensional data in a lower-dimensional space.

I used sklearn's __digits__ dataset for this example which contains images of 0 to 9 having a resolution of __8x8__ pixels. I selected 5 samples of each digit. I applied t-SNE on their features and reduced their dimensionality from 64 to 2. Then, I visualized the reduced features in a 2D plot. I also replaced these features with their corresponding images in another 2D plot.

This is how these plots look like:

![feature_to_image.jpg](https://github.com/randomaccess2023/MG2023/blob/main/Video%2064/feature_to_image.jpg "feature_to_image.jpg")

### The full code is avilable at `feature_to_image.ipynb`.
