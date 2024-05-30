Astro Image Denoiser
This repository contains scripts and resources for training and inferencing a deep learning-based denoising model for astronomical images. The dataset consists of over 34,000 generated Deep Sky Object (DSO) images, each of size 512x512, stored in HDF5 format. The model leverages an encoder-decoder architecture with advanced components such as residual blocks, dense blocks, attention mechanisms, and transformers to achieve high-quality denoising.

<p align="center">
  <img src="astro8 (1).jpg" alt="Original Image" width="400"/>
  <img src="denoised_astro8 (1).png" alt="Denoised Image" width="400"/>
</p>

This project provides a robust solution for denoising astronomical images. It includes:

Training Script: A script to train the denoising model on the provided dataset.
Inference Script: A script to apply the trained model to new noisy images.
Dataset: A large dataset of generated DSO images in HDF5 format.
Key Features
Encoder-decoder architecture with residual and dense blocks.
Attention mechanisms (CBAM and NonLocal blocks) for enhanced feature extraction.
Wavelet transforms and transformer blocks for multi-scale feature extraction.
Supports parallel processing for efficient data extraction and model training.
Dataset
The dataset consists of over 34,000 Deep Sky Object images, each of size 512x512 pixels, generated using Stable Diffusion. The images are stored in HDF5 format for efficient access and processing.

File: SD_Astro_combined.h5
Format: HDF5
Contents: Contains a dataset of 512x512 pixel RGB images.

SD DSO Astro DataSet 34000 images, 18gb: https://drive.google.com/file/d/14yLiI7R8ghl0BlAGMSgMEuafA9t9Whxa/view?usp=sharing
Additional SD DSO Astro Data (11000 images, 9gb): https://drive.google.com/file/d/1x0B4vog2sqJ4P-kJOKpYupuR0hwkbTMs/view?usp=drive_link
