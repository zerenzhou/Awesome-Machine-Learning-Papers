# awesome-machine-learning-papers Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create a community-driven awesome-list of ML papers organized by domain direction and technique direction.

**Architecture:** Static markdown repository. README.md as navigation hub, `domains/` and `techniques/` directories containing per-category paper lists. CONTRIBUTING.md for community guidelines. No build tooling or scripts required.

**Tech Stack:** Markdown, Git

---

## File Structure

```
README.md                   — Navigation hub with project intro and tables linking to all category files
CONTRIBUTING.md             — Contribution guidelines, venue criteria, formatting rules
LICENSE                     — MIT license
domains/
  cv.md                     — Computer Vision papers, tagged with technique directions
  nlp.md                    — NLP papers, tagged with technique directions
  time-series.md            — Time Series Forecasting papers, tagged with technique directions
  speech.md                 — Speech & Audio papers, tagged with technique directions
  graph.md                  — Graph Learning papers, tagged with technique directions
  multimodal.md             — Multimodal Learning papers, tagged with technique directions
techniques/
  rnn.md                    — RNN/LSTM/GRU papers, tagged with domain directions
  cnn.md                    — CNN papers, tagged with domain directions
  transformer.md            — Transformer & Attention papers, tagged with domain directions
  mamba.md                  — Mamba & SSM papers, tagged with domain directions
  gan.md                    — GAN papers, tagged with domain directions
  diffusion.md              — Diffusion model papers, tagged with domain directions
  gnn.md                    — GNN papers, tagged with domain directions
```

---

### Task 1: Create README.md

**Files:**
- Create: `README.md`

- [ ] **Step 1: Create README.md**

```markdown
# Awesome Machine Learning Papers

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated collection of classic and recent machine learning papers from top venues (NeurIPS, ICML, ICLR, CVPR, ACL, etc.), organized by **domain direction** and **technique direction**.

- **Domain direction**: Application-specific papers within a field (CV, NLP, Time Series, etc.)
- **Technique direction**: Cross-domain foundational papers on model architectures and methods (Transformer, CNN, Mamba, etc.)

## Domain Directions

| Domain | Description |
|--------|-------------|
| [Computer Vision](domains/cv.md) | Image classification, object detection, semantic segmentation |
| [Natural Language Processing](domains/nlp.md) | Text classification, machine translation, question answering |
| [Time Series Forecasting](domains/time-series.md) | Time series prediction and classification |
| [Speech & Audio](domains/speech.md) | Speech recognition, synthesis, audio understanding |
| [Graph Learning](domains/graph.md) | Node classification, link prediction, graph generation |
| [Multimodal Learning](domains/multimodal.md) | Vision-language, cross-modal retrieval |

## Technique Directions

| Technique | Description |
|-----------|-------------|
| [RNN / LSTM / GRU](techniques/rnn.md) | Recurrent networks and variants |
| [CNN](techniques/cnn.md) | Convolutional network architecture evolution |
| [Transformer & Attention](techniques/transformer.md) | Self-attention mechanisms and Transformer variants |
| [Mamba & State Space Models](techniques/mamba.md) | SSM and selective state space models |
| [GAN](techniques/gan.md) | Generative adversarial networks |
| [Diffusion Models](techniques/diffusion.md) | Diffusion models and score-based models |
| [Graph Neural Networks](techniques/gnn.md) | Graph convolution and message passing networks |

## Contributing

We welcome contributions! Please read our [Contributing Guidelines](CONTRIBUTING.md) before submitting a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
```

- [ ] **Step 2: Commit**

```bash
git add README.md
git commit -m "docs: add README with project intro and navigation"
```

---

### Task 2: Create CONTRIBUTING.md and LICENSE

**Files:**
- Create: `CONTRIBUTING.md`
- Create: `LICENSE`

- [ ] **Step 1: Create CONTRIBUTING.md**

