# Graph Learning

A collection of must-read graph learning papers from top venues.

## Tech Tree

```mermaid
graph TD
    classDef spectral fill:#DBEAFE,stroke:#2563EB
    classDef spatial fill:#D1FAE5,stroke:#059669
    classDef theory fill:#FED7AA,stroke:#EA580C
    classDef trans fill:#E9D5FF,stroke:#7C3AED
    classDef pretrain fill:#FECDD3,stroke:#E11D48
    classDef gen fill:#FEF08A,stroke:#CA8A04
    classDef llm fill:#E0E7FF,stroke:#4F46E5
    classDef star fill:#FFD700,stroke:#B8860B

    GCN["⭐ GCN (2017)"]:::star --> VGAE["VGAE (2016)"]:::gen
    GCN --> GIN["GIN (2019)"]:::spatial
    GCN --> PretrainGNN["Pre-training GNNs (2020)"]:::pretrain

    GraphSAGE["⭐ GraphSAGE (2017)"]:::star --> GAT["⭐ GAT (2018)"]:::star
    GAT --> GIN
    GAT -.-> GTN["Graph Transformer Networks (2019)"]:::trans
    GraphSAGE --> PretrainGNN

    GIN -.-> MPNN["MPNN Framework (2017)"]:::theory

    GTN --> GPS["GPS (2023)"]:::trans
    GPS --> Exphormer["Exphormer (2023)"]:::trans

    PretrainGNN --> GraphMAE2["GraphMAE2 (2023)"]:::pretrain
    PretrainGNN --> PRODIGY["PRODIGY (2023)"]:::pretrain
    PRODIGY --> OneForAll["One for All (2024)"]:::pretrain
    OneForAll --> GraphAny["GraphAny (2024)"]:::pretrain
    PRODIGY -.-> ULTRA["ULTRA (2024)"]:::pretrain

    OneForAll --> GOFA["GOFA (2025)"]:::llm
    OneForAll -.-> RAG4GFM["RAG4GFM (2025)"]:::pretrain
    GraphAny -.-> RAG4GFM

    VGAE --> DiGress["DiGress (2023)"]:::gen
    DiGress --> LayerDAG["LayerDAG (2025)"]:::gen
    DiGress --> DeFoG["DeFoG (2025)"]:::gen

    GAT -.-> GraphGPT["GraphGPT (2023)"]:::llm
    GraphGPT --> LLaGA["LLaGA (2024)"]:::llm
    GraphGPT --> InstructGraph["InstructGraph (2024)"]:::llm
    LLaGA -.-> GOFA
    RAG4GFM --> GFMRAG["GFM-RAG (2025)"]:::llm
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Spectral Methods](https://img.shields.io/badge/Spectral_Methods-DBEAFE?style=flat-square) | Graph convolutions defined in the spectral domain via graph Fourier transforms |
| ![Spatial Methods](https://img.shields.io/badge/Spatial_Methods-D1FAE5?style=flat-square) | Message-passing approaches that aggregate neighbor features directly in graph space |
| ![Expressiveness & Theory](https://img.shields.io/badge/Expressiveness_%26_Theory-FED7AA?style=flat-square) | Theoretical analysis of GNN expressiveness, connections to Weisfeiler-Lehman tests |
| ![Graph Transformer](https://img.shields.io/badge/Graph_Transformer-E9D5FF?style=flat-square) | Attention-based architectures adapted for graph-structured data, from local+global (GPS) to sparse (Exphormer) |
| ![Pre-training & Foundation](https://img.shields.io/badge/Pre--training_%26_Foundation-FECDD3?style=flat-square) | Self-supervised and foundation model strategies for transferable graph representations across diverse domains |
| ![Generative](https://img.shields.io/badge/Generative-FEF08A?style=flat-square) | Variational and diffusion-based generative models for graph structure generation |
| ![LLM + Graph](https://img.shields.io/badge/LLM_%2B_Graph-E0E7FF?style=flat-square) | Methods integrating large language models with GNNs for text-based graph reasoning and instruction following |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2026](2026.md)
- [2025](2025.md)
- [2024](2024.md)
- [2023](2023.md)
- [2020](2020.md)
- [2019](2019.md)
- [2016](2016.md)
