# Classic — Generative Recommendation

Foundational works (2022–2023) that established generative retrieval as a recommendation paradigm, seeded by differentiable search indices from IR and realized through semantic item IDs.

#### Paradigm Launch (2022-2023)

### Recommender Systems with Generative Retrieval
- **Authors:** Rajput et al.
- **Venue:** NeurIPS 2023
- **Paper:** [ArXiv](https://arxiv.org/abs/2305.05065)
- **Summary:** TIGER assigns hierarchical semantic IDs to items via RQ-VAE and trains a sequence-to-sequence model to generate item IDs auto-regressively, enabling end-to-end generative recommendation without separate retrieval and ranking stages.
- **Tags:** `#tiger` `#semantic-id` `#seminal`

### Transformer Memory as a Differentiable Search Index
- **Authors:** Tay et al.
- **Venue:** NeurIPS 2022
- **Paper:** [ArXiv](https://arxiv.org/abs/2202.06991)
- **Summary:** DSI shows that a single transformer can memorize a corpus and retrieve documents by generating their IDs, directly seeding the generative-rec direction. From IR literature; foundational to TIGER and subsequent generative recommenders.
- **Tags:** `#dsi` `#generative-retrieval` `#ir-origin`
