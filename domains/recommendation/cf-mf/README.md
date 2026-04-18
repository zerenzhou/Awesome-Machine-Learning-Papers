# Collaborative Filtering & Matrix Factorization

The foundational paradigm of recommendation systems. Models user-item interactions via latent-factor decomposition or neighborhood methods.

## Tech Tree

```mermaid
graph TD
    classDef neighbor fill:#DBEAFE,stroke:#2563EB
    classDef latent fill:#D1FAE5,stroke:#059669
    classDef ranking fill:#FED7AA,stroke:#EA580C
    classDef fm fill:#E9D5FF,stroke:#7C3AED
    classDef star fill:#FFD700,stroke:#B8860B

    ItemCF["⭐ Item-based CF (2001)"]:::star --> SlopeOne["Slope One (2005)"]:::neighbor
    NetflixMF["⭐ Matrix Factorization (2009)"]:::star --> SVDpp["SVD++ (2008)"]:::latent
    NetflixMF --> BPR["⭐ BPR (2009)"]:::star
    BPR --> WRMF["WRMF / eALS (2014)"]:::ranking
    SVDpp --> FM["⭐ FM (2010)"]:::star
    FM --> FFM["FFM (2016)"]:::fm
    FM --> AFM["AFM (2017)"]:::fm
    FM --> NFM["NFM (2017)"]:::fm
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![Neighborhood](https://img.shields.io/badge/Neighborhood-DBEAFE?style=flat-square) | Item/user-based CF with similarity heuristics |
| ![Latent Factor](https://img.shields.io/badge/Latent_Factor-D1FAE5?style=flat-square) | SVD, SVD++, biased MF — low-rank decomposition of rating matrix |
| ![Ranking-aware](https://img.shields.io/badge/Ranking-FED7AA?style=flat-square) | BPR, WRMF, eALS — optimize ranking losses for implicit feedback |
| ![Factorization Machines](https://img.shields.io/badge/FM-E9D5FF?style=flat-square) | FM family — generalizes MF to arbitrary feature interactions |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — 1994–2015 foundational works
- [2017](2017.md)
- [2018](2018.md)
- [2019](2019.md)
- [misc](misc.md) — sparse years combined
