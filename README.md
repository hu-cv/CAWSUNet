
# MSFSRNet
Hi! You are welcome to visit here! This repository will be used to release the code of a novel image denoising model called the Channel Attention Weight Sharing U-Net for Single Image Denoising (abbreviated as CAWSUNet), which has been proposed in our paper entitled "CAWSUNet: Channel Attention Weight Sharing U-Net for Single Image Denoising" submitted to the International journal of XXX. **NOTE that once our manuscript is accepted by the journal, we will release the code immediately**. 
## Abstract

 <p> Image denoising plays a crucial role in image processing, with the primary goal of removing noise while preserving details. 
Traditional denoising methods have good removal effects for simple noise, but often perform poorly when dealing with complex noise. In contrast, deep learning-based techniques perform better in complex noise scenes, but may also face the problem of over-smoothing, resulting in the loss of image details. In this paper, we propose a channel attention weight sharing U-Net (CAWSUNet) to solve this problem. CAWSUNet optimizes the channel attention mechanism and adopts a weight sharing strategy to share attention weights locally and globally, which can not only effectively extract local features, but also enhance the capture of global information, thereby avoiding excessive attention to local details and ignoring global structures. In order to avoid the over-smoothing phenomenon in existing deep learning denoising methods, CAWSUNet pays special attention to detail retention to prevent the image from losing its original texture and color. It uses a feature sub-block weight sharing module to accurately retain the tiny details in the image while denoising and prevent the image from becoming blurred. In addition, in terms of computational efficiency, CAWSUNet adopts weight sharing and lightweight design to significantly reduce the number of parameters and computation of the model. To validate the effectiveness of the proposed method, extensive experiments were conducted on four synthetic datasets and two real-world datasets. The results demonstrate that the CAWSUNet model significantly outperforms existing methods in both denoising effectiveness and computational efficiency. Codes are available at https://github.com/hu-cv/CAWSUNet.
 </p>
 
# Experimental Datasets
## Image Denoising
###  Gray-Scale Image Denoising
* **BSD68 [1]** :BSD68 is a grayscale image converted from the CBSD68 dataset.
* **Set12 [2]** :Set12 is a collection of 12 grayscale images of different scenes that are widely used for evaluation of image denoising methods. The size of each image is 256×256.
###  Synthetic Color Image Denoising
* **CBSD68 [1]** :Color BSD68 dataset for image denoising benchmarks is part of The Berkeley Segmentation Dataset and Benchmark. It is used for measuring image denoising algorithms performance. It contains 68 images. https://github.com/clausmichele/CBSD68-dataset
* **Kodak24 [3]** :Kodak24 includes 24 color images, all images are 500*500 in size.
* **McMaster [4]** :The McMaster dataset is a dataset for color demosaicing, which contains 18 cropped images of size 500×500.
###  Real-World Color Image Denoising
* **SIDD [5]** :  SIDD includes about 30,000 noise images from 10 scenes, taken by 5 representative smartphone cameras, and generated their ground truth images. https://abdokamel.github.io/sidd/#sidd-benchmark
* **DND [6]**:  It consists of 50 pairs of real noisy images and corresponding ground truth images that were captured with consumer grade cameras of differing sensor sizes. For each pair, a reference image is taken with the base ISO level while the noisy image is taken with higher ISO and appropriately adjusted exposure time. The reference image undergoes a careful post-processing entailing small camera shift adjustment, linear intensity scaling and removal of low-frequency bias. The post-processed image serves as ground truth for our denoising benchmark. https://noise.visinf.tu-darmstadt.de/


References: <br>
[1] Julien Mairal, Francis R. Bach, Jean Ponce, Guillermo Sapiro, Andrew Zisserman: Non-local sparse models for image restoration. IEEE 12th International Conference on Computer Vision, ICCV 2009: 2272-2279. https://doi.org/10.1109/ICCV.2009.5459452 <br>
[2] Stefan Roth, Michael J. Black:Fields of Experts: A Framework for Learning Image Priors.2005 IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR 2005), 20-26 June 2005, San Diego, CA, USA.: 860-867. https://doi.org/10.1109/CVPR.2005.160 <br>
[3] Franzen R (1999) Kodak lossless true color image suite vol 4, https://r0k.us/graphics/kodak. <br>
[4] Lei Zhang, Xiaolin Wu, Antoni Buades, Xin Li: Color demosaicking by local directional interpolation and nonlocal adaptive thresholding. J. Electronic Imaging 20(2): 023016 (2011). https://doi.org/10.1117/1.3600632 <br>
[5]Abdelrahman Abdelhamed, Stephen Lin, Michael S. Brown: A High-Quality Denoising Dataset for Smartphone Cameras. Proceedings of the 2018 IEEE Conference on Computer Vision and Pattern Recognition, CVPR 2018: 1692-1700. https://doi.org/10.1109/CVPR.2018.00182 
[6]Tobias Plötz, Stefan Roth: Benchmarking Denoising Algorithms with Real Photographs. 2017 IEEE Conference on Computer Vision and Pattern Recognition, CVPR 2017: 2750-2759. https://doi.org/10.1109/CVPR.2017.294 




