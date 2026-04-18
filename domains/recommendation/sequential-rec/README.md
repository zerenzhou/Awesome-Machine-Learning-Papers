# Sequential Recommendation

Sequential recommendation models the user's full interaction history to predict the next item. Evolved from Markov chains (FPMC) → RNN (GRU4Rec) → Transformer (SASRec, BERT4Rec) → self-supervised and contrastive methods.

## Tech Tree

```mermaid
graph TD
    classDef rnn fill:#DBEAFE,stroke:#2563EB
    classDef cnn fill:#D1FAE5,stroke:#059669
    classDef transformer fill:#E9D5FF,stroke:#7C3AED
    classDef contrastive fill:#FCE7F3,stroke:#DB2777
    classDef diffusion fill:#FEF08A,stroke:#CA8A04
    classDef star fill:#FFD700,stroke:#B8860B

    FPMC["FPMC (2010)"]:::rnn --> GRU4Rec["⭐ GRU4Rec (2016)"]:::star
    GRU4Rec --> Caser["Caser (2018)"]:::cnn
    GRU4Rec --> SASRec["⭐ SASRec (2018)"]:::star
    SASRec --> BERT4Rec["BERT4Rec (2019)"]:::transformer
    SASRec --> TiSASRec["TiSASRec (2020)"]:::transformer
    SASRec --> SSSRec["S³-Rec (2020)"]:::contrastive
    BERT4Rec --> CL4SRec["⭐ CL4SRec (2022)"]:::star
    CL4SRec --> DuoRec["DuoRec (2022)"]:::contrastive
    SASRec -.-> DiffRec["DiffRec (2023)"]:::diffusion
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![RNN-based](https://img.shields.io/badge/RNN--based-DBEAFE?style=flat-square) | RNN/GRU-based sequential models (GRU4Rec, FPMC) |
| ![Convolutional](https://img.shields.io/badge/Convolutional-D1FAE5?style=flat-square) | Convolutional sequential models (Caser) |
| ![Transformer](https://img.shields.io/badge/Transformer-E9D5FF?style=flat-square) | Attention-based sequential models (SASRec, BERT4Rec) |
| ![Contrastive](https://img.shields.io/badge/Contrastive-FCE7F3?style=flat-square) | Self-supervised / contrastive learning (CL4SRec, DuoRec) |
| ![Diffusion](https://img.shields.io/badge/Diffusion-FEF08A?style=flat-square) | Diffusion-based sequential models (DiffRec) |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — Pre-deep foundational works
- [2016](2016.md)
- [2018](2018.md)
- [2019](2019.md)
- [2020](2020.md)
- [2022](2022.md)
- [2023](2023.md)
