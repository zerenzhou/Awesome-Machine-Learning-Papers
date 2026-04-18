# Session-based Recommendation

Session-based recommendation works on short anonymous sessions (no user ID). Evolved from attention-based (NARM, STAMP) to graph-based (SR-GNN) to hypergraph and contrastive methods.

## Tech Tree

```mermaid
graph TD
    classDef rnn_attn fill:#DBEAFE,stroke:#2563EB
    classDef gnn fill:#FECDD3,stroke:#E11D48
    classDef hypergraph fill:#E0E7FF,stroke:#4F46E5
    classDef contrastive fill:#FCE7F3,stroke:#DB2777
    classDef star fill:#FFD700,stroke:#B8860B

    GRU4Rec["⭐ GRU4Rec (2016)"]:::star --> NARM["NARM (2017)"]:::rnn_attn
    NARM --> STAMP["STAMP (2018)"]:::rnn_attn
    STAMP --> SRGNN["⭐ SR-GNN (2019)"]:::star
    SRGNN --> GCEGNN["GCE-GNN (2020)"]:::gnn
    SRGNN --> FGNN["FGNN (2019)"]:::gnn
    GCEGNN --> TAGNN["TAGNN (2020)"]:::gnn
    TAGNN --> DHCN["DHCN (2021)"]:::hypergraph
    DHCN --> COTREC["COTREC (2021)"]:::contrastive
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![RNN+Attention](https://img.shields.io/badge/RNN%2BAttention-DBEAFE?style=flat-square) | RNN + attention over session items (NARM, STAMP) |
| ![Session-as-Graph](https://img.shields.io/badge/Session--as--Graph-FECDD3?style=flat-square) | Graph neural networks on session graphs (SR-GNN, FGNN) |
| ![Hypergraph](https://img.shields.io/badge/Hypergraph-E0E7FF?style=flat-square) | Hyperedge modeling for session data (DHCN) |
| ![Contrastive](https://img.shields.io/badge/Contrastive-FCE7F3?style=flat-square) | Contrastive session learning (COTREC) |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — 2016–2017 launch era works
- [2018](2018.md)
- [2019](2019.md)
- [2020](2020.md)
- [2021](2021.md)
