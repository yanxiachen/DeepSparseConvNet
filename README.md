# DeepSparseConvNet
Model-based Convolutional De-Aliasing Network Learning for Parallel MR Imaging
## Introduction
Parallel imaging has been an essential technique to accelerate MR imaging. Nevertheless, the acceleration rate is still limited due to the ill-condition and challenges associated with the undersampled reconstruction. In this paper, we propose a model-based convolutional dealiasing network with adaptive parameter learning to achieve accurate reconstruction from multi-coil undersampled k-space data. Three main contributions have been made: a de-aliasing reconstruction model was proposed to accelerate parallel MR imaging with deep learning exploring both spatial redundancy and multi-coil correlations; a split Bregman iteration algorithm was developed to solve the model efficiently; and unlike most existing parallel imaging methods which rely on the accuracy of the estimated multi-coil sensitivity, the proposed method can perform parallel reconstruction from undersampled data without explicit sensitivity calculation. Evaluations were conducted on in vivo brain dataset with a variety of undersampling patterns and different acceleration factors. Our results demonstrated that this method could achieve superior performance in both quantitative and qualitative analysis, compared to three state-of-the-art methods.
### Fig.1
<div align=center><img src="https://github.com/yanxiachen/DeepSparseConvNet/blob/master/Fig1.pdf" alt="Fig.1"/></div>

An illustration of the filter operator with convolutional neural networks for both spatial and multi-coil correlations.
### Fig.2
<div align=center><img src="https://github.com/yanxiachen/DeepSparseConvNet/blob/master/Fig2.pdf" alt="Fig.1"/></div>

The proposed convolutional de-aliasing network architecture for pMRI reconstruction. (a) is the flow chart. The orange arrow indicates the process of reconstructing the undersampled k-space data by forward propagation, and the green arrow indicates the parameter updating through back propagation. (b) and (c) are the detailed configurations of Conv1 and Conv2.
### Fig.3
<div align=center><img src="https://github.com/yanxiachen/DeepSparseConvNet/blob/master/Fig3.pdf" alt="Fig.1"/></div>

Comparison of different methods in reconstruction accuracy with different undersampling patterns and acceleration factors: reconstruction results and error maps are presented with corresponding quantitative measurements in PSNR/SSIM.
## Requirements and Dependencies
    MATLAB R2018a
    MatConvNet-1.0-beta25
