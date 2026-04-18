# Misc / Surveys — Collaborative Filtering & Matrix Factorization

Surveys, benchmark studies, and cross-year works that do not belong to a single year file.

## Surveys & Tutorials

### Matrix Factorization Techniques for Recommender Systems
- **Authors:** Koren, Bell, Volinsky
- **Venue:** IEEE Computer 2009
- **Paper:** [IEEE Computer Magazine](https://ieeexplore.ieee.org/document/5197422)
- **Summary:** The canonical review of matrix factorization for recommendation; covers biased MF, temporal dynamics, and confidence weighting. While foundational, it remains the most-cited entry point for new researchers entering the CF-MF paradigm.
- **Tags:** `#survey` `#mf` `#seminal`

### Collaborative Filtering beyond the User-Item Matrix: A Survey of the State of the Art and Future Challenges
- **Authors:** Shi et al.
- **Venue:** ACM Computing Surveys 2014
- **Paper:** (search: Collaborative Filtering Beyond User-Item Matrix Survey Shi 2014 ACM Computing Surveys)
- **Summary:** Comprehensive survey of CF extensions including social networks, contextual information, and multi-criteria ratings, mapping the landscape before the deep learning era.
- **Tags:** `#survey` `#cf` `#context-aware`

## Benchmark & Reproducibility Studies

### Are We Really Making Much Progress? A Worrying Analysis of Recent Neural Recommendation Approaches
- **Authors:** Dacrema et al.
- **Venue:** RecSys 2019
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/3298689.3347058)
- **Code:** [GitHub](https://github.com/MaurizioFD/RecSys2019_DeepLearning_Evaluation)
- **Summary:** Systematic reproducibility study showing that many proposed deep CF models cannot outperform simple tuned baselines (ItemKNN, P3alpha, RP3beta) on standard benchmarks; a landmark paper that improved rigor in the CF evaluation community.
- **Tags:** `#reproducibility` `#benchmark` `#cf`

### SimpleX: A Simple and Strong Baseline for Collaborative Filtering
- **Authors:** Mao et al.
- **Venue:** CIKM 2021
- **Paper:** [arXiv](https://arxiv.org/abs/2109.12613)
- **Code:** [GitHub](https://github.com/xue-pai/Open-CF-Benchmarks)
- **Summary:** Proposes a cosine-contrastive loss with large negative sampling as a surprisingly strong CF baseline; comprehensively benchmarks against graph- and attention-based models and finds that the simple model often matches GNN CF on standard datasets.
- **Tags:** `#simplex` `#baseline` `#contrastive` `#cf`

## Negative Sampling Studies

### Sampling-Bias-Corrected Neural Modeling for Large Corpus Item Recommendations
- **Authors:** Yi et al.
- **Venue:** RecSys 2019
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/3298689.3346996)
- **Summary:** Proposes frequency-based correction for in-batch negative sampling in two-tower models, accounting for item popularity in the training corpus; widely adopted in industrial two-tower systems at Google/YouTube.
- **Tags:** `#negative-sampling` `#two-tower` `#industrial`
