# Image & Video Signal Processing

Deep learning for image/video reconstruction and inverse problems — compressive sensing image recovery, MRI/CT reconstruction, and diffusion-based solvers for general noisy inverse problems. This subdomain overlaps with computer vision but is included because its methodology (sampling operators, forward models, iterative solvers) is fundamentally signal-processing.

## Tech Tree

```mermaid
graph TD
    classDef cs fill:#FECDD3,stroke:#E11D48
    classDef unroll fill:#DBEAFE,stroke:#2563EB
    classDef star fill:#FFD700,stroke:#B8860B

    ADMMNet["ADMM-Net (2016)"]:::unroll --> ISTANet["ISTA-Net (2018)"]:::unroll
    CSGen["⭐ CS Generative (2017)"]:::star --> LDAMP["Learned D-AMP (2017)"]:::cs
    CSGen --> DeepInverse["DeepInverse (2017)"]:::cs
    CSGen --> DeepCS["Deep CS (2019)"]:::cs
    CSGen -.-> ScoreIP["Score-Based IP (2022)"]:::cs
    ScoreIP --> DPS["DPS (2023)"]:::cs
    ScoreIP --> AmbientDiff["Ambient Diffusion (2023)"]:::cs
    DPS --> ReSample["ReSample (2024)"]:::cs
    DPS --> DiffStateGrad["DiffStateGrad (2025)"]:::cs
    DeepCS -.-> IDM["IDM (2025)"]:::cs
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Compressed Sensing & Inverse Problems](https://img.shields.io/badge/CS_%26_Inverse_Problems-FECDD3?style=flat-square) | Learned measurement and reconstruction for compressive sensing and inverse problems, from generative priors to diffusion-based solvers |
| ![Algorithm Unrolling](https://img.shields.io/badge/Algorithm_Unrolling-DBEAFE?style=flat-square) | Deep networks derived by unrolling iterative optimization algorithms (ISTA, ADMM) for image reconstruction |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Benchmark Datasets

| Dataset | Task | Description |
|:---|:---|:---|
| **Set11 / BSD68 / Urban100** | CS image reconstruction | Natural-image benchmarks reused for CS evaluation |
| **fastMRI** | MRI reconstruction | 1,500+ knee / brain MRI volumes; standard undersampled reconstruction benchmark |
| **Calgary-Campinas / SKM-TEA** | MRI reconstruction | Multi-coil brain / knee MRI benchmarks |
| **Mayo Low-Dose CT** | CT reconstruction | AAPM Low-Dose CT Grand Challenge data |
| **FFHQ / ImageNet validation** | Diffusion inverse problems | Used by DPS, ReSample, IDM, DiffStateGrad |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2025](2025.md) — DiffStateGrad · IDM invertible diffusion CS
- [2024](2024.md) — ReSample latent-diffusion inverse solver
- [2023](2023.md) — DPS · Ambient Diffusion
- [2022](2022.md) — Score-based inverse problems for medical imaging
- [2019](2019.md) — Deep Compressed Sensing (meta-learning)
- [2018](2018.md) — ISTA-Net unrolled image CS
- [2017](2017.md) — ⭐ CS Generative · Learned D-AMP · DeepInverse
- [2016](2016.md) — Deep ADMM-Net for CS MRI
