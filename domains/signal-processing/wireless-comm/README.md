# Wireless & Communication Signals

Deep learning for physical-layer communications: autoencoder-based transceivers, modulation recognition, channel estimation, CSI feedback, MIMO detection, and semantic / joint source-channel coding.

## Tech Tree

```mermaid
graph TD
    classDef comm fill:#D1FAE5,stroke:#059669
    classDef unroll fill:#DBEAFE,stroke:#2563EB
    classDef star fill:#FFD700,stroke:#B8860B

    ModRec["⭐ Mod. Recognition (2016)"]:::star --> RadioML["RadioML Dataset (2016)"]:::comm
    ModRec --> OTA["OTA Classification (2018)"]:::comm
    Autoencoder["⭐ DL Physical Layer (2017)"]:::star --> OTAComm["DL Over the Air (2018)"]:::comm
    Autoencoder --> OFDM["DL for OFDM (2018)"]:::comm
    Autoencoder --> CsiNet["CsiNet (2018)"]:::comm
    Autoencoder --> DJSCC["Deep JSCC (2019)"]:::comm
    OFDM --> ChannelEst["DL Channel Est. (2019)"]:::comm
    DJSCC --> NTSCC["NTSCC (2022)"]:::comm
    Autoencoder --> BeyondBits["Beyond Bits (2023)"]:::comm

    DetNet["DetNet (2019)"]:::unroll --> OAMPNet["OAMP-Net (2020)"]:::unroll
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Communications & Wireless](https://img.shields.io/badge/Communications_%26_Wireless-D1FAE5?style=flat-square) | Deep learning for physical-layer problems: autoencoder-based transceivers, modulation recognition, channel estimation, CSI feedback, semantic communications |
| ![Algorithm Unrolling](https://img.shields.io/badge/Algorithm_Unrolling-DBEAFE?style=flat-square) | Unrolling iterative optimization algorithms (projected gradient, AMP) into trainable networks for MIMO detection |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Benchmark Datasets

| Dataset | Task | Scale | Description |
|:---|:---|:---|:---|
| **RadioML 2016.10a / 10b** | Modulation recognition | 220k / 1.2M samples, 11 classes | GNU Radio synthetic RF signals over varying SNR; DeepSig benchmark |
| **RadioML 2018.01a** | Modulation recognition | 2.56M samples, 24 classes | Over-the-air captures plus synthetic channels |
| **CSI Dataset (COST2100)** | CSI feedback | — | Standard channel for CsiNet-family evaluation |
| **DeepMIMO** | MIMO / beam prediction | Ray-tracing | Parametrized mmWave and massive-MIMO channel dataset |
| **ViWi / Raymobtime** | V2X / beam selection | Multi-modal | Vision-aided / ray-traced channel datasets |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2023](2023.md) — Semantic / task-oriented communications tutorial
- [2022](2022.md) — Nonlinear transform source-channel coding (NTSCC)
- [2020](2020.md) — OAMP-Net MIMO detection
- [2019](2019.md) — DetNet · Deep JSCC · DL channel estimation
- [2018](2018.md) — End-to-end OTA communication · OFDM · CsiNet · OTA radio classification
- [2017](2017.md) — ⭐ Physical-layer autoencoder
- [2016](2016.md) — ⭐ Modulation recognition · RadioML dataset
