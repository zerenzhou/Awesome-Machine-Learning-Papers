# Recommendation Systems Domain — Design Spec

**Date:** 2026-04-18
**Status:** Approved (pending user review)
**Owner:** DJarinZHOU

## 1. Goal

Add **Recommendation Systems** as a new *domain direction* under `domains/recommendation/`, providing a comprehensive, paradigm-organized curated list of must-read papers with a medium selectivity bar (~300-500 papers total), covering the full field from classical collaborative filtering to modern LLM-based and generative recommenders.

## 2. Why Now

The existing repo covers 7 domains (CV, NLP, Time Series, Speech, Graph, Multimodal, Signal Processing) but recommendation systems — one of the largest applied-ML subfields with its own top venues (SIGIR, RecSys) — is missing. Adding it fills a major gap for users researching industrial ML or doing recommender-systems research.

## 3. Scope

### 3.1 In Scope

- **10 sub-paradigms**, each as its own subdirectory under `domains/recommendation/`
- **Selectivity:** medium (~5-15 papers per year per paradigm), target total ~300-500 papers
- **Venue coverage:** SIGIR, RecSys, KDD, WWW, NeurIPS, ICML, ICLR, CIKM, AAAI, IJCAI, ACL, TOIS
- **Year span:** classical works from ~1994; year files from ~2016 onward
- **Language:** English (consistent with existing domains)

### 3.2 Out of Scope

- Multimodal recommendation as a standalone paradigm (papers living at the intersection go into their closest primary paradigm, e.g., LLM4Rec or Graph)
- Conversational recommendation as a standalone paradigm (folded into LLM4Rec when relevant)
- Cold-start / multi-task as standalone paradigms (included within CTR-Ranking or Sequential-Rec where they primarily appear)
- Benchmarks leaderboard with numeric SOTA results (the existing biomedical README includes one; we defer this to a future enhancement)

## 4. Directory Structure

```
domains/recommendation/
├── README.md                           # Top-level: cross-paradigm tech tree, paradigm nav, datasets, metrics
├── cf-mf/                              # Collaborative Filtering & Matrix Factorization
│   ├── README.md                       # Paradigm tech tree + intro
│   ├── classic.md                      # Foundational works (1994-2015)
│   ├── 2016.md ... 2026.md             # Year files (created only if ≥5 papers that year; otherwise merged)
│   └── misc.md                         # (optional) Sparse years combined
├── deep-rec/                           # Deep Recommenders (feature interaction)
├── ctr-ranking/                        # CTR prediction & ranking
├── sequential-rec/                     # Sequential recommendation (long-term history)
├── session-rec/                        # Session-based recommendation (short anonymous)
├── graph-rec/                          # Graph-based recommendation
├── llm4rec/                            # LLM for recommendation
├── generative-rec/                     # Generative recommendation
├── debias-causal/                      # Debiasing / fairness / causal
└── rl-rec/                             # Reinforcement learning for recommendation
```

Each sub-paradigm directory mirrors the structure of `cf-mf/` above.

## 5. The 10 Sub-Paradigms

| # | Dir | Paradigm (EN) | Range | Key Papers |
|---|---|---|---|---|
| 1 | `cf-mf/` | Collaborative Filtering & Matrix Factorization | 1994-present | SVD++, BPR, FM, FFM, WRMF, eALS |
| 2 | `deep-rec/` | Deep Recommenders (Feature Interaction) | 2016-present | NCF, Wide&Deep, DeepFM, xDeepFM, AutoInt, DCN-V2, FiBiNET |
| 3 | `ctr-ranking/` | CTR Prediction & Ranking | 2016-present | DIN, DIEN, DSIN, DCN, MMoE, PLE, ESMM, DLRM, CAN |
| 4 | `sequential-rec/` | Sequential Recommendation | 2016-present | GRU4Rec, Caser, SASRec, BERT4Rec, TiSASRec, CL4SRec, DuoRec |
| 5 | `session-rec/` | Session-based Recommendation | 2016-present | NARM, STAMP, SR-GNN, GCE-GNN, FGNN |
| 6 | `graph-rec/` | Graph-based Recommendation | 2018-present | PinSage, NGCF, LightGCN, UltraGCN, SimGCL, XSimGCL |
| 7 | `llm4rec/` | LLM for Recommendation | 2023-present | P5, TALLRec, LlamaRec, RecGPT, E4SRec, BIGRec |
| 8 | `generative-rec/` | Generative Recommendation | 2023-present | TIGER, HSTU, GenRec, LC-Rec, COBRA |
| 9 | `debias-causal/` | Debiasing / Fairness / Causal | 2016-present | IPS, DR, PDA, MACR, CR, CausalRec |
| 10 | `rl-rec/` | RL for Recommendation | 2018-present | YouTube REINFORCE, SlateQ, M3Rec, EGPG |

## 6. Top-Level README (domains/recommendation/README.md)

