# Recommendation Systems

A collection of must-read recommendation system papers from top venues (SIGIR, RecSys, KDD, WWW, NeurIPS, ICML, ICLR, CIKM, AAAI, IJCAI, ACL, TOIS). Organized into 10 paradigm subdirectories covering collaborative filtering, deep learning, CTR prediction, sequential methods, session-based recommendation, graph neural networks, LLM-based approaches, generative models, debiasing/fairness, and reinforcement learning.

## Tech Tree

```mermaid
graph TD
    classDef cf fill:#DBEAFE,stroke:#2563EB
    classDef deep fill:#D1FAE5,stroke:#059669
    classDef ctr fill:#FED7AA,stroke:#EA580C
    classDef seq fill:#E9D5FF,stroke:#7C3AED
    classDef session fill:#FCE7F3,stroke:#DB2777
    classDef gnn fill:#FECDD3,stroke:#E11D48
    classDef llm fill:#E0E7FF,stroke:#4F46E5
    classDef gen fill:#FEF08A,stroke:#CA8A04
    classDef debias fill:#CCFBF1,stroke:#0D9488
    classDef rl fill:#E5E7EB,stroke:#4B5563
    classDef star fill:#FFD700,stroke:#B8860B

    MF["⭐ MF (2009)"]:::star --> BPR["BPR (2009)"]:::cf
    MF --> SVDpp["SVD++ (2008)"]:::cf
    BPR --> FM["⭐ FM (2010)"]:::star
    FM --> DeepFM["⭐ DeepFM (2017)"]:::star
    FM --> xDeepFM["xDeepFM (2018)"]:::deep
    DeepFM --> DCN["DCN (2017)"]:::deep
    DCN --> DCNv2["DCN-V2 (2021)"]:::deep

    BPR --> NCF["NCF (2017)"]:::deep
    NCF --> LightGCN["⭐ LightGCN (2020)"]:::star
    NCF --> NGCF["NGCF (2019)"]:::gnn
    NGCF --> LightGCN
    LightGCN --> SimGCL["SimGCL (2022)"]:::gnn
    LightGCN --> XSimGCL["XSimGCL (2024)"]:::gnn

    DeepFM --> DIN["⭐ DIN (2018)"]:::star
    DIN --> DIEN["DIEN (2019)"]:::ctr
    DIEN --> SIM["SIM (2020)"]:::ctr
    DIN --> CAN["CAN (2022)"]:::ctr

    GRU4Rec["⭐ GRU4Rec (2016)"]:::star --> SASRec["⭐ SASRec (2018)"]:::star
    SASRec --> BERT4Rec["BERT4Rec (2019)"]:::seq
    SASRec --> CL4SRec["CL4SRec (2022)"]:::seq
    BERT4Rec --> DuoRec["DuoRec (2022)"]:::seq

    GRU4Rec --> NARM["NARM (2017)"]:::session
    NARM --> SRGNN["SR-GNN (2019)"]:::session
    SRGNN --> GCEGNN["GCE-GNN (2020)"]:::session

    SASRec -.-> P5["⭐ P5 (2022)"]:::star
    P5 --> TALLRec["TALLRec (2023)"]:::llm
    P5 --> LlamaRec["LlamaRec (2023)"]:::llm
    TALLRec --> BIGRec["BIGRec (2023)"]:::llm

    P5 --> TIGER["⭐ TIGER (2023)"]:::star
    TIGER --> HSTU["HSTU (2024)"]:::gen
    TIGER --> LCRec["LC-Rec (2024)"]:::gen

    BPR -.-> IPS["IPS (2016)"]:::debias
    IPS --> DR["DR (2019)"]:::debias
    DR --> PDA["PDA (2021)"]:::debias

    NCF -.-> ReinRec["YouTube REINFORCE (2019)"]:::rl
    ReinRec --> SlateQ["SlateQ (2019)"]:::rl
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![CF & MF](https://img.shields.io/badge/CF_%26_MF-DBEAFE?style=flat-square) | Collaborative filtering and matrix factorization — the foundational paradigm |
| ![Deep Rec](https://img.shields.io/badge/Deep_Rec-D1FAE5?style=flat-square) | Deep neural architectures for feature interaction learning |
| ![CTR & Ranking](https://img.shields.io/badge/CTR_%26_Ranking-FED7AA?style=flat-square) | Click-through rate prediction and industrial ranking systems |
| ![Sequential](https://img.shields.io/badge/Sequential-E9D5FF?style=flat-square) | Modeling long-term user behavior sequences |
| ![Session](https://img.shields.io/badge/Session-FCE7F3?style=flat-square) | Short anonymous session-based recommendation |
| ![Graph](https://img.shields.io/badge/Graph-FECDD3?style=flat-square) | GNN-based recommendation via user-item interaction graphs |
| ![LLM4Rec](https://img.shields.io/badge/LLM4Rec-E0E7FF?style=flat-square) | Large language models applied to recommendation |
| ![Generative](https://img.shields.io/badge/Generative-FEF08A?style=flat-square) | Generative retrieval, semantic IDs, and generative recommenders |
| ![Debias & Causal](https://img.shields.io/badge/Debias_%26_Causal-CCFBF1?style=flat-square) | Bias correction, fairness, and causal inference for recommendation |
| ![RL](https://img.shields.io/badge/RL-E5E7EB?style=flat-square) | Reinforcement learning for long-term user value optimization |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact, foundational to the field |

## Benchmark Datasets

### General / Academic

| Dataset | Users / Items / Interactions | Description |
|:---|:---|:---|
| **MovieLens (100K / 1M / 10M / 20M / 25M)** | varying | De facto academic benchmark for CF, sequential, and graph methods |
| **Amazon Reviews (Beauty / Sports / Toys / Books / Clothing)** | varying | Large-scale review datasets; standard for sequential and LLM4Rec |
| **Yelp** | ~1.9M / 150K / 8M+ | User reviews of businesses; popular for graph-based methods |
| **Gowalla** | 30K / 41K / 1M | Location check-in graph; LightGCN-era benchmark |
| **Last.FM** | 2K / 18K / 93K | Music listening; HetRec and social rec benchmark |
| **Book-Crossing** | 280K / 271K / 1.1M | Book rating network |

### CTR / Industrial Advertising

| Dataset | Scale | Description |
|:---|:---|:---|
| **Criteo** | 45M ads | Standard CTR benchmark for feature-interaction models |
| **Avazu** | 40M impressions | Mobile ad click prediction |
| **iPinYou** | 19.5M bids | RTB click + conversion |
| **KuaiRand / KuaiSAR** | — | Kuaishou short-video click and search+recommend dataset with unbiased evaluation |

### Industrial / Large-Scale

| Dataset | Description |
|:---|:---|
| **Taobao User Behavior** | 100M interactions for CTR / sequential rec |
| **Alibaba Ads** | Production ad dataset released with DIN/DIEN papers |
| **Tenrec** | 5M users / 140M interactions; Tencent benchmark for 10+ tasks |

### Sequential / Session

| Dataset | Description |
|:---|:---|
| **Diginetica** | E-commerce session clicks; RecSys 2016 Challenge |
| **YooChoose** | E-commerce session clicks; RecSys 2015 Challenge |
| **RetailRocket** | E-commerce session/transaction |

### News & Text-Attributed

| Dataset | Description |
|:---|:---|
| **MIND (small / large)** | Microsoft news recommendation with article text |
| **Adressa** | Norwegian news click stream |

## Evaluation Metrics

| Metric | Used For | Definition |
|:---|:---|:---|
| **HR@K** | Top-K | Hit rate at K |
| **NDCG@K** | Top-K | Normalized discounted cumulative gain at K |
| **Recall@K** | Top-K | Recall among top K |
| **MRR** | Top-K | Mean reciprocal rank |
| **AUC / GAUC** | CTR | Area under ROC / group-weighted AUC |
| **Coverage / Diversity / Novelty / Serendipity** | Top-K | Beyond-accuracy metrics |

## Contents

- [Collaborative Filtering & Matrix Factorization](cf-mf/)
- [Deep Recommenders](deep-rec/)
- [CTR Prediction & Ranking](ctr-ranking/)
- [Sequential Recommendation](sequential-rec/)
- [Session-based Recommendation](session-rec/)
- [Graph-based Recommendation](graph-rec/)
- [LLM for Recommendation](llm4rec/)
- [Generative Recommendation](generative-rec/)
- [Debiasing / Fairness / Causal](debias-causal/)
- [Reinforcement Learning for Recommendation](rl-rec/)
