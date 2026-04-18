# Debiasing / Fairness / Causal Recommendation

Recommendation data is subject to popularity bias, exposure bias, selection bias, and conformity bias. This paradigm applies causal inference tools (IPS, DR, counterfactuals) to debias.

## Tech Tree

```mermaid
graph TD
    classDef propensity fill:#DBEAFE,stroke:#2563EB
    classDef doubly_robust fill:#D1FAE5,stroke:#059669
    classDef causal fill:#FED7AA,stroke:#EA580C
    classDef fairness fill:#E9D5FF,stroke:#7C3AED
    classDef star fill:#FFD700,stroke:#B8860B

    IPS["⭐ IPS for Rec (2016)"]:::star --> DR["⭐ DR (2019)"]:::star
    DR --> AutoDebias["AutoDebias (2021)"]:::doubly_robust
    IPS --> PDA["PDA (2021)"]:::causal
    PDA --> MACR["MACR (2021)"]:::causal
    PDA --> DICE["DICE (2021)"]:::causal
    MACR --> CR["CR (2022)"]:::causal
    CausalEmb["Causal Embeddings (2018)"]:::causal --> PDA
    FairRec["FairRec (2020)"]:::fairness -.-> MACR
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![Propensity](https://img.shields.io/badge/Propensity-DBEAFE?style=flat-square) | IPS / propensity-weighted debiasing |
| ![Doubly Robust](https://img.shields.io/badge/Doubly_Robust-D1FAE5?style=flat-square) | DR family combining IPS and direct estimation |
| ![Causal](https://img.shields.io/badge/Causal-FED7AA?style=flat-square) | Counterfactual / causal embeddings approaches |
| ![Fairness](https://img.shields.io/badge/Fairness-E9D5FF?style=flat-square) | Fair recommendation for providers and users |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — 2015–2018 foundational works
- [2019](2019.md)
- [2020](2020.md)
- [2021](2021.md)
- [2022](2022.md)
