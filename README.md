# [AAAI 2025] HybridReg: Robust 3D Point Cloud Registration with Hybrid Motions

<h4 align = "center">Keyu Du<sup>1</sup>, Hao Xu<sup>2</sup>, Haipeng Li<sup>1</sup>, Hong Qu<sup>1</sup>, Chi-Wing Fu<sup>2</sup>, Shuaicheng Liu<sup>1</sup></h4>
<h4 align = "center"> <sup>1</sup>University of Electronic Science and Technology of China (UESTC)</center></h4>
<h4 align = "center"> <sup>2</sup>The Chinese University of Hong Kong (CUHK)</center></h4>

This is the official implementation of our AAAI2025 paper, HybridReg: Robust 3D Point Cloud Registration with Hybrid Motions.

## Introduction
Scene-level point cloud registration is very challenging when considering dynamic foregrounds. Existing indoor datasets mostly assume rigid motions, so the trained models can not robustly handle scenes with non-rigid motions. On the other hand, non-rigid datasets are mainly object-level, so the trained models cannot generalize well to complex scenes.  
This paper presents HybridReg, a new approach to 3D point cloud registration, learning uncertainty mask to account for hybrid motions: rigid for backgrounds and non-rigid/rigid for
instance-level foregrounds. First, we build a scene-level 3D registration dataset, namely HybridMatch, designed specifically with strategies to arrange diverse deforming foregrounds in a controllable manner. Second, we account for different motion types and formulate a mask-learning module to alleviate the interference of deforming outliers. Third, we exploit a simple yet effective negative log-likelihood loss to adopt uncertainty to guide the feature extraction and correlation computation. To our best knowledge, HybridReg is the first work that exploits hybrid motions for robust point cloud registration. Extensive experiments show HybridReg’s strengths, leading it to achieve state-of-the-art performance on both widely-used indoor and outdoor datasets.

![image text](./pipeline.png)

## Installation

## Data Preparation
Our scene-level 3D registration dataset HybridMatch can be downloaded from [HybridMatch](https://huggingface.co/datasets/kinseyxyz/HybridMatch).
