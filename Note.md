# Table of Contents
### 1. [Models](#1-models)
### 2. [Table Compare Models](#2-table-compare-models)
---
# 1. Models
## 1.1 Cascaded Anisotropic Convolutional Neural Networks

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


123