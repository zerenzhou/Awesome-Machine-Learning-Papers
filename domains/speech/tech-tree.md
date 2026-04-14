# Speech & Audio — Tech Tree

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

## Key Evolution Paths

| Path | Description |
|------|-------------|
| **Recognition** | Deep Speech 2 (RNN+CTC) → wav2vec 2.0 (self-supervised) → Whisper (large-scale weak supervision) |
| **Self-Supervised** | wav2vec 2.0 → HuBERT (masked prediction on clusters) |
| **Hybrid** | Transformer + CNN → Conformer (best of both) |
| **Generation** | WaveNet (autoregressive CNN) → DiffWave (diffusion-based) |
| **Key Shift** | From supervised RNN to self-supervised Transformer representations |
