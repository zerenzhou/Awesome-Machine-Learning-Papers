# Natural Language Processing — Tech Tree

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

## Key Evolution Paths

| Path | Description |
|------|-------------|
| **Representations** | Word2Vec → GloVe → ELMo → BERT (contextualized) |
| **Seq2Seq** | LSTM → Seq2Seq → Attention → Transformer |
| **Autoregressive LM** | GPT-2 → GPT-3 → LLaMA (open-source) |
| **Bidirectional LM** | BERT → RoBERTa (optimized pre-training) |
| **Knowledge-Augmented** | LLM + Retrieval → RAG |
