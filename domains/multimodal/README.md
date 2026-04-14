# Multimodal Learning

A collection of must-read multimodal learning papers from top venues.

## Tech Tree

```mermaid
graph TD
    classDef early fill:#DBEAFE,stroke:#2563EB
    classDef contrastive fill:#D1FAE5,stroke:#059669
    classDef vlm fill:#FED7AA,stroke:#EA580C
    classDef unified fill:#E9D5FF,stroke:#7C3AED
    classDef star fill:#FFD700,stroke:#B8860B

    ViLBERT["⭐ ViLBERT (2019)"]:::star --> CLIP["⭐ CLIP (2021)"]:::star
    CLIP --> ALIGN["ALIGN (2021)"]:::contrastive
    CLIP --> Flamingo["Flamingo (2022)"]:::vlm
    Flamingo --> BLIP2["BLIP-2 (2023)"]:::vlm
    BLIP2 --> LLaVA["LLaVA (2023)"]:::vlm
    CLIP --> ImageBind["ImageBind (2023)"]:::unified
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Early Vision-Language](https://img.shields.io/badge/Early_Vision--Language-DBEAFE?style=flat-square) | First dual-stream architectures jointly modeling vision and language modalities |
| ![Contrastive Learning](https://img.shields.io/badge/Contrastive_Learning-D1FAE5?style=flat-square) | Methods aligning image and text representations in a shared embedding space via contrastive objectives |
| ![Visual Language Models](https://img.shields.io/badge/Visual_Language_Models-FED7AA?style=flat-square) | Large models integrating frozen LLMs with visual encoders for multimodal understanding and generation |
| ![Unified Embedding](https://img.shields.io/badge/Unified_Embedding-E9D5FF?style=flat-square) | Models that align more than two modalities (image, text, audio, depth, etc.) into a single representation space |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2023](2023.md)
- [2022](2022.md)
- [2021](2021.md)
