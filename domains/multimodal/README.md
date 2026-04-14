# Multimodal Learning

A collection of must-read multimodal learning papers from top venues.

## Tech Tree

```mermaid
graph TD
    subgraph Early Vision-Language
        ViLBERT["⭐ ViLBERT (2019)"]
    end

    subgraph Contrastive Learning
        ViLBERT --> CLIP["⭐ CLIP (2021)"]
        CLIP --> ALIGN["ALIGN (2021)"]
    end

    subgraph Visual Language Models
        CLIP --> Flamingo["Flamingo (2022)"]
        Flamingo --> BLIP2["BLIP-2 (2023)"]
        BLIP2 --> LLaVA["LLaVA (2023)"]
    end

    subgraph Unified Embedding
        CLIP --> ImageBind["ImageBind (2023)"]
    end

    ViLBERT -.->|"dual-encoder → contrastive"| CLIP
    Flamingo -.->|"frozen LLM + visual"| BLIP2

    style ViLBERT fill:#FFD700
    style CLIP fill:#FFD700
```

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2023](2023.md)
- [2022](2022.md)
- [2021](2021.md)
