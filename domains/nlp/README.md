# Natural Language Processing (NLP)

A collection of must-read NLP papers from top venues.

## Tech Tree

```mermaid
graph TD
    classDef word fill:#DBEAFE,stroke:#2563EB
    classDef seq fill:#D1FAE5,stroke:#059669
    classDef plm fill:#FED7AA,stroke:#EA580C
    classDef rag fill:#E9D5FF,stroke:#7C3AED
    classDef star fill:#FFD700,stroke:#B8860B

    Word2Vec["⭐ Word2Vec (2013)"]:::star --> GloVe["GloVe (2014)"]:::word
    LSTM["LSTM (1997)"]:::seq --> Seq2Seq["⭐ Seq2Seq (2014)"]:::star
    Seq2Seq --> Attention["Bahdanau Attention (2015)"]:::seq
    Attention --> Transformer["⭐ Transformer (2017)"]:::star

    Word2Vec -.-> ELMo["ELMo (2018)"]:::plm
    Transformer -.-> BERT["⭐ BERT (2019)"]:::star
    BERT --> RoBERTa["RoBERTa (2019)"]:::plm
    Transformer -.-> GPT2["GPT-2 (2019)"]:::plm
    GPT2 --> GPT3["GPT-3 (2020)"]:::plm
    GPT3 --> LLaMA["LLaMA (2023)"]:::plm

    BERT -.-> RAG["RAG (2020)"]:::rag
    GPT3 -.-> RAG
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Word Representations](https://img.shields.io/badge/Word_Representations-DBEAFE?style=flat-square) | Static distributed word embeddings that encode semantic relationships in dense vectors |
| ![Sequence Modeling](https://img.shields.io/badge/Sequence_Modeling-D1FAE5?style=flat-square) | Architectures for processing variable-length sequences, from RNN to attention mechanisms |
| ![Pre-trained LMs](https://img.shields.io/badge/Pre--trained_LMs-FED7AA?style=flat-square) | Large-scale models pre-trained on unlabeled text, enabling transfer learning across NLP tasks |
| ![Retrieval-Augmented](https://img.shields.io/badge/Retrieval--Augmented-E9D5FF?style=flat-square) | Methods combining parametric LMs with non-parametric retrieval for knowledge-grounded generation |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2023](2023.md)
- [2020](2020.md)
- [2019](2019.md)
- [2014](2014.md)
