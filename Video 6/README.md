# Internal Cluster Validation: `Silhouette` score, `Davies-Bouldin (DB)` score, `Calinski-Harabasz (CH)` score 

* In notebook `SDBCH.ipynb`, I showed how `internal cluster validation` can be performed using **Silhouette score, Davies-Bouldin (DB) score and Calinski-Harabasz (CH) score**.

* _Silhouette_ score, __DB__ score and __CH__ score are all internal cluster validation techniques which can determine the goodness of clustering algorithms without external references.

* _Silhouette_ score and __CH__ score denote better clustering if the score is `higher`. On the other hand, a `lower` value of the __DB__ score indicates better clustering.

* We can easily calculate these metrics using built-in packages that are available in the `scikit-learn` library.

> Some differences can be found with notebook `SDBCH.ipynb` and the code that has been shown in the video of __MEDIOCRE_GUY__ YouTube channel.

These are minor differences. __NO NEED TO WORRY ABOUT IT__.
