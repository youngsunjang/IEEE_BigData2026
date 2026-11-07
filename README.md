# Knowledge-Guided Graph Fusion for Flood Segmentation

Official repository for the paper:

**Knowledge-Guided Graph Fusion for Flood Segmentation in Remote Sensing Imagery**

Zachary J. Cohen-Neamie and Youngsun Jang  
IEEE International Conference on Big Data (BigData 2026)

## Overview

This project presents a knowledge-guided U-Net–GCN fusion
framework for flood segmentation using:

- RGB satellite imagery
- SAR VV/VH observations
- Permanent-water prior information
- SLIC superpixel graphs and graph convolution

The framework integrates multimodal information and
geographic prior knowledge into a U-Net architecture.

## Dataset

SDSU Midwest Flood 2019 Dataset:

https://huggingface.co/datasets/youngsun05/SDSU_MidWest_Flood_2019

Additional SAR observations and permanent-water masks
will be shared through Google Drive.

## Main Experiment

`main-unet_e3_sar_water_gcn1.ipynb`

The notebook implements the proposed E3-level fusion
model with a single GCN layer.

## Installation

Install the required Python packages:

```bash
pip install -r requirements.txt
```

## Code Availability

The implementation will be released following
publication of the paper.

## Results

The proposed model achieved the following validation
performance:

| Metric | Value |
|---|---|
| Global Dice | 0.9039 |
| Global IoU | 0.8246 |
