# Design: awesome-machine-learning-papers

## Overview

An open-source, community-driven collection of classic and recent machine learning papers from top venues, organized by **domain direction** and **technique direction** as two independent dimensions.

- **Audience**: Open-source community (GitHub awesome-list style)
- **Language**: English only
- **Venue scope**: CCF-A venues prioritized; high-impact papers from CCF-B venues also included

## Project Structure

```
README.md
├── domains/
│   ├── cv.md
│   ├── nlp.md
│   ├── time-series.md
│   ├── speech.md
│   ├── graph.md
│   └── multimodal.md
├── techniques/
│   ├── rnn.md
│   ├── cnn.md
│   ├── transformer.md
│   ├── mamba.md
│   ├── gan.md
│   ├── diffusion.md
│   └── gnn.md
└── CONTRIBUTING.md
```

### Design rationale

Technique papers (e.g., the original Transformer paper) are cross-domain and general-purpose. Domain papers (e.g., applying Transformer to time series) are domain-specific applications. These two categories are fundamentally different and should be organized separately.

## README.md

The README serves as the entry point and navigation hub. It contains:

1. **Title + badges** — awesome badge, star count, contributor count
2. **Project introduction** — one paragraph describing the project: curated ML papers from top venues, organized by domain and technique
3. **Navigation tables** — two tables listing all domain files and technique files with links and paper counts
4. **How to Contribute** — brief instructions pointing to CONTRIBUTING.md
5. **License**

The README does NOT contain paper entries — it is purely a navigation page.

## Paper Entry Format

Every paper follows this uniform format:

```markdown
- **Paper Title** — Venue Year [`tag1`] [`tag2`]
  [[Paper](link)] [[Code](link)]
  Brief one-sentence summary of the core contribution.
```

### Example

```markdown
- ⭐ **Attention Is All You Need** — NeurIPS 2017 [`Attention`] [`Encoder-Decoder`]
  [[Paper](https://arxiv.org/abs/1706.03762)] [[Code](https://github.com/tensorflow/tensor2tensor)]
  Proposed the Transformer architecture, replacing recurrence with self-attention for sequence modeling.
```

### Rules

- **Tags**: Domain files tag technique directions (e.g., `Transformer`, `CNN`). Technique files tag domain directions (e.g., `CV`, `NLP`).
- **Code link**: Include when an official repository exists; omit otherwise.
- **One-sentence summary**: Describes the core contribution, one line max.
- **Landmark marker**: Pioneering/foundational papers are prefixed with ⭐. All other papers have no prefix.
- **Ordering**: Papers are sorted by year in descending order (newest first) within each file.

## File Template

Each domain/technique file uses this template:

```markdown
# Category Name (Abbreviation)

A collection of must-read papers in [category] from top venues.

- ⭐ **Landmark Paper** — Venue Year [`tag`]
  [[Paper](link)] [[Code](link)]
  One-sentence summary.

- **Regular Paper** — Venue Year [`tag`]
  [[Paper](link)] [[Code](link)]
  One-sentence summary.
```

No time-based sections. All papers in a single list, sorted by year descending.

## Initial Coverage

### Domain directions (domains/)

| File | Domain | Scope |
|------|--------|-------|
| `cv.md` | Computer Vision | Image classification, object detection, semantic segmentation, etc. |
| `nlp.md` | Natural Language Processing | Text classification, machine translation, QA, etc. |
| `time-series.md` | Time Series Forecasting | Time series prediction, classification |
| `speech.md` | Speech & Audio | Speech recognition, synthesis, audio understanding |
| `graph.md` | Graph Learning | Node classification, link prediction, graph generation |
| `multimodal.md` | Multimodal Learning | Vision-language, cross-modal retrieval, etc. |

### Technique directions (techniques/)

| File | Technique | Scope |
|------|-----------|-------|
| `rnn.md` | RNN / LSTM / GRU | Recurrent networks and variants |
| `cnn.md` | CNN | Convolutional network architecture evolution |
| `transformer.md` | Transformer & Attention | Self-attention mechanisms and Transformer variants |
| `mamba.md` | Mamba & State Space Models | SSM and selective state space models |
| `gan.md` | GAN | Generative adversarial networks |
| `diffusion.md` | Diffusion Models | Diffusion models, score-based models |
| `gnn.md` | Graph Neural Networks | Graph convolution, message passing networks |

New files can be added as needed without affecting existing structure.

## CONTRIBUTING.md

### What to contribute

- **Venue criteria**: CCF-A papers prioritized; high-citation/high-impact CCF-B papers also accepted
- **Welcome contributions**: New papers, missing classics, code links, summary improvements

### How to contribute

- Fork → add paper in the correct file following the format → submit PR
- PR title format: `Add <Paper Title> to <category>`
- Every paper must include: title, venue/year, paper link, one-sentence summary, technique or domain tags
- ⭐ marker is reserved for widely recognized pioneering papers; PRs adding this marker must justify it in the PR description

### Formatting rules

- Use the paper entry template strictly
- Sort by year descending within each file
- Proposing a new domain or technique direction requires opening an Issue first for discussion
