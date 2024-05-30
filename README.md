<!DOCTYPE html>

<h1>Astro Image Denoiser - Created With GPT</h1>

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

<h2>Dataset</h2>

<p>The dataset consists of over 34,000 Deep Sky Object images, each of size 512x512 pixels, generated using Stable Diffusion. The images are stored in HDF5 format for efficient access and processing.</p>

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
