# Time Series Forecasting — Tech Tree

```mermaid
graph TD
    subgraph RNN-based
        DeepAR["DeepAR (2020)"]
    end

    subgraph MLP-based
        NBEATS["N-BEATS (2020)"] --> Linear["⭐ LTSF-Linear (2023)"]
    end

    subgraph CNN-based
        TCN["TCN (2018)"] --> SCINet["SCINet (2022)"]
        TCN --> TimesNet["TimesNet (2023)"]
    end

    subgraph Transformer-based
        Informer["⭐ Informer (2021)"] --> Autoformer["Autoformer (2021)"]
        Autoformer --> FEDformer["FEDformer (2022)"]
        Informer --> PatchTST["PatchTST (2023)"]
        PatchTST --> iTransformer["iTransformer (2024)"]
    end

    Linear -.->|"challenges"| Informer
    DeepAR -.-> Informer

    style Informer fill:#FFD700
    style Linear fill:#FFD700
```

## Key Evolution Paths

| Path | Description |
|------|-------------|
| **Transformer** | Informer → Autoformer → FEDformer (frequency) → PatchTST (patching) → iTransformer (inverted) |
| **MLP** | N-BEATS → LTSF-Linear (challenged Transformer dominance) |
| **CNN** | TCN → SCINet / TimesNet (2D temporal modeling) |
| **RNN** | DeepAR (probabilistic autoregressive) |
| **Key Debate** | LTSF-Linear showed simple models can beat Transformers, sparking the "Are Transformers Effective?" discussion |
