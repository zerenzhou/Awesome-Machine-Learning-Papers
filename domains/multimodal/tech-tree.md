# Multimodal Learning — Tech Tree

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

## Key Evolution Paths

| Path | Description |
|------|-------------|
| **Vision-Language Pre-training** | ViLBERT (co-attention) → CLIP (contrastive) → ALIGN (noisy data scaling) |
| **Visual LLMs** | Flamingo (gated cross-attention) → BLIP-2 (Q-Former bridge) → LLaVA (instruction tuning) |
| **Unified Multimodal** | CLIP (2 modalities) → ImageBind (6 modalities) |
| **Key Shift** | From task-specific fine-tuning to zero-shot transfer via contrastive pre-training |
