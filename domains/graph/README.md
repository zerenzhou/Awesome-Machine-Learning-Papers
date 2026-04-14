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
    classDef star fill:#FFD700,stroke:#B8860B

    GCN["⭐ GCN (2017)"]:::star --> VGAE["VGAE (2016)"]:::gen
    GCN --> GIN["GIN (2019)"]:::spatial
    GCN --> PretrainGNN["Pre-training GNNs (2020)"]:::pretrain

    GraphSAGE["⭐ GraphSAGE (2017)"]:::star --> GAT["⭐ GAT (2018)"]:::star
    GAT --> GIN
    GAT -.-> GTN["Graph Transformer Networks (2019)"]:::trans
    GraphSAGE --> PretrainGNN

    GIN -.-> MPNN["MPNN Framework (2017)"]:::theory
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Spectral Methods](https://img.shields.io/badge/Spectral_Methods-DBEAFE?style=flat-square) | Graph convolutions defined in the spectral domain via graph Fourier transforms |
| ![Spatial Methods](https://img.shields.io/badge/Spatial_Methods-D1FAE5?style=flat-square) | Message-passing approaches that aggregate neighbor features directly in graph space |
| ![Expressiveness & Theory](https://img.shields.io/badge/Expressiveness_%26_Theory-FED7AA?style=flat-square) | Theoretical analysis of GNN expressiveness, connections to Weisfeiler-Lehman tests |
| ![Graph Transformer](https://img.shields.io/badge/Graph_Transformer-E9D5FF?style=flat-square) | Attention-based architectures adapted for graph-structured data |
| ![Pre-training](https://img.shields.io/badge/Pre--training-FECDD3?style=flat-square) | Self-supervised strategies for learning transferable graph representations |
| ![Generative](https://img.shields.io/badge/Generative-FEF08A?style=flat-square) | Variational and generative models for graph structure generation |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2020](2020.md)
- [2019](2019.md)
- [2016](2016.md)
