# General Methods (Cross-Signal Paradigms)

Signal-processing methodologies that are not tied to a specific signal type — algorithm unrolling, complex-valued networks, and neural operators. These paradigms are applied across communications, biomedical, imaging, and physics signals. Papers are listed in reverse chronological order; ⭐ marks pioneering works.

## 2025

- **Sensitivity-Constrained Fourier Neural Operators for Forward and Inverse Problems** — ICLR 2025 [`Neural Operator`]
  [[Paper](https://arxiv.org/abs/2505.08740)] [[Code](https://github.com/AMBehroozi/SC_Neural_Operators)]
  Introduced sensitivity-based regularization into FNO training, improving forward prediction, parameter inversion, and robustness across up to 82-dimensional parameter spaces.

## 2023

- **Model-Based Deep Learning** — Proceedings of the IEEE 2023 [`Algorithm Unrolling`]
  [[Paper](https://arxiv.org/abs/2012.08405)]
  Authoritative tutorial surveying strategies for combining domain knowledge with deep learning, covering learned optimizers, deep unfolding, and DNN-aided inference for signal processing.

## 2022

- **Deep Unfolding with Normalizing Flow Priors for Inverse Problems** — IEEE TSP 2022 [`Algorithm Unrolling`]
  [[Paper](https://arxiv.org/abs/2107.02848)]
  Embedded normalizing flow generative models as learned proximal operators within an unrolled proximal gradient algorithm for compressed sensing and image reconstruction.

## 2021

- **Algorithm Unrolling: Interpretable, Efficient Deep Learning for Signal and Image Processing** — IEEE SPM 2021 [`Algorithm Unrolling`]
  [[Paper](https://arxiv.org/abs/1912.10557)]
  Definitive survey on algorithm unrolling published in IEEE Signal Processing Magazine, systematically reviewing the connection between iterative algorithms and deep networks across imaging, vision, and communications.

- **Fourier Neural Operator for Parametric Partial Differential Equations** — ICLR 2021 [`Neural Operator`]
  [[Paper](https://arxiv.org/abs/2010.08895)] [[Code](https://github.com/neuraloperator/neuraloperator)]
  Proposed learning mappings between function spaces via Fourier-domain parameterization, achieving 1000x speedup over PDE solvers while generalizing across resolutions.

## 2018

- ⭐ **Deep Complex Networks** — ICLR 2018 [`Complex-Valued`]
  [[Paper](https://arxiv.org/abs/1705.09792)] [[Code](https://github.com/ChihebTrabelsi/deep_complex_networks)]
  Provided key building blocks for complex-valued deep networks including complex convolutions, complex batch normalization, and complex weight initialization — the reference implementation for complex-valued deep learning.

## 2017

- **AMP-Inspired Deep Networks for Sparse Linear Inverse Problems** — IEEE TSP 2017 [`Algorithm Unrolling`]
  [[Paper](https://arxiv.org/abs/1612.01183)] [[Code](https://github.com/mborgerding/onsager_deep_learning)]
  Proposed Learned AMP and Learned VAMP by unfolding approximate message passing with Onsager correction into trainable deep networks for sparse recovery.

## 2016

- **Full-Capacity Unitary Recurrent Neural Networks** — NeurIPS 2016 [`Complex-Valued`]
  [[Paper](https://arxiv.org/abs/1611.00035)] [[Code](https://github.com/stwisdom/urnn)]
  Proposed full-capacity unitary RNNs that optimize over all unitary matrices via a multiplicative gradient step on the unitary manifold, avoiding vanishing/exploding gradients.

## 2014

- **Deep Unfolding: Model-Based Inspiration of Novel Deep Architectures** — arXiv 2014 [`Algorithm Unrolling`]
  [[Paper](https://arxiv.org/abs/1409.2574)]
  Coined the term "deep unfolding" by proposing to unfold inference iterations of model-based algorithms as layers in a deep network with untied parameters, trained discriminatively.

## 2010

- ⭐ **Learning Fast Approximations of Sparse Coding** — ICML 2010 [`Algorithm Unrolling`]
  [[Paper](https://icml.cc/Conferences/2010/papers/449.pdf)]
  Proposed LISTA (Learned ISTA) by unrolling the iterative shrinkage-thresholding algorithm into a trainable neural network, founding the algorithm unrolling paradigm.

## Benchmark Datasets

| Dataset | Scale | Description |
|:---|:---|:---|
| **FNO Benchmark Suite** | Burgers / Darcy / Navier-Stokes | Canonical PDE benchmarks from the Fourier Neural Operator paper |
| **PDEBench** | 11 PDE families | Comprehensive benchmark for scientific ML / neural operators |
| **The Well** | 15 datasets, 15TB | Large-scale physics simulation corpus for training foundation PDE models |
