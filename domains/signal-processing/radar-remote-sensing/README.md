# Radar & Remote Sensing Signals

Deep learning for SAR automatic target recognition, remote-sensing scene classification, direction-of-arrival estimation, and multi-modal (optical + SAR + multispectral) foundation models. Papers are listed in reverse chronological order; ⭐ marks pioneering works.

## 2025

- **SARATR-X: Toward Building A Foundation Model for SAR Target Recognition** — IEEE TIP 2025 [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2405.09365)] [[Code](https://github.com/waterdisappear/SARATR-X)]
  First foundation model for SAR ATR trained on 0.18M unlabelled SAR samples via self-supervised learning with multi-scale gradient features, matching supervised methods in few-shot settings.

## 2024

- **SpectralGPT: Spectral Remote Sensing Foundation Model** — IEEE TPAMI 2024 [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2311.07113)] [[Code](https://github.com/danfenghong/IEEE_TPAMI_SpectralGPT)]
  First foundation model for spectral remote sensing using a 3D generative pre-trained transformer on 1M+ spectral images with progressive training across varying resolutions and regions.

- **SkySense: A Multi-Modal Remote Sensing Foundation Model Towards Universal Interpretation for Earth Observation Imagery** — CVPR 2024 [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2312.10115)] [[Code](https://github.com/Jack-bo1220/SkySense)]
  Largest multi-modal RS foundation model pre-trained on 21.5M temporal sequences of optical and SAR data, surpassing 18 prior RSFMs across 16 datasets and 7 tasks.

## 2023

- **RingMo: A Remote Sensing Foundation Model with Masked Image Modeling** — IEEE TGRS 2023 [`Foundation Model`]
  [[Paper](https://ieeexplore.ieee.org/document/10105625)]
  Built a 2M-image RS pre-training dataset with density-aware masking, achieving SOTA on 8 benchmarks across scene classification, detection, segmentation, and change detection.

## 2022

- **SatMAE: Pre-training Transformers for Temporal and Multi-Spectral Satellite Imagery** — NeurIPS 2022 [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2207.08051)] [[Code](https://github.com/sustainlab-group/SatMAE)]
  Adapted masked autoencoder pre-training to multi-spectral and temporal satellite imagery with spectral positional encodings, improving downstream RS tasks by up to 14%.

## 2021

- **Deep-Learning for Radar: A Survey** — IEEE Access 2021
  [[Paper](https://ieeexplore.ieee.org/document/9568916)]
  Comprehensive survey covering deep learning for radar waveform design, LPI recognition, SAR/HRRP-based automatic target recognition, and jamming/clutter suppression.

## 2020

- **DeepMUSIC: Multiple Signal Classification via Deep Learning** — IEEE Sensors Letters 2020
  [[Paper](https://arxiv.org/abs/1912.04357)]
  Designed multiple CNNs each dedicated to angular subregions for multi-source DOA estimation, achieving superior accuracy and lower complexity than both classical and DL-based methods.

## 2017

- **Remote Sensing Image Scene Classification: Benchmark and State of the Art** — Proceedings of the IEEE 2017
  [[Paper](https://arxiv.org/abs/1703.00121)]
  Introduced the NWPU-RESISC45 benchmark (31,500 images, 45 scene classes) and provided comprehensive evaluation of deep learning methods for remote sensing scene classification.

## 2016

- ⭐ **Target Classification Using the Deep Convolutional Networks for SAR Images** — IEEE TGRS 2016
  [[Paper](https://ieeexplore.ieee.org/document/7460942)]
  Proposed all-convolutional networks (A-ConvNets) without fully connected layers for SAR automatic target recognition on the MSTAR dataset, addressing overfitting from limited training data.

## Benchmark Datasets

| Dataset | Modality | Classes / Scale | Description |
|:---|:---|:---|:---|
| **MSTAR** | SAR | 10 vehicle classes, ~6k chips | X-band SAR target recognition benchmark (SOC / EOC) |
| **OpenSARShip / FUSAR-Ship** | SAR | ship types | Sentinel-1 / Gaofen-3 SAR ship classification |
| **UC Merced Land Use** | Optical | 21 classes × 100 | Early remote sensing scene classification benchmark |
| **AID** | Optical | 30 classes × ~300 | Aerial-image scene classification |
| **NWPU-RESISC45** | Optical | 45 classes × 700 | Standard remote-sensing scene classification benchmark |
| **DOTA / DOTA-v2.0** | Aerial | 18 object classes | Oriented object detection in aerial imagery |
| **BigEarthNet-S1/S2** | SAR + Multispectral | 590k patches, 43 labels | Sentinel-1/2 multi-label land-cover benchmark for remote-sensing foundation models |
| **SEN1-2 / SEN12MS** | SAR + Optical | 180k / 541k | Paired Sentinel-1/2 dataset for multimodal remote sensing |
| **fMoW / xView / iSAID** | High-res aerial | 1M / 1M / 655k objects | Functional map, general detection, and instance segmentation benchmarks |
