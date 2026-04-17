# Biomedical Signals

Deep learning for physiological signal decoding: EEG-based brain-computer interfaces, ECG arrhythmia classification, wearable biosignals (PPG), and large-scale biosignal foundation models.

## Tech Tree

```mermaid
graph TD
    classDef bio fill:#E9D5FF,stroke:#7C3AED
    classDef fm fill:#E0E7FF,stroke:#4F46E5
    classDef star fill:#FFD700,stroke:#B8860B

    EEGDecode["EEG Decoding (2017)"]:::bio --> EEGNet["⭐ EEGNet (2018)"]:::star
    ECG["ECG Nature Med (2019)"]:::bio --> ECG12Lead["12-Lead ECG DNN (2020)"]:::bio
    EEGNet -.-> BrainBERT["BrainBERT (2023)"]:::fm
    BrainBERT --> LaBraM["LaBraM (2024)"]:::fm
    LaBraM --> NeuroLM["NeuroLM (2025)"]:::fm
    LaBraM --> CBraMod["CBraMod (2025)"]:::fm
    ECG12Lead -.-> WearableFM["Wearable FM (2024)"]:::fm
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Biomedical Signal Processing](https://img.shields.io/badge/Biomedical_Signal-E9D5FF?style=flat-square) | Deep learning for EEG-based brain-computer interfaces, ECG arrhythmia classification, and physiological signal decoding |
| ![Foundation Models](https://img.shields.io/badge/Foundation_Models-E0E7FF?style=flat-square) | Large-scale pre-trained models for EEG/ECG biosignals enabling transfer learning and few-shot generalization |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

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

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2025](2025.md) — NeuroLM · CBraMod large EEG foundation models
- [2024](2024.md) — LaBraM · Wearable biosignal foundation models
- [2023](2023.md) — BrainBERT intracranial EEG pre-training
- [2020](2020.md) — 12-lead ECG DNN clinical validation
- [2019](2019.md) — Cardiologist-level ECG arrhythmia detection
- [2018](2018.md) — ⭐ EEGNet compact CNN for BCI
- [2017](2017.md) — Braindecode deep EEG decoding
