# Graph Learning

A collection of must-read graph learning papers from top venues.

## Tech Tree

```mermaid
graph TD
    subgraph Spectral Methods
        GCN["⭐ GCN (2017)"]
    end

    subgraph Spatial Methods
        GraphSAGE["⭐ GraphSAGE (2017)"]
        GraphSAGE --> GAT["⭐ GAT (2018)"]
        GAT --> GIN["GIN (2019)"]
    end

    subgraph Generative
        GCN --> VGAE["VGAE (2016)"]
    end

    subgraph Expressiveness & Theory
        GCN --> GIN
        GIN -.->|"WL-test analysis"| MPNN["MPNN Framework (2017)"]
    end

    subgraph Graph Transformer
        GAT -.-> GTN["Graph Transformer Networks (2019)"]
    end

    subgraph Pre-training
        GCN --> PretrainGNN["Pre-training GNNs (2020)"]
        GraphSAGE --> PretrainGNN
    end

    style GCN fill:#FFD700
    style GraphSAGE fill:#FFD700
    style GAT fill:#FFD700
```

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2020](2020.md)
- [2019](2019.md)
- [2016](2016.md)
