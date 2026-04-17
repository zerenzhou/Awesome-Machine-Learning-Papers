# Mechanical Fault Diagnosis (Vibration Signals)

Deep learning for rotating-machinery fault diagnosis and prognosis health management (PHM): bearing and gearbox fault classification from vibration / acoustic signals, cross-working-condition domain adaptation, and GNN-based machine fault diagnosis. Papers are listed in reverse chronological order; ⭐ marks pioneering works.

## 2021

- **Multireceptive Field Graph Convolutional Networks for Machine Fault Diagnosis** — IEEE TIE 2021 [`GNN`]
  [[Paper](https://ieeexplore.ieee.org/document/9122502)]
  Proposed MRF-GCN that constructs graphs from vibration segments and fuses features across multiple receptive fields, introducing graph neural networks to intelligent fault diagnosis and outperforming CNN baselines on CWRU and gearbox datasets.

- **Applications of Unsupervised Deep Transfer Learning to Intelligent Fault Diagnosis: A Survey and Comparative Study** — IEEE TIM 2021 [`Survey`] [`Domain Adaptation`]
  [[Paper](https://arxiv.org/abs/1912.12528)]
  Systematic benchmark of unsupervised deep transfer learning methods for cross-domain fault diagnosis, covering feature-based, adversarial, and distribution-alignment approaches with a unified evaluation protocol.

## 2020

- ⭐ **Applications of Machine Learning to Machine Fault Diagnosis: A Review and Roadmap** — MSSP 2020 [`Survey`]
  [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0888327019306321)]
  Authoritative review covering traditional ML, deep learning, and transfer learning for machine fault diagnosis, with a roadmap identifying challenges in small samples, imbalanced data, compound faults, and cross-domain generalization.

## 2019

- **Deep Learning and Its Applications to Machine Health Monitoring** — MSSP 2019 [`Survey`]
  [[Paper](https://arxiv.org/abs/1612.07640)]
  First comprehensive survey on deep learning for PHM, systematically covering Auto-Encoders, RBMs, CNNs, and RNNs across machine health monitoring tasks including fault diagnosis and remaining-useful-life prediction.

## 2018

- **A New Convolutional Neural Network-Based Data-Driven Fault Diagnosis Method** — IEEE TIE 2018 [`CNN`]
  [[Paper](https://ieeexplore.ieee.org/document/8114247)]
  Converted 1D vibration signals to 2D images and applied a LeNet-style CNN for end-to-end fault classification, widely adopted baseline for time-frequency image input schemes.

## 2017

- **A New Deep Learning Model for Fault Diagnosis with Good Anti-Noise and Domain Adaptation Ability on Raw Vibration Signals (WDCNN)** — Sensors 2017 [`CNN`]
  [[Paper](https://www.mdpi.com/1424-8220/17/2/425)]
  Proposed WDCNN with wide first-layer kernels on raw 1D vibration signals, combining AdaBN for domain adaptation — became a de-facto baseline for bearing fault diagnosis benchmarks.

- **Deep Model Based Domain Adaptation for Fault Diagnosis** — IEEE TIE 2017 [`Domain Adaptation`]
  [[Paper](https://ieeexplore.ieee.org/document/7593253)]
  Early application of deep domain adaptation (MMD-based feature alignment) to fault diagnosis, enabling transfer across working conditions without target-domain labels.

## 2016

- ⭐ **Deep Neural Networks: A Promising Tool for Fault Characteristic Mining and Intelligent Diagnosis of Rotating Machinery with Massive Data** — MSSP 2016 [`DNN`]
  [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0888327015004859)]
  Pioneering application of deep neural networks to rotating-machinery fault diagnosis using frequency-spectrum features, demonstrating that DL can automatically mine fault-characteristic representations from massive data.

- **Convolutional Neural Network Based Fault Detection for Rotating Machinery** — Journal of Sound and Vibration 2016 [`CNN`]
  [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0022460X16001905)]
  First CNN-based fault detection system for rotating machinery, processing discrete Fourier transforms of accelerometer signals to classify healthy and faulty bearing conditions.

## Benchmark Datasets

| Dataset | Modality | Scale | Description |
|:---|:---|:---|:---|
| **CWRU Bearing** | Vibration | 4 fault types × multi-load | Case Western Reserve University bearing dataset — the de-facto standard benchmark for bearing fault diagnosis |
| **Paderborn (KAT)** | Vibration + Current | 32 bearings, real + artificial damage | Paderborn University bearing dataset with accelerated life-test and artificial damage classes |
| **MFPT** | Vibration | Baseline + outer/inner race faults | Machinery Failure Prevention Technology bearing dataset |
| **PHM 2009 Gearbox** | Vibration | 8 health conditions | PHM Society 2009 data challenge gearbox dataset |
| **XJTU-SY Bearing** | Run-to-failure vibration | 15 bearings, 3 conditions | Xi'an Jiaotong / Changxing Sumyoung run-to-failure dataset for RUL prediction |
| **IMS Bearing** | Run-to-failure vibration | 4 bearings × 3 run-to-failure tests | NASA IMS dataset for degradation / RUL modeling |
| **JNU / SEU Bearing** | Vibration | Multi-condition | Jiangnan / Southeast University datasets used in DTL benchmarks |
