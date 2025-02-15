# AI Image Generator for Numbers

## Motivation

The idea for this project was to develop an image generator, inspired by well-known models like DALL-E or MidJourney. However, since I don’t have access to large compute clusters or high-performance hardware, I decided to create an image generator specifically tailored for numbers. This approach allowed me to keep the latent vector small and the computational requirements low, making it possible to run on limited hardware. Thereby, I was able to experiment with generative modeling concepts without being overwhelmed by compute complexity. 


I used Generative Adversarial Networks (GANs) and Conditional Variational Autoencoders (CVAEs). GANs use an adversarial framework where a generator and a discriminator compete to produce images and recognize images. In contrast, CVAEs rely on a bottle neck architecture and reconstruction based loss with a standardized latent vector in the middle.

I also wanted to experiment with both Tensorflow/Keras and PyTorch so I used them for the GAN and CVAE respectively.
## Dataset

Due to the lack of large-scale datasets, I used the MNIST dataset of handwritten digits. The MNIST dataset is well suited for this purpose because it provides a standardized collection of grayscale images of handwritten numbers representing labeled numbers from 0 to 9.

## Recombination

Since these are generative models I was able to generate combinations of numbers such as mixtures between 5 and 9 without the model ever having seen such an image.

