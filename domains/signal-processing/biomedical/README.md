# Biomedical Signals

Deep learning for physiological signal decoding: EEG-based brain-computer interfaces, ECG arrhythmia classification, wearable biosignals (PPG), and large-scale biosignal foundation models. Papers are listed in reverse chronological order; ⭐ marks pioneering works.

## 2025

- **NeuroLM: A Universal Multi-task Foundation Model for Bridging the Gap between Language and EEG Signals** — ICLR 2025 [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2409.00101)] [[Code](https://github.com/935963004/NeuroLM)]
  First multi-task EEG foundation model treating EEG as a foreign language for LLMs, with the 1.7B-parameter NeuroLM-XL pre-trained on ~25,000 hours of EEG achieving SOTA across six BCI tasks.

- **CBraMod: A Criss-Cross Brain Foundation Model for EEG Decoding** — ICLR 2025 [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2412.07236)] [[Code](https://github.com/wjq-learning/CBraMod)]
  Proposed a criss-cross transformer separately modeling spatial and temporal EEG dependencies, pre-trained via patch-based masked reconstruction, achieving SOTA across 10 BCI tasks on 12 datasets.

## 2024

- **Large Brain Model for Learning Generic Representations with Tremendous EEG Data in BCI** — ICLR 2024 Spotlight [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2405.18765)] [[Code](https://github.com/935963004/LaBraM)]
  First large-scale EEG foundation model (LaBraM) pre-trained on ~2,500 hours of EEG from ~20 datasets via vector-quantized neural spectrum prediction, achieving SOTA across diverse BCI tasks.

- **Large-scale Training of Foundation Models for Wearable Biosignals** — ICLR 2024 [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2312.05409)]
  First foundation model for PPG and ECG biosignals pre-trained via self-supervised contrastive learning on 141K participants, demonstrating strong transfer to cardiovascular and activity tasks.

## 2023

- **BrainBERT: Self-supervised Representation Learning for Intracranial Recordings** — ICLR 2023 [`Foundation Model`]
  [[Paper](https://arxiv.org/abs/2302.14367)] [[Code](https://github.com/czlwang/BrainBERT)]
  Applied BERT-style masked pre-training to intracranial EEG spectrograms, producing reusable representations that generalize across subjects and reduce labeled data requirements by up to 85%.

## 2020

- **Automatic Diagnosis of the 12-Lead ECG Using a Deep Neural Network** — Nature Communications 2020
  [[Paper](https://arxiv.org/abs/1904.01949)] [[Code](https://github.com/antonior92/automatic-ecg-diagnosis)]
  Trained a DNN on over 2 million 12-lead ECGs to diagnose 6 cardiac abnormalities, outperforming cardiology residents with F1 scores above 80% and specificity over 99%.

## 2019

- **Cardiologist-Level Arrhythmia Detection and Classification in Ambulatory Electrocardiograms Using a Deep Neural Network** — Nature Medicine 2019
  [[Paper](https://www.nature.com/articles/s41591-018-0268-3)] [[Code](https://github.com/awni/ecg)]
  Validated that a 34-layer CNN trained on 91,232 single-lead ECGs from 53,549 patients exceeds average cardiologist performance (F1: 0.837 vs. 0.780) in 12-class arrhythmia detection.

## 2018

- ⭐ **EEGNet: A Compact Convolutional Neural Network for EEG-Based Brain-Computer Interfaces** — Journal of Neural Engineering 2018
  [[Paper](https://arxiv.org/abs/1611.08024)] [[Code](https://github.com/vlawhern/arl-eegmodels)]
  Introduced a compact CNN using depthwise and separable convolutions for EEG-based BCI, generalizing across P300, ERN, MRCP, and SMR paradigms with an order of magnitude fewer parameters — the standard compact model for EEG-BCI.

## 2017

- **Deep Learning with Convolutional Neural Networks for EEG Decoding and Visualization** — Human Brain Mapping 2017
  [[Paper](https://arxiv.org/abs/1703.05051)] [[Code](https://github.com/braindecode/braindecode)]
  Showed that deep ConvNets with batch normalization and cropped training match or exceed FBCSP for EEG decoding, with novel visualization of learned spectral-spatial features.

## Benchmark Datasets

| Dataset | Modality | Scale | Description |
|:---|:---|:---|:---|
| **BCI Competition IV (2a/2b)** | EEG | 9 subjects | Motor-imagery BCI benchmark; EEGNet evaluation |
| **PhysioNet MI** | EEG | 109 subjects | EEG Motor Movement/Imagery Dataset |
| **TUH EEG Corpus (TUEG)** | EEG | 30k+ recordings, 69k patients | Largest open clinical EEG corpus; pretraining corpus for LaBraM/CBraMod |
| **SEED / SEED-IV / DEAP** | EEG | — | Emotion recognition benchmarks |
| **MIT-BIH Arrhythmia** | ECG | 48 records | Classic ECG arrhythmia benchmark |
| **PhysioNet Challenge 2017 / 2020 / 2021** | ECG | 8k–88k records | Atrial fibrillation / 12-lead diagnosis challenges |
| **CPSC2018** | 12-lead ECG | 6,877 records | Chinese Physiological Signal Challenge; standard clinical ECG benchmark |
| **PTB-XL** | 12-lead ECG | 21,837 records | Large public clinical ECG dataset for supervised learning |
| **MIMIC-III / MIMIC-IV (waveforms)** | Multi-signal | 50k+ patients | ICU physiological signals for multi-task biosignal foundation models |
