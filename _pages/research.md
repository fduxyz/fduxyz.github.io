---
layout: archive
permalink: /research/
title: ""
---



# Medical imaging with deep learning

Medical images, especially MRI (structural and functional modality) could provide a non-invasive way to conduct diagnosis and provide valuable information for the following treatment. Recently, COVID-19 has been a hot topic in medical imaging analysis. In addition, the accurate diagnosis of AD, PD and other psychotic diseases is significant, which requires new deep learning algorithms and task-specific framework to deal with this problem.

## Predicting the deterioration of COVID-19

<p align="center">
  <img width="50%" src="/images/covid.png">
</p> 

The respective value of clinical data and CT examinations in predicting COVID-19 progression is unclear, because the CT scans and clinical data previously used are not synchronized in time. To address this issue, we collected 119 COVID-19 patients with 341 longitudinal CT scans and paired clinical data, and we developed an AI system for the prediction of COVID-19 deterioration. By combining features extracted from CT and clinical data with our system, we can predict whether a patient will develop severe symptoms during hospitalization. Complementary to clinical data, CT examinations show significant add-on values for the prediction of COVID-19 progression in the early stage of COVID-19, especially in the 6th to 8th day after the symptom onset, indicating that this is the ideal time window for the introduction of CT examinations. We release our AI system to provide clinicians with additional assistance to optimize CT usage in the clinical workflow.

## GAN-Based Multiple MRI Modalities Synthesis and Segmentation for Mouse Brain Structures
<p align="center">
  <img width="50%" src="/images/gan.png">
</p> 

Automatic segmentation of mouse brain structures in magnetic resonance (MR) images plays a crucial role in understanding brain organization and function in both basic and translational research. Due to fundamental differences in contrast, image size, and anatomical structure between the human and mouse brains, existing neuroimaging analysis tools designed for the human brain are not readily applicable to the mouse brain. To address this problem, we propose a generative adversarial network (GAN)-based network, named MouseGAN, to synthesize multiple MRI modalities and to segment mouse brain structures using a single MRI modality. MouseGAN contains a modality translation module to project multi-modality image features into a shared latent content space that encodes modality-invariant brain structures and a modality-specific attribute. In addition, the content encoder learned from the modality translation module is reused for the segmentation module to improve the structural segmentation. Our results demonstrate that MouseGAN can segment up to 50 mouse brain structures with an averaged dice coefficient of 83%, which is a 7–10% increase compared to baseline U-Net segmentation. To the best of our knowledge, it is the first Atlas-free tool for segmenting mouse brain structures from MRI data. Another benefit is that with the help of the shared encoder, MouseGAN can handle missing MRI modalities without significant sacrifice of the performance. We will release our code and trained model to promote its free usage for neuroimaging applications.


## 3D Global Fourier Network for Alzheimer’s Disease Diagnosis using Structural MRI

<p align="center">
  <img width="60%" src="/images/gfnet.png">
</p> 

Deep learning models, such as convolutional neural networks and self-attention mechanisms, have been shown to be effective in computer-aided diagnosis (CAD) of Alzheimer’s disease (AD) using structural magnetic resonance imaging (sMRI). Most of them use spatial convolutional filters to learn local information from the images. In this paper, we propose a 3D Global Fourier Network (GF-Net) to utilize global frequency information that captures long-range dependency in the spatial domain. The GF-Net contains three primary components: a 3D discrete Fourier transform, an element-wise multiplication between frequency domain features and learnable global filters, and a 3D inverse Fourier transform. The GF-Net is trained by a multi-instance learning strategy to identify discriminative features. Extensive experiments on two independent datasets (ADNI and AIBL) demonstrate that our proposed GF-Net outperforms several state-of-the-art methods in terms of accuracy and other metrics, and can also identify pathological regions of AD.



# MRI technology



## CEST

<img align="right" width="40%" src="/images/research/hyperspectral/mixed_pixel.jpg"> 

One application of hyperspectral images is land cover mapping. Land cover information refers to the spatial composition of man-made materials (e.g. asphalt, roof) and green vegetation (e.g. trees, grass) of a particular area, usually an urban area. This information is useful because urban environment is impacted by the spatial distribution of these materials, which in turn impacts the resident health and even global climate. 

Land cover mapping can be achieved by directly classifying the pixels (spectra) in hyperspectral images. However, this requires the hyperspectral image to be collected from an aircraft flying at a low altitude, which is an expensive process. A promising future is to use an orbital spectrometer (onboard a satellite) to collect hyperspectral images continuously. Then, however, the spatial resolution of the collected hyperspectral image will not be promising, i.e. a pixel may corresponds to several meters' area (e.g. 16 m or 30 m diameter) on the earth. In this case, we need some kind of *soft-classification* to find the proportion of different materials in a pixel. This problem is called the *spectral unmixing* problem [...](https://github.com/zhouyuanzxcv/Hyperspectral) 

## Registration and Fusion

Another problem is that a satellite often provides a multispectral image (or a panchromatic image) in addition to the hyperspectral image. A multispectral image has higher spatial resolution than a hyperspectral image but lower spectral resolution. Fusing these two types of images can lead to a both spatially and spectrally high-resolution image. How to spatially calibrate these two images for fusion (i.e. image registration) and how to combine them to produce an image that has both the advantages is another research topic [...](https://github.com/zhouyuanzxcv/Hyperspectral)

![fusion_flowchart](/images/research/hyperspectral/reg_fusion_flowchart.jpg)
