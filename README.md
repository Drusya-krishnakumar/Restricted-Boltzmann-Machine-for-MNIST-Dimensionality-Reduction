# Restricted-Boltzmann-Machine-for-MNIST-Dimensionality-Reduction
### Overview

This project implements a Restricted Boltzmann Machine (RBM) using TensorFlow to perform dimensionality reduction on the MNIST handwritten digit dataset. The RBM learns a compressed representation of images and reconstructs them using Contrastive Divergence (CD-1).

#### Dataset

The MNIST dataset contains:

60,000 training images

10,000 testing images
Each sample is a 28x28 grayscale image flattened into a vector of size 784.

#### Model Architecture

Visible layer: 784 units (input pixels)

Hidden layer: 128 units (learned features)

Weight matrix and bias vectors for visible and hidden units

Sigmoid activation used for probabilistic sampling

### Training Method

Training algorithm: Contrastive Divergence (CD-1)

Number of epochs: 20

Batch size suitable for stochastic gradient updates

Mean Squared Error (MSE) used as reconstruction loss

Training progressively reduced the reconstruction error, showing successful learning of the underlying structure from MNIST images.

### Feature Extraction

After training, hidden layer activations were extracted to form reduced dimensional representations of size 128 for each image. These features capture meaningful digit characteristics.

### Visualization

Dimensionality reduction methods:

PCA (Principal Component Analysis)

t-SNE (t-distributed Stochastic Neighbor Embedding)

t-SNE revealed clear digit clusters in 2D space, demonstrating that the RBM learned useful latent features.

### Results Summary

RBM trained successfully using CD-1

Reconstruction error decreased consistently across epochs

Hidden representations formed distinct class-wise separations

RBM proved effective for dimensionality reduction on MNIST

### Tools and Libraries

Python

TensorFlow

NumPy

Scikit-learn

Matplotlib

### Conclusion

This project shows that Restricted Boltzmann Machines can extract compressed and meaningful feature representations from image data. The learned features perform well when visualized in lower dimensions, revealing digit class clusters.
