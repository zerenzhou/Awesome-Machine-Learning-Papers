# Speech & Audio

A collection of must-read speech and audio processing papers from top venues.

## Tech Tree

```mermaid
graph TD
    classDef asr fill:#DBEAFE,stroke:#2563EB
    classDef tts fill:#D1FAE5,stroke:#059669
    classDef codec fill:#FED7AA,stroke:#EA580C
    classDef llm fill:#E9D5FF,stroke:#7C3AED
    classDef music fill:#FECDD3,stroke:#E11D48
    classDef star fill:#FFD700,stroke:#B8860B

    DeepSpeech["⭐ Deep Speech 2 (2016)"]:::star --> wav2vec["⭐ wav2vec 2.0 (2020)"]:::star
    wav2vec --> HuBERT["HuBERT (2021)"]:::asr
    wav2vec --> Whisper["Whisper (2023)"]:::asr
    wav2vec -.-> Conformer["Conformer (2020)"]:::asr

    WaveNet["⭐ WaveNet (2016)"]:::star --> DiffWave["DiffWave (2021)"]:::tts
    WaveNet --> Voicebox["Voicebox (2023)"]:::tts
    DiffWave -.-> NatSpeech2["NaturalSpeech 2 (2023)"]:::tts
    Voicebox --> CosyVoice["CosyVoice (2024)"]:::tts
    Voicebox --> F5TTS["F5-TTS (2024)"]:::tts

    VALLE["VALL-E (2023)"]:::codec --> SpeechTokenizer["SpeechTokenizer (2024)"]:::codec
    VALLE --> WavTokenizer["WavTokenizer (2024)"]:::codec

    Whisper -.-> SALMONN["SALMONN (2024)"]:::llm
    Whisper -.-> QwenAudio["Qwen-Audio (2024)"]:::llm
    wav2vec -.-> AudioPaLM["AudioPaLM (2023)"]:::llm

    WaveNet -.-> MusicLM["MusicLM (2023)"]:::music
    MusicLM --> MusicGen["MusicGen (2023)"]:::music
```

### Paradigm Guide

| Paradigm | Description |
|:---|:---|
| ![Speech Recognition](https://img.shields.io/badge/Speech_Recognition-DBEAFE?style=flat-square) | End-to-end models mapping raw audio to text, from self-supervised pre-training (wav2vec) to robust large-scale ASR (Whisper) |
| ![Speech Synthesis](https://img.shields.io/badge/Speech_Synthesis-D1FAE5?style=flat-square) | Neural TTS and audio generation, from autoregressive vocoders (WaveNet) to non-autoregressive flow-matching systems (F5-TTS) |
| ![Neural Codec](https://img.shields.io/badge/Neural_Codec-FED7AA?style=flat-square) | Audio tokenization converting speech into discrete tokens, enabling language-model-based speech generation (VALL-E) |
| ![Audio Language Models](https://img.shields.io/badge/Audio_Language_Models-E9D5FF?style=flat-square) | Large language models extended with audio understanding for universal speech and sound reasoning |
| ![Music Generation](https://img.shields.io/badge/Music_Generation-FECDD3?style=flat-square) | Models synthesizing music from text descriptions or audio prompts via generative modeling |
| ![Classic](https://img.shields.io/badge/⭐_Classic-FFD700?style=flat-square) | Pioneering works with high impact and citation, foundational to the field |

## Contents

- [Classic Papers](classic.md) — Foundational and pioneering works
- [2024](2024.md)
- [2023](2023.md)
- [2021](2021.md)
- [2020](2020.md)
