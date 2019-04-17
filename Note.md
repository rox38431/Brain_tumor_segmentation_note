# Table of Contents
1. [Models](#1-models)   
    1.1 [Cascaded Anisotropic Convolutional Neural Networks](#11-cascaded-anisotropic-convolutional-neural-networks)   
    1.2 [DeepMedic (3D segment)](#12-deepmedic-3d-segment)   
    1.3 [U-net (2D segment)](#13-u-net-2d-segment)   
    1.4 [EFFICIENT SYMMETRY-DRIVEN FULLY CONVOLUTIONAL NETWORK FOR MULTIMODAL BRAIN TUMOR SEGMENTATION](#14-efficient-symmetry-driven-fully-convolutional-network-for-multimodal-brain-tumor-segmentation)   
    1.5 [Boundary-Aware Fully Convolutional Network for Brain Tumor Segmentation](#15-boundary-aware-fully-convolutional-network-for-brain-tumor-segmentation)   
    1.6 [Ensembles of Multiple Models and Architectures for Robust Brain Tumour Segmentation](#16-ensembles-of-multiple-models-and-architectures-for-robust-brain-tumour-segmentation)   
    1.7 [3D U-Net: Learning Dense Volumetric Segmentation from Sparse Annotation](#17-3d-u-net-learning-dense-volumetric-segmentation-from-sparse-annotation)   
    1.8 [On the Compactness, Efficiency, and Representation of 3D Convolutional Networks: Brain Parcellation as a Pretext Task]   
    1.9 [3D MRI brain tumor segmentation using autoencoder regularization]   
2. [Table Compare Models](#2-table-compare-models)   
---
# 1. Models
## 1.1 [Cascaded Anisotropic Convolutional Neural Networks](https://arxiv.org/abs/1709.00382 "link") 
## 1.2 DeepMedic (3D segment)
## 1.3 U-net (2D segment)
## 1.4 EFFICIENT SYMMETRY-DRIVEN FULLY CONVOLUTIONAL NETWORK FOR MULTIMODAL BRAIN TUMOR SEGMENTATION
## 1.5 Boundary-Aware Fully Convolutional Network for Brain Tumor Segmentation
## 1.6 Ensembles of Multiple Models and Architectures for Robust Brain Tumour Segmentation
## 1.7 3D U-Net: Learning Dense Volumetric Segmentation from Sparse Annotation
## 1.8 On the Compactness, Efficiency, and Representation of 3D Convolutional Networks: Brain Parcellation as a Pretext Task
## 1.9 3D MRI brain tumor segmentation using autoencoder regularization

# 2. Table Compare Models
|               Model              	|                                 Input                                	|  Kernel Size 	|     Residual Connection     	| Layer 數 	| 抓取不同深度的  feature map  做 concatenate 	| AAAAAAAAAAAA 	| AAAAAAAAAAA 	| AAAAAAAAAAAAAAAA 	| AAAAAAAAAAAAA 	| AAAAA 	| AAAA 	| AAAA 	|
|:--------------------------------:	|:--------------------------------------------------------------------:	|:------------:	|:---------------------------:	|:--------:	|:-------------------------------------------:	|--------------	|-------------	|------------------	|---------------	|-------	|------	|------	|
|               CACN               	| 以3個不同方向的 MRI train 3 個 model, 144x144x19, 96x96x19, 64x64x19 	| 3x3x1, 1x1x3 	|              Y              	|    26    	|                      Y                      	|              	|             	|                  	|               	|       	|      	|      	|
|             DeepMedic            	|                          25x25x25, 19x19x19                          	|     3x3x3    	|              Y              	|    11    	|                      N                      	|              	|             	|                  	|               	|       	|      	|      	|
|               U-Net              	|                                572x572                               	|      3x3     	|              N              	|    23    	|                      Y                      	|              	|             	|                  	|               	|       	|      	|      	|
|                FCN               	|                              僅水平切面                              	|      3x3     	|              N              	|          	|                                             	|              	|             	|                  	|               	|       	|      	|      	|
| Ensemble (U-Net, DeepMedic, FCN) 	|                                 3D圖                                 	|     3x3x3    	| FCN,U-Net 無,  DeepMedic 有 	|          	|                                             	|              	|             	|                  	|               	|       	|      	|      	|
|              3D-Unet             	|                                                                      	|              	|                             	|          	|                                             	|              	|             	|                  	|               	|       	|      	|      	|
|            HC-default            	|                                 3D圖                                 	|     3x3x3    	|              Y              	|          	|                                             	|              	|             	|                  	|               	|       	|      	|      	|
---
## 1.1 Hello World
