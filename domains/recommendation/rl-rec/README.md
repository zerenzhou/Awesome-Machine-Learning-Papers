# Reinforcement Learning for Recommendation

RL for recommendation optimizes long-term user engagement/retention rather than single-step click. Off-policy correction (YouTube REINFORCE) and slate actions (SlateQ) are core challenges.

## Tech Tree

```mermaid
graph TD
    classDef bandit fill:#DBEAFE,stroke:#2563EB
    classDef policy_grad fill:#D1FAE5,stroke:#059669
    classDef value_based fill:#FED7AA,stroke:#EA580C
    classDef hierarchical fill:#E9D5FF,stroke:#7C3AED
    classDef star fill:#FFD700,stroke:#B8860B

    LinUCB["⭐ LinUCB (2010)"]:::star --> ContextBandit["Contextual Bandits (2014)"]:::bandit
    LinUCB -.-> YouTubeRE["⭐ YouTube REINFORCE (2019)"]:::star
    YouTubeRE --> SlateQ["SlateQ (2019)"]:::value_based
    YouTubeRE --> TopKOffPolicy["Top-K Off-Policy (2019)"]:::policy_grad
    SlateQ --> M3Rec["M3Rec (2022)"]:::hierarchical
    YouTubeRE --> HRL["HRL4Rec (2019)"]:::hierarchical
    M3Rec --> EGPG["EGPG (2023)"]:::policy_grad
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![Contextual Bandit](https://img.shields.io/badge/Contextual_Bandit-DBEAFE?style=flat-square) | Contextual bandit methods (LinUCB, Thompson Sampling) |
| ![Policy Gradient](https://img.shields.io/badge/Policy_Gradient-D1FAE5?style=flat-square) | Policy-gradient / REINFORCE-based methods |
| ![Value-based](https://img.shields.io/badge/Value--based-FED7AA?style=flat-square) | Q-learning / SlateQ for combinatorial action spaces |
| ![Hierarchical RL](https://img.shields.io/badge/Hierarchical_RL-E9D5FF?style=flat-square) | HRL / multi-level policy for recommendation |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — Bandit foundations
- [2019](2019.md)
- [2020](2020.md)
- [2021](2021.md)
- [2022](2022.md)
- [2023](2023.md)
- [2024](2024.md)
- [2025](2025.md)