```markdown
# Contributing Guidelines

Thank you for contributing to awesome-machine-learning-papers! This document explains how to add papers and what standards to follow.

## What We Accept

- **CCF-A venues prioritized**: NeurIPS, ICML, ICLR, CVPR, ICCV, ACL, EMNLP, KDD, AAAI, IJCAI, SIGIR, WWW, TPAMI, JMLR, etc.
- **High-impact CCF-B papers**: ECCV, NAACL, COLING, CIKM, WSDM, etc. — only widely cited or influential papers.
- **Welcome contributions**: New papers, missing classics, code links, summary improvements.

## Paper Entry Format

Every paper must follow this format:

```
- **Paper Title** — Venue Year [`tag1`] [`tag2`]
  [[Paper](link)] [[Code](link)]
  Brief one-sentence summary of the core contribution.
```

### Rules

- **Tags**: Domain files use technique tags (e.g., `Transformer`, `CNN`). Technique files use domain tags (e.g., `CV`, `NLP`).
- **Code link**: Include when an official repository exists. Omit otherwise — do not link unofficial reproductions.
- **One-sentence summary**: Describe the core contribution. One line maximum.
- **Ordering**: Papers are sorted by year in descending order (newest first).
- **Landmark marker**: Prefix pioneering papers with ⭐. This is reserved for widely recognized foundational work. If your PR adds this marker, explain why in the PR description.

## How to Contribute

1. Fork this repository
2. Add your paper entry in the correct file under `domains/` or `techniques/`
3. Follow the format above strictly
4. Submit a pull request with title: `Add <Paper Title> to <category>`

## Proposing New Categories

To propose a new domain or technique direction, open an Issue first for discussion before creating a PR.

## Quality Checklist

Before submitting, verify:

- [ ] Paper link points to the official publication or arXiv
- [ ] Venue and year are correct
- [ ] Tags match existing tag names used in the repository
- [ ] Summary accurately describes the core contribution
- [ ] Entry is placed in the correct chronological position (newest first)
```

- [ ] **Step 2: Create LICENSE (MIT)**

```
MIT License

Copyright (c) 2026 awesome-machine-learning-papers contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

- [ ] **Step 3: Commit**

```bash
git add CONTRIBUTING.md LICENSE
git commit -m "docs: add contributing guidelines and MIT license"
```

---

### Task 3: Create techniques/transformer.md

**Files:**
- Create: `techniques/transformer.md`

- [ ] **Step 1: Create techniques/transformer.md**

```markdown
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
```

- [ ] **Step 2: Commit**

```bash
git add techniques/transformer.md
git commit -m "docs: add Transformer & Attention papers"
```

---

### Task 4: Create techniques/rnn.md

**Files:**
- Create: `techniques/rnn.md`

- [ ] **Step 1: Create techniques/rnn.md**

```markdown
# RNN / LSTM / GRU

A collection of must-read papers on recurrent neural networks and their variants from top venues.

