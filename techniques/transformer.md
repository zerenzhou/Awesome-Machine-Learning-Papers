# Transformer & Attention

A collection of must-read papers on Transformer architectures and attention mechanisms from top venues.

- ⭐ **Attention Is All You Need** — NeurIPS 2017 [`NLP`]
  [[Paper](https://arxiv.org/abs/1706.03762)] [[Code](https://github.com/tensorflow/tensor2tensor)]
  Proposed the Transformer architecture, replacing recurrence entirely with multi-head self-attention for sequence transduction.

- ⭐ **BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding** — NAACL 2019 [`NLP`]
  [[Paper](https://arxiv.org/abs/1810.04805)] [[Code](https://github.com/google-research/bert)]
  Introduced bidirectional pre-training of Transformers via masked language modeling and next sentence prediction.

- ⭐ **An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale** — ICLR 2021 [`CV`]
  [[Paper](https://arxiv.org/abs/2010.11929)] [[Code](https://github.com/google-research/vision_transformer)]
  Proposed Vision Transformer (ViT), applying a pure Transformer directly to sequences of image patches for classification.

- ⭐ **GPT-2: Language Models are Unsupervised Multitask Learners** — OpenAI 2019 [`NLP`]
  [[Paper](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)] [[Code](https://github.com/openai/gpt-2)]
  Demonstrated that large-scale autoregressive language models can perform diverse NLP tasks zero-shot without explicit supervision.

- **Swin Transformer: Hierarchical Vision Transformer using Shifted Windows** — ICCV 2021 [`CV`]
  [[Paper](https://arxiv.org/abs/2103.14030)] [[Code](https://github.com/microsoft/Swin-Transformer)]
  Introduced shifted window-based self-attention for efficient hierarchical feature extraction in vision tasks.

- **Longformer: The Long-Document Transformer** — arXiv 2020 [`NLP`]
  [[Paper](https://arxiv.org/abs/2004.05150)] [[Code](https://github.com/allenai/longformer)]
  Proposed a combination of local windowed and global attention to scale Transformers to long documents with linear complexity.

- **Informer: Beyond Efficient Transformer for Long Sequence Time-Series Forecasting** — AAAI 2021 [`TSF`]
  [[Paper](https://arxiv.org/abs/2012.07436)] [[Code](https://github.com/zhouhaoyi/Informer2020)]
  Introduced ProbSparse self-attention and distilling operation to efficiently handle long-sequence time-series forecasting.

- **Autoformer: Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting** — NeurIPS 2021 [`TSF`]
  [[Paper](https://arxiv.org/abs/2106.13008)] [[Code](https://github.com/thuml/Autoformer)]
  Replaced standard attention with an auto-correlation mechanism and series decomposition for long-term time series forecasting.

- **PatchTST: A Time Series is Worth 64 Words: Long-term Forecasting with Transformers** — ICLR 2023 [`TSF`]
  [[Paper](https://arxiv.org/abs/2211.14730)] [[Code](https://github.com/yuqinie98/PatchTST)]
  Applied patching and channel-independent design to Transformers for multivariate long-term time series forecasting.

- **iTransformer: Inverted Transformers Are Effective for Time Series Forecasting** — ICLR 2024 [`TSF`]
  [[Paper](https://arxiv.org/abs/2310.06625)] [[Code](https://github.com/thuml/iTransformer)]
  Inverted the Transformer architecture to apply attention on the variate dimension instead of the temporal dimension.
