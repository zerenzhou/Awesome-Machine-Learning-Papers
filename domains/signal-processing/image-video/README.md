# Image & Video Signal Processing

Deep learning for image/video reconstruction and inverse problems — compressive sensing image recovery, MRI/CT reconstruction, and diffusion-based solvers for general noisy inverse problems. This subdomain overlaps substantially with computer vision but is included because its methodology (sampling operators, forward models, iterative solvers) is fundamentally signal-processing. Papers are listed in reverse chronological order; ⭐ marks pioneering works.

## 2025

- **Diffusion State-Guided Projected Gradient for Inverse Problems** — ICLR 2025 [`Diffusion`]
  [[Paper](https://arxiv.org/abs/2410.03463)] [[Code](https://github.com/Anima-Lab/DiffStateGrad)]
  Projects measurement guidance gradients onto a low-rank subspace from intermediate diffusion states, acting as a plug-in for existing diffusion-based inverse solvers with improved robustness.

- **Invertible Diffusion Models for Compressed Sensing** — IEEE TPAMI 2025 [`Diffusion`]
  [[Paper](https://arxiv.org/abs/2403.17006)]
  Repurposed the diffusion sampling process as an end-to-end CS reconstruction model via a two-level invertible design, reducing GPU memory by up to 93.8% during training.

## 2024

- **Solving Inverse Problems with Latent Diffusion Models via Hard Data Consistency** — ICLR 2024 Spotlight [`Diffusion`]
  [[Paper](https://arxiv.org/abs/2307.08123)] [[Code](https://github.com/soominkwon/resample)]
  Proposed ReSample, solving general inverse problems using pre-trained latent diffusion models by incorporating hard data consistency with a resampling scheme to maintain the noisy data manifold.

## 2023

- **Diffusion Posterior Sampling for General Noisy Inverse Problems** — ICLR 2023 Spotlight [`Diffusion`]
  [[Paper](https://arxiv.org/abs/2209.14687)] [[Code](https://github.com/DPS2022/diffusion-posterior-sampling)]
  Extended diffusion-based solvers to handle general noisy and nonlinear inverse problems by approximating the posterior score via a tractable likelihood term — a field standard.

- **Ambient Diffusion: Learning Clean Distributions from Corrupted Data** — NeurIPS 2023 [`Diffusion`]
  [[Paper](https://arxiv.org/abs/2305.19256)] [[Code](https://github.com/giannisdaras/ambient-diffusion)]
  First diffusion framework that learns clean data distributions from only corrupted/incomplete observations, enabling compressed sensing recovery without clean training data.

## 2022

- **Solving Inverse Problems in Medical Imaging with Score-Based Generative Models** — ICLR 2022
  [[Paper](https://arxiv.org/abs/2111.08005)] [[Code](https://github.com/yang-song/score_inverse_problems)]
  Used score-based generative models as learned priors to solve CT and MRI inverse problems without task-specific training, matching or exceeding supervised baselines.

## 2019

- **Deep Compressed Sensing** — ICML 2019
  [[Paper](https://arxiv.org/abs/1905.06723)]
  Proposed a framework jointly training generators and reconstruction via meta-learning, simultaneously optimizing measurement and recovery for compressed sensing.

## 2018

- **ISTA-Net: Interpretable Optimization-Inspired Deep Network for Image Compressive Sensing** — CVPR 2018 [`Algorithm Unrolling`]
  [[Paper](https://openaccess.thecvf.com/content_cvpr_2018/html/Zhang_ISTA-Net_Interpretable_Optimization-Inspired_CVPR_2018_paper.html)] [[Code](https://github.com/jianzhangcs/ISTA-Net-PyTorch)]
  Unrolled ISTA into a deep network with learned nonlinear transforms for proximal mapping, achieving fast and interpretable compressive sensing image reconstruction.

## 2017

- ⭐ **Compressed Sensing using Generative Models** — ICML 2017
  [[Paper](https://arxiv.org/abs/1703.03208)] [[Code](https://github.com/AshishBora/csgm)]
  Replaced sparsity assumptions with generative model priors for compressed sensing, achieving accurate reconstruction with 5-10x fewer measurements than Lasso.

- **Learned D-AMP: Principled Neural Network based Compressive Image Recovery** — NeurIPS 2017
  [[Paper](https://arxiv.org/abs/1704.06625)] [[Code](https://github.com/ricedsp/D-AMP_Toolbox)]
  Designed a neural network mimicking denoising-based approximate message passing for compressive image recovery, running 50x faster than BM3D-AMP.

- **Learning to Invert: Signal Recovery via Deep Convolutional Networks** — ICASSP 2017
  [[Paper](https://arxiv.org/abs/1701.03891)]
  Proposed DeepInverse, a deep convolutional network that directly learns the inverse mapping from compressive measurements to signals without iterative optimization.

## 2016

- **Deep ADMM-Net for Compressive Sensing MRI** — NeurIPS 2016 [`Algorithm Unrolling`]
  [[Paper](https://papers.nips.cc/paper/6406-deep-admm-net-for-compressive-sensing-mri)] [[Code](https://github.com/yangyan92/Deep-ADMM-Net)]
  Unrolled the ADMM optimization algorithm into a deep network with learnable transforms and shrinkage functions for MRI reconstruction, achieving fast and accurate CS recovery.

## Benchmark Datasets

| Dataset | Task | Description |
|:---|:---|:---|
| **Set11 / BSD68 / Urban100** | CS image reconstruction | Natural-image benchmarks reused for CS evaluation |
| **fastMRI** | MRI reconstruction | 1,500+ knee / brain MRI volumes; standard undersampled reconstruction benchmark |
| **Calgary-Campinas / SKM-TEA** | MRI reconstruction | Multi-coil brain / knee MRI benchmarks |
| **Mayo Low-Dose CT** | CT reconstruction | AAPM Low-Dose CT Grand Challenge data |
| **FFHQ / ImageNet validation** | Diffusion inverse problems | Used by DPS, ReSample, IDM, DiffStateGrad |
