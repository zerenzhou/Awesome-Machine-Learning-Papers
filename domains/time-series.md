# Time Series Forecasting (TSF)

A collection of must-read time series forecasting papers from top venues.

- ⭐ **Informer: Beyond Efficient Transformer for Long Sequence Time-Series Forecasting** — AAAI 2021 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2012.07436)] [[Code](https://github.com/zhouhaoyi/Informer2020)]
  Introduced ProbSparse self-attention and distilling operation for efficient long-sequence time-series forecasting.

- ⭐ **Are Transformers Effective for Time Series Forecasting?** — AAAI 2023 [`MLP`]
  [[Paper](https://arxiv.org/abs/2205.13504)] [[Code](https://github.com/cure-lab/LTSF-Linear)]
  Challenged the necessity of Transformers for TSF, showing simple linear models can outperform complex architectures.

- **Autoformer: Decomposition Transformers with Auto-Correlation for Long-Term Series Forecasting** — NeurIPS 2021 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2106.13008)] [[Code](https://github.com/thuml/Autoformer)]
  Replaced attention with auto-correlation and introduced deep decomposition for long-term forecasting.

- **FEDformer: Frequency Enhanced Decomposed Transformer for Long-term Series Forecasting** — ICML 2022 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2201.12740)] [[Code](https://github.com/MAZiqing/FEDformer)]
  Applied frequency-domain attention with seasonal-trend decomposition for long-term time series forecasting.

- **PatchTST: A Time Series is Worth 64 Words: Long-term Forecasting with Transformers** — ICLR 2023 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2211.14730)] [[Code](https://github.com/yuqinie98/PatchTST)]
  Applied patching and channel-independent design to Transformers for multivariate long-term forecasting.

- **iTransformer: Inverted Transformers Are Effective for Time Series Forecasting** — ICLR 2024 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2310.06625)] [[Code](https://github.com/thuml/iTransformer)]
  Inverted the Transformer to apply attention on the variate dimension instead of the temporal dimension.

- **TimesNet: Temporal 2D-Variation Modeling for General Time Series Analysis** — ICLR 2023 [`CNN`]
  [[Paper](https://arxiv.org/abs/2210.02186)] [[Code](https://github.com/thuml/TimesNet)]
  Transformed 1D time series into 2D tensors to capture intra- and inter-period variations via 2D convolution.

- **N-BEATS: Neural Basis Expansion Analysis for Interpretable Time Series Forecasting** — ICLR 2020 [`MLP`]
  [[Paper](https://arxiv.org/abs/1905.10437)] [[Code](https://github.com/ElementAI/N-BEATS)]
  Proposed a deep stack of fully-connected blocks with basis expansion for interpretable time series forecasting.

- **DeepAR: Probabilistic Forecasting with Autoregressive Recurrent Networks** — International Journal of Forecasting 2020 [`RNN`]
  [[Paper](https://arxiv.org/abs/1704.04110)]
  Combined autoregressive RNNs with probabilistic output for scalable multi-step time series forecasting.

- **SCINet: Time Series Modeling and Forecasting with Sample Convolution and Interaction** — NeurIPS 2022 [`CNN`]
  [[Paper](https://arxiv.org/abs/2106.09305)] [[Code](https://github.com/cure-lab/SCINet)]
  Introduced a recursive downsampling-convolution-interaction architecture for temporal modeling.
