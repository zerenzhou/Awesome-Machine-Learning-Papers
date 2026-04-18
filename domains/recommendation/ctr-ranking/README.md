# CTR Prediction & Ranking

CTR prediction and industrial ranking systems, emphasizing user-interest modeling, multi-task learning, and long-sequence modeling for production-scale recommender systems.

## Tech Tree

```mermaid
graph TD
    classDef interest fill:#E9D5FF,stroke:#7C3AED
    classDef multitask fill:#CCFBF1,stroke:#0D9488
    classDef long_seq fill:#FED7AA,stroke:#EA580C
    classDef industrial fill:#F3F4F6,stroke:#6B7280
    classDef star fill:#FFD700,stroke:#B8860B

    DIN["⭐ DIN (2018)"]:::star --> DIEN["DIEN (2019)"]:::interest
    DIEN --> DSIN["DSIN (2019)"]:::interest
    DIEN --> MIMN["MIMN (2019)"]:::long_seq
    MIMN --> SIM["SIM (2020)"]:::long_seq
    SIM --> ETA["ETA (2021)"]:::long_seq
    DIN --> CAN["CAN (2022)"]:::interest
    MMoE["⭐ MMoE (2018)"]:::star --> PLE["PLE (2020)"]:::multitask
    MMoE --> ESMM["ESMM (2018)"]:::multitask
    PLE --> STAR["STAR (2021)"]:::multitask
    DLRM["⭐ DLRM (2019)"]:::star --> ZeroShot["Meta Inference Scaling"]:::industrial
    YouTubeDNN["⭐ YouTube DNN (2016)"]:::star --> DIN
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![Interest Modeling](https://img.shields.io/badge/Interest_Modeling-E9D5FF?style=flat-square) | User interest modeling (DIN, DIEN, DSIN) |
| ![Multi-task](https://img.shields.io/badge/Multi--task-CCFBF1?style=flat-square) | Multi-task / gate architectures (MMoE, PLE, ESMM) |
| ![Long Sequence](https://img.shields.io/badge/Long_Sequence-FED7AA?style=flat-square) | Long sequence behavior modeling (MIMN, SIM, ETA) |
| ![Industrial](https://img.shields.io/badge/Industrial-F3F4F6?style=flat-square) | Production-scale systems (YouTube DNN, DLRM) |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — 2016–2018 foundational works
- [2019](2019.md)
- [2020](2020.md)
- [2021](2021.md)
- [2022](2022.md)
- [2023](2023.md)
- [2024](2024.md)
- [2025](2025.md)
