# LLM for Recommendation

LLMs applied to recommendation, either as zero/few-shot recommenders or fine-tuned for instruction-following over recommendation tasks. Paradigm began in 2022 with P5.

## Tech Tree

```mermaid
graph TD
    classDef unified_prompt fill:#E0E7FF,stroke:#4F46E5
    classDef instruction_tune fill:#D1FAE5,stroke:#059669
    classDef zero_shot fill:#FCE7F3,stroke:#DB2777
    classDef embedding fill:#FEF08A,stroke:#CA8A04
    classDef star fill:#FFD700,stroke:#B8860B

    P5["⭐ P5 (2022)"]:::star --> TALLRec["⭐ TALLRec (2023)"]:::star
    P5 --> LlamaRec["LlamaRec (2023)"]:::instruction_tune
    TALLRec --> BIGRec["BIGRec (2023)"]:::instruction_tune
    TALLRec --> LLaRA["LLaRA (2024)"]:::instruction_tune
    P5 --> E4SRec["E4SRec (2023)"]:::embedding
    ChatGPTRec["ChatGPT-as-Rec (2023)"]:::zero_shot -.-> TALLRec
    LLaRA --> ReLLa["ReLLa (2024)"]:::instruction_tune
```

### Paradigm Legend

| Color | Meaning |
|:---|:---|
| ![Unified Prompt](https://img.shields.io/badge/Unified_Prompt-E0E7FF?style=flat-square) | P5-style multi-task prompting for recommendation |
| ![Instruction Tuning](https://img.shields.io/badge/Instruction_Tuning-D1FAE5?style=flat-square) | LoRA / fine-tuned LLMs for recommendation tasks |
| ![Zero-shot](https://img.shields.io/badge/Zero--shot-FCE7F3?style=flat-square) | ChatGPT/GPT-4 as recommender with no fine-tuning |
| ![Embedding](https://img.shields.io/badge/Embedding-FEF08A?style=flat-square) | LLM embeddings injected into existing rec models |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works |

## Contents

- [Classic Papers](classic.md) — 2022–2023 paradigm launch works
- [2022](2022.md)
- [2023](2023.md)
- [2024](2024.md)
