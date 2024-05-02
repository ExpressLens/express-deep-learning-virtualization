# Express Deep Learning Virtualization
Implementing deep learning in Rust using just a linear algebra library ([nalgebra](https://nalgebra.org/)). The neural network (4 hidden layers, 32 neurons per layer) attempts to reconstruct a 512x512 image. It takes a 2D position as input, and outputs an RGB value.

# Results
Training time is around one minute, which is suprisingly quick considering that no parallelism or GPU acceleration is involved. Here is the reference image:

![Reference photo](https://github.com/ExpressLens/express-deep-learning-virtualization/blob/master/data/photo.jpg)

and here is the reconstruction from the neural network:

![Reconstruction](https://github.com/ExpressLens/express-deep-learning-virtualization/blob/master/reconstruct-fourier.png)

Note that I implemented Fourier features, as described [here](https://arxiv.org/pdf/2006.10739.pdf) to improve reconstructi