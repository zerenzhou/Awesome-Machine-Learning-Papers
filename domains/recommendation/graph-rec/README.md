# Graph-based Recommendation

GNN-based recommendation on user-item interaction graphs. Evolved from heavy-weight message passing (PinSage, NGCF) to minimalist (LightGCN) to contrastive methods (SimGCL).

## Tech Tree

```mermaid
graph TD
    classDef gcn fill:#D1FAE5,stroke:#059669
    classDef contrastive fill:#FCE7F3,stroke:#DB2777
    classDef kg fill:#FED7AA,stroke:#EA580C
    classDef hypergraph fill:#E0E7FF,stroke:#4F46E5
    classDef star fill:#FFD700,stroke:#B8860B

    PinSage["⭐ PinSage (2018)"]:::star --> NGCF["NGCF (2019)"]:::gcn
    NGCF --> LightGCN["⭐ LightGCN (2020)"]:::star
    LightGCN --> UltraGCN["UltraGCN (2021)"]:::gcn
    LightGCN --> SGL["SGL (2021)"]:::contrastive
    SGL --> SimGCL["⭐ SimGCL (2022)"]:::star
    SimGCL --> XSimGCL["XSimGCL (2024)"]:::contrastive
    SimGCL --> LightGCL["LightGCL (2023)"]:::contrastive
    KGAT["KGAT (2019)"]:::kg --> KGIN["KGIN (2021)"]:::kg
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![Graph Convolution](https://img.shields.io/badge/Graph_Convolution-D1FAE5?style=flat-square) | Graph convolution based CF (NGCF, LightGCN, UltraGCN) |
| ![Graph Contrastive](https://img.shields.io/badge/Graph_Contrastive-FCE7F3?style=flat-square) | Graph contrastive learning for recommendation (SGL, SimGCL) |
| ![Knowledge-Graph](https://img.shields.io/badge/Knowledge--Graph-FED7AA?style=flat-square) | Knowledge-graph aware recommendation (KGAT, KGIN) |
| ![Hypergraph](https://img.shields.io/badge/Hypergraph-E0E7FF?style=flat-square) | Hyperedge modeling over user-item structures |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — 2018–2019 launch era works
- [2019](2019.md)
- [2020](2020.md)
- [2021](2021.md)
- [2022](2022.md)
- [2023](2023.md)
- [2024](2024.md)
