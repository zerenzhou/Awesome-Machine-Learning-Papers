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

## Benchmark Datasets

### Node Classification (Citation / Social)

| Dataset | Nodes / Edges | Task | Description |
|:---|:---|:---|:---|
| **Cora** | 2.7k / 5.4k | 7-class | Citation network benchmark introduced by GCN; small-scale semi-supervised classification |
| **Citeseer** | 3.3k / 4.7k | 6-class | Classic citation benchmark alongside Cora |
| **Pubmed** | 19.7k / 44k | 3-class | Diabetes publication citation network |
| **Reddit** | 233k / 11.6M | 41-class | Post-community classification (GraphSAGE benchmark) |
| **Flickr / Yelp / AmazonProducts** | 89k–1.6M | Multi-label | Inductive node classification benchmarks from GraphSAINT |
| **ogbn-arxiv / products / papers100M** | 169k / 2.4M / 111M | Node classification | OGB large-scale citation / co-purchase / academic benchmarks |
| **ogbn-mag / mag240M** | 1.9M / 240M | Heterogeneous | Heterogeneous academic graph (papers/authors/institutions) |

### Link Prediction & Knowledge Graphs

| Dataset | Entities / Relations | Description |
|:---|:---|:---|
| **FB15k-237** | 14.5k / 237 | Filtered Freebase subset; standard KGE benchmark |
| **WN18RR** | 40.9k / 11 | WordNet subset for link prediction |
| **ogbl-ppa / citation2 / collab / ddi** | OGB | Protein-protein / citation / collaboration / drug-drug edge tasks |
| **YAGO3-10 / NELL-995** | — | Additional KG completion benchmarks |

### Graph Classification & Regression

| Dataset | Graphs | Task | Description |
|:---|:---|:---|:---|
| **TUDataset** | 120+ collections | Various | Bioinformatics and social graph benchmarks (MUTAG, PROTEINS, IMDB-B, etc.) |
| **ogbg-molhiv / molpcba** | 41k / 438k molecules | Binary / multi-label | Molecular property prediction (OGB) |
| **ogbg-ppa / ogbg-code2** | 158k / 452k | Multi-class / sequence | Protein associations / code abstract-syntax graphs |
| **ZINC / ZINC-250K** | 12k / 250k molecules | Regression | Constrained solubility regression; canonical graph-regression benchmark |
| **QM9** | 134k molecules | Multi-task regression | Quantum properties of small organic molecules |
| **MoleculeNet** | 17 datasets | Mixed | Drug-discovery benchmark suite |
| **PCQM4Mv2** | 3.8M molecules | DFT energy regression | OGB-LSC graph-regression track |

### Spatio-Temporal Graphs

| Dataset | Nodes | Frequency | Description |
|:---|:---|:---|:---|
| **METR-LA** | 207 sensors | 5min | LA highway speed (DCRNN benchmark) |
| **PEMS-BAY / PEMS03/04/07/08** | 325 / 170–883 | 5min | California traffic flow/speed; standard for STGNN work |

### Graph Foundation Models & Benchmarks

| Dataset | Scale | Description |
|:---|:---|:---|
| **OGB (Open Graph Benchmark)** | 15 datasets | Unified node/link/graph benchmark with standardized splits |
| **OGB-LSC** | 3 datasets | Large-scale challenge track (MAG240M-LSC, WikiKG90Mv2-LSC, PCQM4Mv2-LSC) |
| **PRODIGY Chem/Arxiv** | — | In-context pretraining benchmark used to train PRODIGY |
| **TAG / ULTRA knowledge graphs** | 57 KGs | Multi-source KG mix used to pretrain ULTRA foundation model |
| **One-for-All (OFA) Collection** | 9 text-attributed graphs | Unified text-attributed graph benchmark spanning citation, molecules, KGs |
| **GLBench / GraphArena / TAGLAS** | 30+ datasets | Recent evaluation suites for graph foundation models and LLM+Graph |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2026](2026.md)
- [2025](2025.md)
- [2024](2024.md)
- [2023](2023.md)
- [2020](2020.md)
- [2019](2019.md)
- [2016](2016.md)
