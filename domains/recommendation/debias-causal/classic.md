# Classic — Debiasing / Fairness / Causal Recommendation

Foundational works (2015–2018) that established propensity-weighting, doubly robust estimation, and causal embeddings as tools for unbiased recommendation learning and evaluation.

#### Foundations

### Recommendations as Treatments: Debiasing Learning and Evaluation
- **Authors:** Schnabel et al.
- **Venue:** ICML 2016
- **Paper:** [ArXiv](https://arxiv.org/abs/1602.05352)
- **Summary:** Frames recommendation as a causal inference problem under MNAR (missing-not-at-random) data, applying inverse propensity scoring (IPS) to debias both learning and evaluation of recommender systems.
- **Tags:** `#ips` `#propensity` `#seminal`

### Causal Embeddings for Recommendation
- **Authors:** Bonner & Vasile
- **Venue:** RecSys 2018
- **Paper:** [ArXiv](https://arxiv.org/abs/1706.07639)
- **Summary:** Learns item embeddings that disentangle causal from confounded signals by jointly optimizing uniformly sampled and biased data, producing embeddings robust to exposure bias.
- **Tags:** `#causal-embeddings`

### The Self-Normalized Estimator for Counterfactual Learning
- **Authors:** Swaminathan & Joachims
- **Venue:** NeurIPS 2015
- **Paper:** [NeurIPS Proceedings](https://proceedings.neurips.cc/paper/2015/hash/39027dfad5138c9ca0c474d71db915c3-Abstract.html)
- **Summary:** SNIPS introduces self-normalized IPS to reduce variance of propensity-weighted counterfactual estimators, a key building block for doubly robust recommendation debiasing methods.
- **Tags:** `#snips` `#counterfactual`