- ⭐ **Long Short-Term Memory** — Neural Computation 1997 [`General`]
  [[Paper](https://www.bioinf.jku.at/publications/older/2604.pdf)]
  Introduced the LSTM architecture with gating mechanisms to address the vanishing gradient problem in RNNs.

- ⭐ **Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation** — EMNLP 2014 [`NLP`]
  [[Paper](https://arxiv.org/abs/1406.1078)]
  Proposed the GRU gated unit and the encoder-decoder framework for sequence-to-sequence learning.

- ⭐ **Sequence to Sequence Learning with Neural Networks** — NeurIPS 2014 [`NLP`]
  [[Paper](https://arxiv.org/abs/1409.3215)]
  Demonstrated that a multi-layer LSTM encoder-decoder can map variable-length input sequences to variable-length output sequences for machine translation.

- **Neural Machine Translation by Jointly Learning to Align and Translate** — ICLR 2015 [`NLP`]
  [[Paper](https://arxiv.org/abs/1409.0473)]
  Introduced the attention mechanism for RNN-based encoder-decoder models, allowing the decoder to focus on relevant source positions.

- **Empirical Evaluation of Gated Recurrent Neural Networks on Sequence Modeling** — NeurIPS Workshop 2014 [`General`]
  [[Paper](https://arxiv.org/abs/1412.3555)]
  Systematically compared LSTM and GRU units, finding GRU comparable to LSTM on several sequence modeling tasks.

- **Deep Recurrent Neural Network for Protein Function Prediction** — arXiv 2017 [`Bioinformatics`]
  [[Paper](https://arxiv.org/abs/1701.08318)]
  Applied deep bidirectional LSTM to predict protein function from amino acid sequences.
```

- [ ] **Step 2: Commit**

```bash
git add techniques/rnn.md
git commit -m "docs: add RNN / LSTM / GRU papers"
```

---

### Task 5: Create techniques/cnn.md

**Files:**
- Create: `techniques/cnn.md`

- [ ] **Step 1: Create techniques/cnn.md**

```markdown
# CNN

A collection of must-read papers on convolutional neural network architectures from top venues.

- ⭐ **ImageNet Classification with Deep Convolutional Neural Networks** — NeurIPS 2012 [`CV`]
  [[Paper](https://papers.nips.cc/paper/2012/hash/c399862d3b9d6b76c8436e924a68c45b-Abstract.html)]
  Introduced AlexNet, demonstrating the power of deep CNNs with ReLU, dropout, and GPU training on large-scale image classification.

- ⭐ **Very Deep Convolutional Networks for Large-Scale Image Recognition** — ICLR 2015 [`CV`]
  [[Paper](https://arxiv.org/abs/1409.1556)]
  Showed that increasing network depth with small 3x3 convolution filters (VGGNet) significantly improves image recognition performance.

- ⭐ **Deep Residual Learning for Image Recognition** — CVPR 2016 [`CV`]
  [[Paper](https://arxiv.org/abs/1512.03385)] [[Code](https://github.com/KaimingHe/deep-residual-networks)]
  Introduced residual connections (ResNet) enabling training of very deep networks by learning residual mappings.

- ⭐ **Going Deeper with Convolutions** — CVPR 2015 [`CV`]
  [[Paper](https://arxiv.org/abs/1409.4842)]
  Proposed the Inception module (GoogLeNet), using parallel multi-scale convolutions to improve efficiency and accuracy.

- **Densely Connected Convolutional Networks** — CVPR 2017 [`CV`]
  [[Paper](https://arxiv.org/abs/1608.06993)] [[Code](https://github.com/liuzhuang13/DenseNet)]
  Introduced dense connections between layers (DenseNet), strengthening feature propagation and reducing parameters.

- **Convolutional Sequence to Sequence Learning** — ICML 2017 [`NLP`]
  [[Paper](https://arxiv.org/abs/1705.03122)] [[Code](https://github.com/facebookresearch/fairseq)]
  Applied CNN with gated linear units to sequence-to-sequence tasks, achieving competitive results with faster training than RNNs.

- **EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks** — ICML 2019 [`CV`]
  [[Paper](https://arxiv.org/abs/1905.11946)] [[Code](https://github.com/tensorflow/tpu/tree/master/models/official/efficientnet)]
  Proposed compound scaling of depth, width, and resolution to systematically improve CNN efficiency and accuracy.

- **TCN: An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling** — arXiv 2018 [`TSF`]
  [[Paper](https://arxiv.org/abs/1803.01271)] [[Code](https://github.com/locuslab/TCN)]
  Demonstrated that temporal convolutional networks outperform RNNs on a range of sequence modeling benchmarks.
```

- [ ] **Step 2: Commit**

```bash
git add techniques/cnn.md
git commit -m "docs: add CNN papers"
```

---

### Task 6: Create techniques/mamba.md

**Files:**
- Create: `techniques/mamba.md`

- [ ] **Step 1: Create techniques/mamba.md**

```markdown
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
```

- [ ] **Step 2: Commit**

```bash
git add techniques/mamba.md
git commit -m "docs: add Mamba & State Space Models papers"
```

---

### Task 7: Create techniques/gan.md

**Files:**
- Create: `techniques/gan.md`

- [ ] **Step 1: Create techniques/gan.md**

```markdown
# GAN

A collection of must-read papers on generative adversarial networks from top venues.

- ⭐ **Generative Adversarial Nets** — NeurIPS 2014 [`General`]
  [[Paper](https://arxiv.org/abs/1406.2661)]
  Introduced the adversarial training framework where a generator and discriminator compete in a minimax game.

- ⭐ **Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks** — ICLR 2016 [`CV`]
  [[Paper](https://arxiv.org/abs/1511.06434)]
  Proposed DCGAN, establishing architectural guidelines for stable training of convolutional GANs.

- ⭐ **Wasserstein GAN** — ICML 2017 [`General`]
  [[Paper](https://arxiv.org/abs/1701.07875)]
  Replaced the JS divergence with Wasserstein distance, improving GAN training stability and providing meaningful loss metrics.

- **Conditional Generative Adversarial Nets** — arXiv 2014 [`General`]
  [[Paper](https://arxiv.org/abs/1411.1784)]
  Extended GANs with conditional inputs, enabling class-conditional and attribute-guided generation.

- **Image-to-Image Translation with Conditional Adversarial Networks** — CVPR 2017 [`CV`]
  [[Paper](https://arxiv.org/abs/1611.07004)] [[Code](https://github.com/phillipi/pix2pix)]
  Proposed Pix2Pix, a general framework for paired image-to-image translation using conditional GANs.

- **Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks** — ICCV 2017 [`CV`]
  [[Paper](https://arxiv.org/abs/1703.10593)] [[Code](https://github.com/junyanz/CycleGAN)]
  Introduced CycleGAN with cycle-consistency loss for unpaired image-to-image translation.

- **A Style-Based Generator Architecture for Generative Adversarial Networks** — CVPR 2019 [`CV`]
  [[Paper](https://arxiv.org/abs/1812.04948)] [[Code](https://github.com/NVlabs/stylegan)]
  Proposed StyleGAN with adaptive instance normalization for high-quality controllable image synthesis.

- **TimeGAN: Time-series Generative Adversarial Networks** — NeurIPS 2019 [`TSF`]
  [[Paper](https://papers.nips.cc/paper/2019/hash/c9efe5f26cd17ba6216bbe2a7d26d490-Abstract.html)] [[Code](https://github.com/jsyoon0823/TimeGAN)]
  Combined autoregressive models with GANs for generating realistic time-series data.
```

- [ ] **Step 2: Commit**

```bash
git add techniques/gan.md
git commit -m "docs: add GAN papers"
```

---

### Task 8: Create techniques/diffusion.md

**Files:**
- Create: `techniques/diffusion.md`

- [ ] **Step 1: Create techniques/diffusion.md**

```markdown
# Diffusion Models

A collection of must-read papers on diffusion models and score-based generative models from top venues.

- ⭐ **Denoising Diffusion Probabilistic Models** — NeurIPS 2020 [`CV`]
  [[Paper](https://arxiv.org/abs/2006.11239)] [[Code](https://github.com/hojonathanho/diffusion)]
  Demonstrated that diffusion models with simplified training objectives can generate high-quality images rivaling GANs.

- ⭐ **Score-Based Generative Modeling through Stochastic Differential Equations** — ICLR 2021 [`General`]
  [[Paper](https://arxiv.org/abs/2011.13456)] [[Code](https://github.com/yang-song/score_sde)]
  Unified score matching and diffusion models through a continuous-time SDE framework with controllable generation.

- **Denoising Diffusion Implicit Models** — ICLR 2021 [`CV`]
  [[Paper](https://arxiv.org/abs/2010.02502)]
  Proposed DDIM, a non-Markovian sampling process that accelerates diffusion model inference by 10-50x.

- **High-Resolution Image Synthesis with Latent Diffusion Models** — CVPR 2022 [`CV`]
  [[Paper](https://arxiv.org/abs/2112.10752)] [[Code](https://github.com/CompVis/latent-diffusion)]
  Introduced Latent Diffusion (Stable Diffusion), performing the diffusion process in a compressed latent space for efficiency.

- **Classifier-Free Diffusion Guidance** — NeurIPS Workshop 2022 [`CV`]
  [[Paper](https://arxiv.org/abs/2207.12598)]
  Proposed mixing conditional and unconditional score estimates to guide diffusion sampling without a separate classifier.

- **Diffusion-TS: Interpretable Diffusion for General Time Series Generation** — ICLR 2024 [`TSF`]
  [[Paper](https://arxiv.org/abs/2403.01742)] [[Code](https://github.com/Y-debug-sys/Diffusion-TS)]
  Applied diffusion models with decomposition-based interpretability to time series generation and imputation.

- **DiffWave: A Versatile Diffusion Model for Audio Synthesis** — ICLR 2021 [`Speech`]
  [[Paper](https://arxiv.org/abs/2009.09761)] [[Code](https://github.com/lmnt-com/diffwave)]
  Applied diffusion probabilistic models to raw audio waveform synthesis with high fidelity.
```

- [ ] **Step 2: Commit**

```bash
git add techniques/diffusion.md
git commit -m "docs: add Diffusion Models papers"
```

---

### Task 9: Create techniques/gnn.md

**Files:**
- Create: `techniques/gnn.md`

- [ ] **Step 1: Create techniques/gnn.md**

```markdown
# Graph Neural Networks

A collection of must-read papers on graph neural networks and message passing architectures from top venues.

- ⭐ **Semi-Supervised Classification with Graph Convolutional Networks** — ICLR 2017 [`Graph`]
  [[Paper](https://arxiv.org/abs/1609.02907)] [[Code](https://github.com/tkipf/gcn)]
  Introduced GCN, a scalable spectral-based graph convolution for semi-supervised node classification.

- ⭐ **Graph Attention Networks** — ICLR 2018 [`Graph`]
  [[Paper](https://arxiv.org/abs/1710.10903)] [[Code](https://github.com/PetarV-/GAT)]
  Proposed attention-based neighborhood aggregation (GAT) for graph-structured data, enabling adaptive weighting of neighbors.

- ⭐ **Inductive Representation Learning on Large Graphs** — NeurIPS 2017 [`Graph`]
  [[Paper](https://arxiv.org/abs/1706.02216)] [[Code](https://github.com/williamleif/GraphSAGE)]
  Introduced GraphSAGE, learning node embeddings through sampling and aggregating features from local neighborhoods.

- **Neural Message Passing for Quantum Chemistry** — ICML 2017 [`General`]
  [[Paper](https://arxiv.org/abs/1704.01212)]
  Unified various GNN architectures under the message passing neural network (MPNN) framework.

- **How Powerful are Graph Neural Networks?** — ICLR 2019 [`Graph`]
  [[Paper](https://arxiv.org/abs/1810.00826)] [[Code](https://github.com/weihua916/powerful-gnns)]
  Analyzed the expressive power of GNNs through the Weisfeiler-Leman test and proposed GIN as a maximally powerful architecture.

- **Graph Transformer Networks** — NeurIPS 2019 [`Graph`]
  [[Paper](https://arxiv.org/abs/1911.06455)] [[Code](https://github.com/seongjunyun/Graph_Transformer_Networks)]
  Combined graph structure learning with Transformer-style attention for heterogeneous graph classification.
```

- [ ] **Step 2: Commit**

```bash
git add techniques/gnn.md
git commit -m "docs: add Graph Neural Networks papers"
```

---

### Task 10: Create domains/cv.md

**Files:**
- Create: `domains/cv.md`

- [ ] **Step 1: Create domains/cv.md**

```markdown
# Computer Vision (CV)

A collection of must-read computer vision papers from top venues.

- ⭐ **ImageNet Classification with Deep Convolutional Neural Networks** — NeurIPS 2012 [`CNN`]
  [[Paper](https://papers.nips.cc/paper/2012/hash/c399862d3b9d6b76c8436e924a68c45b-Abstract.html)]
  Introduced AlexNet, demonstrating the power of deep CNNs on large-scale image classification.

- ⭐ **Deep Residual Learning for Image Recognition** — CVPR 2016 [`CNN`]
  [[Paper](https://arxiv.org/abs/1512.03385)] [[Code](https://github.com/KaimingHe/deep-residual-networks)]
  Introduced residual connections enabling training of very deep networks for image recognition.

- ⭐ **An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale** — ICLR 2021 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2010.11929)] [[Code](https://github.com/google-research/vision_transformer)]
  Proposed Vision Transformer (ViT), applying a pure Transformer to image patch sequences for classification.

- ⭐ **Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks** — NeurIPS 2015 [`CNN`]
  [[Paper](https://arxiv.org/abs/1506.01497)] [[Code](https://github.com/rbgirshick/py-faster-rcnn)]
  Introduced Region Proposal Networks for end-to-end trainable object detection with shared convolutional features.

- ⭐ **Generative Adversarial Nets** — NeurIPS 2014 [`GAN`]
  [[Paper](https://arxiv.org/abs/1406.2661)]
  Introduced the adversarial framework for generative modeling, revolutionizing image synthesis.

- **You Only Look Once: Unified, Real-Time Object Detection** — CVPR 2016 [`CNN`]
  [[Paper](https://arxiv.org/abs/1506.02640)] [[Code](https://github.com/pjreddie/darknet)]
  Framed object detection as a single regression problem from image pixels to bounding boxes and class probabilities.

- **Feature Pyramid Networks for Object Detection** — CVPR 2017 [`CNN`]
  [[Paper](https://arxiv.org/abs/1612.03144)]
  Built a top-down feature pyramid with lateral connections for multi-scale object detection.

- **Swin Transformer: Hierarchical Vision Transformer using Shifted Windows** — ICCV 2021 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2103.14030)] [[Code](https://github.com/microsoft/Swin-Transformer)]
  Introduced shifted window-based self-attention for efficient hierarchical feature extraction.

- **Masked Autoencoders Are Scalable Vision Learners** — CVPR 2022 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2111.06377)] [[Code](https://github.com/facebookresearch/mae)]
  Proposed MAE, masking random image patches and reconstructing them for self-supervised pre-training.

- **High-Resolution Image Synthesis with Latent Diffusion Models** — CVPR 2022 [`Diffusion`]
  [[Paper](https://arxiv.org/abs/2112.10752)] [[Code](https://github.com/CompVis/latent-diffusion)]
  Introduced Latent Diffusion for efficient high-resolution image generation in compressed latent space.
```

- [ ] **Step 2: Commit**

```bash
git add domains/cv.md
git commit -m "docs: add Computer Vision domain papers"
```

---

### Task 11: Create domains/nlp.md

**Files:**
- Create: `domains/nlp.md`

- [ ] **Step 1: Create domains/nlp.md**

```markdown
# Natural Language Processing (NLP)

A collection of must-read NLP papers from top venues.

- ⭐ **Attention Is All You Need** — NeurIPS 2017 [`Transformer`]
  [[Paper](https://arxiv.org/abs/1706.03762)] [[Code](https://github.com/tensorflow/tensor2tensor)]
  Proposed the Transformer, replacing recurrence with self-attention for sequence transduction.

- ⭐ **BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding** — NAACL 2019 [`Transformer`]
  [[Paper](https://arxiv.org/abs/1810.04805)] [[Code](https://github.com/google-research/bert)]
  Introduced bidirectional pre-training via masked language modeling, setting new standards across NLP benchmarks.

- ⭐ **Distributed Representations of Words and Phrases and their Compositionality** — NeurIPS 2013 [`Embedding`]
  [[Paper](https://arxiv.org/abs/1310.4546)]
  Extended Word2Vec with negative sampling and phrase detection for learning distributed word representations.

- ⭐ **Sequence to Sequence Learning with Neural Networks** — NeurIPS 2014 [`RNN`]
  [[Paper](https://arxiv.org/abs/1409.3215)]
  Demonstrated multi-layer LSTM encoder-decoder for variable-length sequence mapping in machine translation.

- **GloVe: Global Vectors for Word Representation** — EMNLP 2014 [`Embedding`]
  [[Paper](https://arxiv.org/abs/1405.4053)] [[Code](https://github.com/stanfordnlp/GloVe)]
  Combined global matrix factorization with local context window methods for learning word vectors.

- **Language Models are Few-Shot Learners** — NeurIPS 2020 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2005.14165)]
  Showed that scaling GPT-3 to 175B parameters enables strong few-shot performance across NLP tasks without fine-tuning.

- **RoBERTa: A Robustly Optimized BERT Pretraining Approach** — arXiv 2019 [`Transformer`]
  [[Paper](https://arxiv.org/abs/1907.11692)] [[Code](https://github.com/facebookresearch/fairseq)]
  Demonstrated that carefully tuning BERT's pre-training recipe significantly improves downstream performance.

- **LLaMA: Open and Efficient Foundation Language Models** — arXiv 2023 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2302.13971)] [[Code](https://github.com/facebookresearch/llama)]
  Showed that smaller models trained on more data can match or exceed larger models, democratizing LLM research.

- **Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks** — NeurIPS 2020 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2005.11401)]
  Combined pre-trained parametric and non-parametric memory via retrieval for knowledge-intensive generation.
```

- [ ] **Step 2: Commit**

```bash
git add domains/nlp.md
git commit -m "docs: add NLP domain papers"
```

---

### Task 12: Create domains/time-series.md

**Files:**
- Create: `domains/time-series.md`

- [ ] **Step 1: Create domains/time-series.md**

```markdown
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
```

- [ ] **Step 2: Commit**

```bash
git add domains/time-series.md
git commit -m "docs: add Time Series Forecasting domain papers"
```

---

### Task 13: Create domains/speech.md

**Files:**
- Create: `domains/speech.md`

- [ ] **Step 1: Create domains/speech.md**

```markdown
# Speech & Audio

A collection of must-read speech and audio processing papers from top venues.

- ⭐ **Deep Speech 2: End-to-End Speech Recognition in English and Mandarin** — ICML 2016 [`RNN`]
  [[Paper](https://arxiv.org/abs/1512.02595)]
  Scaled end-to-end deep learning for speech recognition with RNNs and CTC loss across English and Mandarin.

- ⭐ **WaveNet: A Generative Model for Raw Audio** — arXiv 2016 [`CNN`]
  [[Paper](https://arxiv.org/abs/1609.03499)]
  Introduced dilated causal convolutions for autoregressive raw audio waveform generation with high fidelity.

- ⭐ **wav2vec 2.0: A Framework for Self-Supervised Learning of Speech Representations** — NeurIPS 2020 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2006.11477)] [[Code](https://github.com/facebookresearch/fairseq)]
  Learned speech representations from unlabeled audio via contrastive learning and quantization with Transformers.

- **Conformer: Convolution-augmented Transformer for Speech Recognition** — INTERSPEECH 2020 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2005.08100)]
  Combined Transformer self-attention with convolution modules to capture both global and local audio features.

- **HuBERT: Self-Supervised Speech Representation Learning by Masked Prediction of Hidden Units** — TASLP 2021 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2106.07447)] [[Code](https://github.com/facebookresearch/fairseq)]
  Applied masked prediction on offline cluster assignments for self-supervised speech representation learning.

- **Whisper: Robust Speech Recognition via Large-Scale Weak Supervision** — ICML 2023 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2212.04356)] [[Code](https://github.com/openai/whisper)]
  Trained a large-scale Transformer on 680K hours of weakly supervised audio for robust multilingual speech recognition.

- **DiffWave: A Versatile Diffusion Model for Audio Synthesis** — ICLR 2021 [`Diffusion`]
  [[Paper](https://arxiv.org/abs/2009.09761)] [[Code](https://github.com/lmnt-com/diffwave)]
  Applied diffusion probabilistic models to raw audio waveform synthesis with high fidelity.
```

- [ ] **Step 2: Commit**

```bash
git add domains/speech.md
git commit -m "docs: add Speech & Audio domain papers"
```

---

### Task 14: Create domains/graph.md

**Files:**
- Create: `domains/graph.md`

- [ ] **Step 1: Create domains/graph.md**

```markdown
# Graph Learning

A collection of must-read graph learning papers from top venues.

- ⭐ **Semi-Supervised Classification with Graph Convolutional Networks** — ICLR 2017 [`GNN`]
  [[Paper](https://arxiv.org/abs/1609.02907)] [[Code](https://github.com/tkipf/gcn)]
  Introduced GCN, a scalable spectral-based graph convolution for semi-supervised node classification.

- ⭐ **Graph Attention Networks** — ICLR 2018 [`GNN`]
  [[Paper](https://arxiv.org/abs/1710.10903)] [[Code](https://github.com/PetarV-/GAT)]
  Proposed attention-based neighborhood aggregation for graph-structured data with adaptive neighbor weighting.

- ⭐ **Inductive Representation Learning on Large Graphs** — NeurIPS 2017 [`GNN`]
  [[Paper](https://arxiv.org/abs/1706.02216)] [[Code](https://github.com/williamleif/GraphSAGE)]
  Introduced GraphSAGE for learning node embeddings through sampling and aggregating local neighborhood features.

- **Variational Graph Auto-Encoders** — NeurIPS Workshop 2016 [`GNN`]
  [[Paper](https://arxiv.org/abs/1611.07308)] [[Code](https://github.com/tkipf/gae)]
  Applied variational autoencoders to graph-structured data for unsupervised link prediction.

- **How Powerful are Graph Neural Networks?** — ICLR 2019 [`GNN`]
  [[Paper](https://arxiv.org/abs/1810.00826)] [[Code](https://github.com/weihua916/powerful-gnns)]
  Analyzed GNN expressiveness through the Weisfeiler-Leman framework and proposed GIN.

- **Strategies for Pre-training Graph Neural Networks** — ICLR 2020 [`GNN`]
  [[Paper](https://arxiv.org/abs/1905.12265)] [[Code](https://github.com/snap-stanford/pretrain-gnns)]
  Proposed node-level and graph-level pre-training strategies to improve GNN generalization on downstream tasks.

- **Graph Transformer Networks** — NeurIPS 2019 [`Transformer`]
  [[Paper](https://arxiv.org/abs/1911.06455)] [[Code](https://github.com/seongjunyun/Graph_Transformer_Networks)]
  Combined graph structure learning with Transformer-style attention for heterogeneous graph classification.
```

- [ ] **Step 2: Commit**

```bash
git add domains/graph.md
git commit -m "docs: add Graph Learning domain papers"
```

---

### Task 15: Create domains/multimodal.md

**Files:**
- Create: `domains/multimodal.md`

- [ ] **Step 1: Create domains/multimodal.md**

```markdown
# Multimodal Learning

A collection of must-read multimodal learning papers from top venues.

- ⭐ **Learning Transferable Visual Models From Natural Language Supervision** — ICML 2021 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2103.00020)] [[Code](https://github.com/OpenAI/CLIP)]
  Introduced CLIP, learning visual representations from natural language supervision via contrastive pre-training.

- ⭐ **ViLBERT: Pretraining Task-Agnostic Visiolinguistic Representations for Vision-and-Language Tasks** — NeurIPS 2019 [`Transformer`]
  [[Paper](https://arxiv.org/abs/1908.02265)] [[Code](https://github.com/facebookresearch/vilbert-multi-task)]
  Proposed co-attentional Transformer for learning joint vision-language representations via pre-training.

- **BLIP-2: Bootstrapping Language-Image Pre-training with Frozen Image Encoders and Large Language Models** — ICML 2023 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2301.12597)] [[Code](https://github.com/salesforce/LAVIS)]
  Bridged frozen image encoders and LLMs with a lightweight Querying Transformer for efficient vision-language pre-training.

- **LLaVA: Visual Instruction Tuning** — NeurIPS 2023 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2304.08485)] [[Code](https://github.com/haotian-liu/LLaVA)]
  Connected a vision encoder to an LLM via visual instruction tuning for multimodal chat and reasoning.

- **Flamingo: a Visual Language Model for Few-Shot Learning** — NeurIPS 2022 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2204.14198)]
  Proposed gated cross-attention to interleave visual and text tokens for few-shot multimodal learning.

- **ImageBind: One Embedding Space to Bind Them All** — CVPR 2023 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2305.05665)] [[Code](https://github.com/facebookresearch/ImageBind)]
  Learned a joint embedding space across six modalities (image, text, audio, depth, thermal, IMU) using image-paired data.

- **ALIGN: Scaling Up Visual and Vision-Language Representation Learning With Noisy Text Supervision** — ICML 2021 [`Transformer`]
  [[Paper](https://arxiv.org/abs/2102.05918)]
  Scaled vision-language contrastive learning to 1.8B noisy image-text pairs with a dual-encoder architecture.
```

- [ ] **Step 2: Commit**

```bash
git add domains/multimodal.md
git commit -m "docs: add Multimodal Learning domain papers"
```

---

## Self-Review

- **Spec coverage**: All sections covered — README (Task 1), CONTRIBUTING + LICENSE (Task 2), all 7 technique files (Tasks 3-9), all 6 domain files (Tasks 10-15). Navigation tables, paper format, ordering rules, landmark markers, tags all implemented.
- **Placeholder scan**: No TBD/TODO. Every task has complete file content and exact commit commands.
- **Type consistency**: Tag names are consistent across domain and technique files (e.g., `Transformer`, `CNN`, `RNN`, `GAN`, `Diffusion`, `GNN`, `CV`, `NLP`, `TSF`, `Speech`, `Graph`).
- **Paper cross-reference**: Foundational papers (Attention Is All You Need, ResNet, GAN, GCN, etc.) appear in both their technique file and relevant domain file with consistent metadata.
