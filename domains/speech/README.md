# Speech & Audio

A collection of must-read speech and audio processing papers from top venues.

## Tech Tree

```mermaid
graph TD
    subgraph End-to-End Recognition
        DeepSpeech["⭐ Deep Speech 2 (2016)"]
        DeepSpeech --> wav2vec["⭐ wav2vec 2.0 (2020)"]
        wav2vec --> HuBERT["HuBERT (2021)"]
        wav2vec --> Whisper["Whisper (2023)"]
    end

    subgraph Hybrid Architecture
        Conformer["Conformer (2020)"]
        wav2vec -.-> Conformer
    end

    subgraph Audio Generation
        WaveNet["⭐ WaveNet (2016)"]
        WaveNet -.-> DiffWave["DiffWave (2021)"]
    end

    DeepSpeech -.->|"RNN → Transformer"| wav2vec

    style DeepSpeech fill:#FFD700
    style WaveNet fill:#FFD700
    style wav2vec fill:#FFD700
```

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2023](2023.md)
- [2021](2021.md)
- [2020](2020.md)
