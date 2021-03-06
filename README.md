# Visualization of (relatively) clear clustering of MNIST dataset- autoencoder + t-SNE dim-reduction

Inspired by [this paper](https://arxiv.org/pdf/1802.00187.pdf), this script trains an autoencoder to compress the MNIST dataset into a relatively small dimension (30 for the below images), then applies t-SNE dimensionality reduction to compress the dataset further into 2 or 3 dimensions which are visualized below.

In order to acheive the normalization on the encoding representation that the paper suggests, I used a relatively recent [self-normalizing neural network](https://arxiv.org/pdf/1706.02515.pdf) approach.

There's nothing particularly special about the MNIST dataset here- this can be applied to any set of data.

Below is the resulting visualization of the MNIST dataset visualized in two dimensions:

![2-dim](imgs/mnist2.png)

and in three dimensions:

![3-dim](imgs/mnist3.png)

It may be hard to see the clustering in a static image, so here is an animated version of the above plot.

![3-dim](imgs/mnist3.gif)

These results are generally poorer than the results the linked paper contains. This was relatively quick so the autoencoder structure should be varied in terms of layer size, regularization, dropout, etc. to find a better result (todo).

