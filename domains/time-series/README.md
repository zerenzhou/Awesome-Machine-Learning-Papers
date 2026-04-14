# Time Series Forecasting (TSF)

A collection of must-read time series forecasting papers from top venues.

## Tech Tree

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

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2024](2024.md)
- [2023](2023.md)
- [2022](2022.md)
- [2021](2021.md)
- [2020](2020.md)
