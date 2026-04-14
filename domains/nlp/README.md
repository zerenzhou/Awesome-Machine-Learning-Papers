# Natural Language Processing (NLP)

A collection of must-read NLP papers from top venues.

## Tech Tree

```mermaid
graph TD
    subgraph Word Representations
        Word2Vec["⭐ Word2Vec (2013)"] --> GloVe["GloVe (2014)"]
    end

    subgraph Sequence Modeling
        LSTM["LSTM (1997)"] --> Seq2Seq["⭐ Seq2Seq (2014)"]
        Seq2Seq --> Attention["Bahdanau Attention (2015)"]
        Attention --> Transformer["⭐ Transformer (2017)"]
    end

    subgraph Pre-trained Language Models
        Word2Vec -.-> ELMo["ELMo (2018)"]
        Transformer --> BERT["⭐ BERT (2019)"]
        BERT --> RoBERTa["RoBERTa (2019)"]
        Transformer --> GPT2["GPT-2 (2019)"]
        GPT2 --> GPT3["GPT-3 (2020)"]
        GPT3 --> LLaMA["LLaMA (2023)"]
    end

    subgraph Retrieval-Augmented
        BERT -.-> RAG["RAG (2020)"]
        GPT3 -.-> RAG
    end

    style Word2Vec fill:#FFD700
    style Seq2Seq fill:#FFD700
    style Transformer fill:#FFD700
    style BERT fill:#FFD700
```

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2023](2023.md)
- [2020](2020.md)
- [2019](2019.md)
- [2014](2014.md)
