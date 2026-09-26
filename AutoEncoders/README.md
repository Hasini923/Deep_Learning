### Experiment 7 – Autoencoders, Convolutional Autoencoders, Denoising Autoencoders & Variational Autoencoders

Studied representation learning through autoencoders and implemented a Fully Connected Autoencoder, a Convolutional Autoencoder, a Denoising Convolutional Autoencoder and a Variational Autoencoder (VAE) for image reconstruction and generation. The experiment also explored the effect of latent dimension size on reconstruction quality.

**Topics covered:**

* Fully Connected Autoencoder
* Convolutional Autoencoder (CAE)
* Reconstruction metrics: MSE, MAE, SSIM
* Image noise injection: Gaussian and Salt-and-Pepper
* Denoising Convolutional Autoencoder
* Variational Autoencoder (VAE)
* Reparameterization trick
* KL-divergence and reconstruction loss
* Latent space visualization and interpolation
* Generative sampling from a learned latent distribution
* Effect of latent dimension on reconstruction quality

**Dataset:** MNIST Handwritten Digit Dataset

* 10,000 training images and 2,000 test images (recommended laboratory subset)
* Grayscale images, spatial dimension 28 x 28 x 1
* 10 digit classes (0–9), labels used only for latent-space visualization

**Result:**
Compared Fully Connected AE, Convolutional AE, Denoising CAE and VAE models using MSE, MAE, SSIM, parameter count and training time. The experiment also demonstrated denoising performance under varying Gaussian noise levels, VAE-based generative sampling, smoothness of latent-space interpolation, and the trade-off between latent dimension (2, 8, 16, 32) and reconstruction quality. Numerical results were obtained from the experimental execution.
