# `Hartigan index` using Python

__`Hartigan index` is a cluster evaluation technique__.

__Hartigan index (HI)__ is computed by taking the logarithm of the ratio among the sum-of-squares between each cluster (__*SSB*__) and the sum-of-squares within the clusters (__*SSW*__). Mathematically, it can be expressed like this

$$\text{HI}=\log{\left({SSB}\over{SSW}\right)}$$

where,

$$SSB=\sum_{i=1}^{k}n_i(\overline{x_i}-\overline{x})^2$$

and

$$SSW=\sum_{j=1}^{k}\sum_{i=1}^{n_g}(x_{ij}-\overline{x_j})^2$$

Here, $g=1,...,k$ are the number of groups, $n=\sum_{i=1}^{k}n_i$ are the number of data points and $\overline{x_j}$ stands for the center point of each cluster.

- I previously made a video on __Hartigan index__ using __river__ module version 0.7.0.

[![HI](https://markdown-videos-api.jorgenkh.no/youtube/DmHo983YIug)](https://youtu.be/DmHo983YIug)

> `river` module version 0.7.0 is a old version. The latest version of __river__ module doesn't have any method to calculate __Hartigan index__. _Hartigan index_ using `river` module can't be calculated without using the data centroids.

But, I found another way. We can use `ClustersFeatures` module (version 1.0.3) to calculate _Hartigan index_. However, some of the code of the `ClustersFeatures` module is outdated and results in error. So, I downloaded the `ClustersFeatures` __GitHub__ directory and made some changes. This directory after modifications can be found inside the __MODULE__ folder.

This is the original GitHub repository of `ClustersFeatures`: [Simon-Bertrand/Clusters-Features](https://github.com/Simon-Bertrand/Clusters-Features)

##### _I calculated `Hartigan index` using both the `river` and `ClustersFeatures` module and got the same output_.

### The full code is available at the `Hartigan_index.ipynb` file.
