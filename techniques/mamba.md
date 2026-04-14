# Mamba & State Space Models

A collection of must-read papers on state space models and selective state space architectures from top venues.

- ⭐ **Efficiently Modeling Long Sequences with Structured State Spaces** — ICLR 2022 [`General`]
  [[Paper](https://arxiv.org/abs/2111.00396)] [[Code](https://github.com/state-spaces/s4)]
  Introduced S4, combining continuous-time state spaces with HiPPO initialization for efficient long-range sequence modeling.

- ⭐ **Mamba: Linear-Time Sequence Modeling with Selective State Spaces** — ICML 2024 [`General`]
  [[Paper](https://arxiv.org/abs/2312.00752)] [[Code](https://github.com/state-spaces/mamba)]
  Proposed selective state space models with input-dependent parameterization, achieving Transformer-quality with linear-time complexity.

- **Hungry Hungry Hippos: Towards Language Modeling with State Space Models** — ICLR 2023 [`NLP`]
  [[Paper](https://arxiv.org/abs/2212.14052)] [[Code](https://github.com/HazyResearch/H3)]
  Introduced H3, combining SSM layers with attention-like gating to close the gap with Transformers on language modeling.

- **Vision Mamba: Efficient Visual Representation Learning with Bidirectional State Space Model** — ICML 2024 [`CV`]
  [[Paper](https://arxiv.org/abs/2401.09417)] [[Code](https://github.com/hustvl/Vim)]
  Applied bidirectional Mamba to vision tasks, achieving competitive performance with linear complexity in image tokens.

- **TimeMachine: A Time Series is Worth 4 Mambas for Long-term Forecasting** — arXiv 2024 [`TSF`]
  [[Paper](https://arxiv.org/abs/2403.09898)] [[Code](https://github.com/Atik-Ahamed/TimeMachine)]
  Integrated Mamba blocks with multi-scale patching for efficient long-term time series forecasting.

- **MambaOut: Do We Really Need Mamba for Vision?** — arXiv 2024 [`CV`]
  [[Paper](https://arxiv.org/abs/2405.07992)] [[Code](https://github.com/yuweihao/MambaOut)]
  Investigated when SSM mechanisms are necessary for vision tasks, showing gated CNNs can match Mamba on image classification.
