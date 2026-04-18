# Deep Recommenders

Deep feature-interaction models. Build on FM by replacing shallow second-order interactions with deep networks for CTR and ranking.

## Tech Tree

```mermaid
graph TD
    classDef wide_deep fill:#DBEAFE,stroke:#2563EB
    classDef fm_based fill:#D1FAE5,stroke:#059669
    classDef crossnet fill:#FED7AA,stroke:#EA580C
    classDef attention fill:#E9D5FF,stroke:#7C3AED
    classDef star fill:#FFD700,stroke:#B8860B

    WideDeep["⭐ Wide & Deep (2016)"]:::star --> DeepFM["⭐ DeepFM (2017)"]:::star
    WideDeep --> DCN["DCN (2017)"]:::crossnet
    DeepFM --> xDeepFM["xDeepFM (2018)"]:::fm_based
    DeepFM --> NFM["NFM (2017)"]:::fm_based
    DeepFM --> AFM["AFM (2017)"]:::attention
    DCN --> DCNv2["⭐ DCN-V2 (2021)"]:::star
    xDeepFM --> AutoInt["AutoInt (2019)"]:::attention
    AutoInt --> FiBiNET["FiBiNET (2019)"]:::attention
    NCF["⭐ NCF (2017)"]:::star --> DeepFM
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![Wide & Deep style](https://img.shields.io/badge/Wide_%26_Deep_style-DBEAFE?style=flat-square) | Memorization + generalization hybrids |
| ![FM-based](https://img.shields.io/badge/FM--based-D1FAE5?style=flat-square) | Deep FM extensions (DeepFM, NFM, xDeepFM) |
| ![Cross-network](https://img.shields.io/badge/Cross--network-FED7AA?style=flat-square) | Explicit feature crossing (DCN, DCN-V2) |
| ![Attention-based](https://img.shields.io/badge/Attention--based-E9D5FF?style=flat-square) | Attention over feature interactions (AFM, AutoInt, FiBiNET) |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — 2016–2017 foundational works
- [2018](2018.md)
- [2019](2019.md)
- [2021](2021.md)
