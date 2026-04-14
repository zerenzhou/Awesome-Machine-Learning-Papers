# Speech & Audio

A collection of must-read speech and audio processing papers from top venues.

## Tech Tree

```mermaid
graph TD
    classDef e2e fill:#DBEAFE,stroke:#2563EB
    classDef hybrid fill:#D1FAE5,stroke:#059669
    classDef gen fill:#E9D5FF,stroke:#7C3AED
    classDef star fill:#FFD700,stroke:#B8860B

    DeepSpeech["⭐ Deep Speech 2 (2016)"]:::star --> wav2vec["⭐ wav2vec 2.0 (2020)"]:::star
    wav2vec --> HuBERT["HuBERT (2021)"]:::e2e
    wav2vec --> Whisper["Whisper (2023)"]:::e2e
    wav2vec -.-> Conformer["Conformer (2020)"]:::hybrid

    WaveNet["⭐ WaveNet (2016)"]:::star --> DiffWave["DiffWave (2021)"]:::gen
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![End-to-End Recognition](https://img.shields.io/badge/End--to--End_Recognition-DBEAFE?style=flat-square) | Models that directly map raw audio to text, eliminating hand-crafted feature pipelines |
| ![Hybrid Architecture](https://img.shields.io/badge/Hybrid_Architecture-D1FAE5?style=flat-square) | Designs combining convolution and self-attention for joint local and global audio modeling |
| ![Audio Generation](https://img.shields.io/badge/Audio_Generation-E9D5FF?style=flat-square) | Neural vocoders and generative models that synthesize high-fidelity audio waveforms |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2024](2024.md)
- [2023](2023.md)
- [2021](2021.md)
- [2020](2020.md)
