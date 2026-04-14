# Graph Learning — Tech Tree

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

## Key Evolution Paths

| Path | Description |
|------|-------------|
| **Spectral → Spatial** | GCN (spectral convolution) → GraphSAGE (sampling) → GAT (attention) |
| **Expressiveness** | GCN/GraphSAGE → GIN (maximally powerful under WL-test) |
| **Unified Framework** | Various GNNs → MPNN (message passing unification) |
| **Generative** | GCN + VAE → VGAE (link prediction) |
| **Scalability** | GCN → GraphSAGE (inductive, sampling-based) → Pre-training GNNs |