Sections, in order:

1. **Title + description** — one-paragraph field overview
2. **Cross-paradigm Tech Tree** (mermaid) — a *simplified* graph showing only flagship representatives per paradigm and cross-paradigm influence edges (e.g., Transformer → SASRec → BERT4Rec; GCN → NGCF → LightGCN; LLM → P5 → TALLRec). Target 25-35 nodes, not 60+.
3. **Paradigm Guide** — color-badge table mapping each of the 10 paradigms to a short description
4. **Benchmark Datasets** — grouped by task:
   - General: MovieLens (100K/1M/10M/20M/25M), Amazon Reviews (Beauty/Sports/Toys/Books), Yelp, Gowalla
   - CTR: Criteo, Avazu, KuaiRand, KuaiSAR
   - Industrial: Taobao, Alibaba Ads, Tenrec
   - Sequential/Session: Diginetica, YooChoose, RetailRocket
   - News: MIND, Adressa
   - Graph/KG: Last.FM, Book-Crossing
5. **Evaluation Metrics** — HR@K, NDCG@K, MRR, Recall@K, AUC, GAUC, Coverage, Diversity, Novelty, Serendipity
6. **Contents** — links to 10 sub-paradigm READMEs

## 7. Sub-Paradigm README Template

Each of the 10 sub-paradigm READMEs follows:

1. **Title** — paradigm name
2. **Intro** — 2-3 sentence description, what problem it solves, what distinguishes it from sibling paradigms
3. **Tech Tree** (mermaid) — detailed intra-paradigm evolution, 10-25 nodes, color-coded by sub-branch (e.g., in sequential-rec: RNN-based / Transformer-based / Contrastive / Diffusion)
4. **Sub-branch Legend** — color mapping
5. **Representative Datasets** — only if paradigm-specific (otherwise "see top-level README")
6. **Contents** — `classic.md`, year files in reverse chronological order

## 8. Year File Format

Each year file follows the format established by existing domains:

```markdown
# YYYY Recommendation — <Paradigm> Papers

## <Optional sub-section, e.g., "Transformer-based">

### Paper Title
- **Authors:** ...
- **Venue:** SIGIR 2024
- **Paper:** [arXiv](...) / [Proceedings](...)
- **Code:** [GitHub](...)
- **Summary:** 1-2 sentences on contribution
- **Tags:** `#sequential` `#contrastive`
```

Papers within a year are grouped by sub-branch where useful, otherwise listed flat by venue.

## 9. classic.md Files

Each `classic.md` captures foundational pre-2016 works for that paradigm. Examples:

- `cf-mf/classic.md`: Item-based CF (2001), Netflix Prize SVD (2007), SVD++ (2008), BPR (2009), FM (2010), eALS (2014)
- `sequential-rec/classic.md`: Markov Chain recommenders, FPMC (2010), HRM (2015)
- `rl-rec/classic.md`: contextual bandits for recommendation (LinUCB 2010, Thompson sampling)

If a paradigm has no meaningful pre-2016 work (e.g., LLM4Rec, Generative-Rec), `classic.md` lists the 2-3 seminal papers that launched the paradigm instead, or is omitted with a note in the sub-README.

## 10. Top-level Repo README Update

Add a new row to the Domain Directions table in the root `README.md`:

| Domain | Description |
|--------|-------------|
| [Recommendation Systems](domains/recommendation/) | Collaborative filtering, CTR prediction, sequential/session/graph/LLM-based/generative recommendation |

## 11. Rollout Plan (Preview — full plan deferred to writing-plans)

Because this touches ~60-80 files, the implementation will proceed in waves:

1. **Scaffolding wave** — create top-level README, 10 sub-directory READMEs with tech trees, paradigm legends
2. **Classic wave** — all `classic.md` files
3. **Paradigm waves** (10 × 1) — for each paradigm, create year files in reverse-chronological order (2026 → 2016)
4. **Polish wave** — cross-link fixes, top-level tech-tree refinement, root README update, index consistency check

Per-paradigm commit granularity: one commit per paradigm directory (all its year files + README) keeps history readable.

## 12. Success Criteria

- All 10 sub-paradigm directories exist with populated README + classic.md
- Each paradigm has year files for 2023-2026 at minimum (active years)
- Top-level README links to all 10 paradigms and renders the cross-paradigm mermaid diagram without errors
- Root `README.md` includes a row for the new domain
- Every paper entry has: authors, venue, paper link, summary (code link optional but strongly preferred)
- Repo passes existing structural conventions (checked by comparison with `domains/graph/` and `domains/nlp/`)

## 13. Non-Goals / Future Work

- SOTA leaderboard with numeric results (see biomedical example) — can be added later
- Chinese-language version of READMEs
- Integration with `techniques/` cross-links (e.g., Transformer → Sequential-Rec) — noted in text but no automated cross-index
- Multimodal-Rec, ConvRec, Cold-start as standalone paradigms
