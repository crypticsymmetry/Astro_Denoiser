<!DOCTYPE html>

<h1>Astro Image Denoiser - Created With The Help of ChatGPT</h1>

<p>This repository contains scripts and resources for training and inferencing a deep learning-based denoising model for astronomical images. The dataset consists of over 34,000 generated Deep Sky Object (DSO) images, each of size 512x512, stored in HDF5 format. The model leverages an encoder-decoder architecture with advanced components such as residual blocks, dense blocks, attention mechanisms, and transformers to achieve high-quality denoising.</p>

<div style="text-align:center;">
    <img src="astro8 (1).jpg" alt="Original Image" width="400"/>
    <img src="denoised_astro8 (1).png" alt="Denoised Image" width="400"/>
</div>

<h2>Overview</h2>

<p>This project provides a robust solution for denoising astronomical images. It includes:</p>
<ul>
    <li><strong>Training Script</strong>: A script to train the denoising model on the provided dataset.</li>
    <li><strong>Inference Script</strong>: A script to apply the trained model to new noisy images.</li>
    <li><strong>Dataset</strong>: A large dataset of generated DSO images in HDF5 format.</li>
</ul>

<h3>Key Features</h3>
<ul>
    <li>Encoder-decoder architecture with residual and dense blocks.</li>
    <li>Attention mechanisms (CBAM and NonLocal blocks) for enhanced feature extraction.</li>
    <li>Wavelet transforms and transformer blocks for multi-scale feature extraction.</li>
    <li>Supports parallel processing for efficient data extraction and model training.</li>
</ul>

<h2>Custom Loss Function</h2>

<p>The model uses a custom loss function designed to improve the quality of denoised images. The custom loss function combines multiple loss components to capture different aspects of image quality:</p>
<ul>
    <li><strong>Charbonnier Loss</strong>: A robust L1 loss variant for improved stability.</li>
    <li><strong>Perceptual Loss</strong>: Ensures the perceptual quality of images by comparing feature maps from a pre-trained VGG network.</li>
    <li><strong>MSSSIM Loss</strong>: Maximizes the structural similarity between denoised and target images.</li>
    <li><strong>Frequency Domain Loss</strong>: Captures frequency information to preserve fine details.</li>
    <li><strong>Edge Loss</strong>: Enhances edge preservation by focusing on edge differences.</li>
    <li><strong>Color Luminance Loss</strong>: Maintains accurate color and luminance by comparing color spaces (LAB and YUV).</li>
    <li><strong>TV Loss</strong>: Encourages smoothness in the denoised images to reduce noise.</li>
</ul>

<h2>Dataset</h2>

<p>The dataset consists of over 34,000 Deep Sky Object images, each of size 512x512 pixels, generated using Stable Diffusion at 1024x1024 and downscaled to 512x512 using lancoz sampling. The images are stored in HDF5 format for efficient access and processing.</p>

<ul>
    <li><strong>File</strong>: <code>SD_Astro_combined.h5</code></li>
    <li><strong>Format</strong>: HDF5</li>
    <li><strong>Contents</strong>: Contains a dataset of 512x512 pixel RGB images.</li>
</ul>

<h3>Download Links</h3>
<ul>
    <li><a href="https://drive.google.com/file/d/14yLiI7R8ghl0BlAGMSgMEuafA9t9Whxa/view?usp=sharing">SD DSO Astro DataSet (34,000 images, 18GB)</a></li>
    <li><a href="https://drive.google.com/file/d/1x0B4vog2sqJ4P-kJOKpYupuR0hwkbTMs/view?usp=drive_link">Additional SD DSO Astro Data (11,000 images, 9GB)</a></li>
</ul>

</body>
</html>
