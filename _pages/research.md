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

## Denoising of 3D MR images using a voxel-wise hybrid residual MLP-CNN model to improve small lesion diagnostic confidence
<p align="center">
  <img width="60%" src="/images/denoise.png">
</p> 

Small lesions in magnetic resonance imaging (MRI) images are crucial for clinical diagnosis of many kinds of diseases. However, the MRI quality can be easily degraded by various noise, which can greatly affect the accuracy of diagnosis of small lesion. Although some methods for denoising MR images have been proposed, task-specific denoising methods for improving the diagnosis confidence of small lesions are lacking. In this work, we propose a voxel-wise hybrid residual MLP-CNN model to denoise three-dimensional (3D) MR images with small lesions. We combine basic deep learning architecture, MLP and CNN, to obtain an appropriate inherent bias for the image denoising and integrate each output layers in MLP and CNN by adding residual connections to leverage long-range information. We evaluate the proposed method on 720 T2-FLAIR brain images with small lesions at different noise levels. The results show the superiority of our method in both quantitative and visual evaluations on testing dataset compared to state-of-the-art methods. Moreover, two experienced radiologists agreed that at moderate and high noise levels, our method outperforms other methods in terms of recovery of small lesions and overall image denoising quality. 

# MRI technology



## CEST



## MRS

