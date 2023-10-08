# Internal Cluster Validation Using `ClustersFeatures` Module 

* In notebook `ClustersFeatures.ipynb`, I showed how `internal cluster validation` can be performed using **Ball-Hall index, Banfeld-Raftery index, Ray-Turi index, Xie-Beni index, C index, Mclain-Rao index, Wemmert-Gancarski index and PBM index**.

* __Ball-Hall__ index, __Banfeld-Raftery__ index, __Ray-Turi__ index, __Xie-Beni__ index, __C__ index and __Mclain-Rao__ index denote better clustering if the `index value` is _lower_.

* On the other hand, __Wemmert-Gancarski__ index and __PBM__ index designate better clustering if the `index value` is _higher_.

* We can easily calculate these metrics using the `ClustersFeatures` module. In the folder __ClusterFeatures__, you will find a file named `indices.json`. This file is required for `ClustersCharacteristics` method within `ClustersFeatures` module to work properly. You don't need to understand anything that's wriiten in this file.

> Some differences can be found with notebook `ClustersFeatures.ipynb` and the code that has been shown in the video of __MEDIOCRE_GUY__ YouTube channel.

These are minor differences. __NO NEED TO WORRY ABOUT IT__.
