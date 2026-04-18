# Generative Recommendation

Generative recommendation treats recommendation as sequence generation: predict item IDs (or semantic codes) auto-regressively. Enables foundation-model-style scaling.

## Tech Tree

```mermaid
graph TD
    classDef semantic_id fill:#FEF08A,stroke:#CA8A04
    classDef gen_retrieval fill:#E9D5FF,stroke:#7C3AED
    classDef foundation fill:#E0E7FF,stroke:#4F46E5
    classDef star fill:#FFD700,stroke:#B8860B

    DSI["DSI (2022)"]:::gen_retrieval --> TIGER["⭐ TIGER (2023)"]:::star
    TIGER --> LCRec["LC-Rec (2024)"]:::semantic_id
    TIGER --> IDGenRec["IDGenRec (2024)"]:::semantic_id
    TIGER --> COBRA["COBRA (2024)"]:::semantic_id
    HSTU["⭐ HSTU (2024)"]:::star --> OneRec["OneRec (2024)"]:::foundation
    HSTU --> Meta["Meta Scaling Laws (2024)"]:::foundation
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![Semantic ID](https://img.shields.io/badge/Semantic_ID-FEF08A?style=flat-square) | RQ-VAE / semantic-code based item representations |
| ![Generative Retrieval](https://img.shields.io/badge/Generative_Retrieval-E9D5FF?style=flat-square) | Generative retrieval paradigm from IR (DSI, TIGER) |
| ![Foundation](https://img.shields.io/badge/Foundation-E0E7FF?style=flat-square) | Foundation-model scaling for recommendation (HSTU, OneRec) |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — 2022–2023 paradigm launch works
- [2022](2022.md)
- [2023](2023.md)
- [2024](2024.md)
