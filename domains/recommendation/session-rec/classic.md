# Classic — Session-based Recommendation

> GRU4Rec (2016) also appears in sequential-rec/classic.md — both paradigms claim it as foundational.

Foundational works (2016–2017) that established session-based recommendation as a distinct paradigm, moving from pure RNN to attention-augmented session modeling.

#### Launch Era

### Session-based Recommendations with Recurrent Neural Networks
- **Authors:** Hidasi et al.
- **Venue:** ICLR 2016
- **Paper:** [ArXiv](https://arxiv.org/abs/1511.06939)
- **Code:** [GitHub](https://github.com/hidasib/GRU4Rec)
- **Summary:** GRU4Rec applies gated recurrent units to model click sequences within sessions, introducing session-based recommendation as a distinct research problem with scalable training via session-parallel mini-batches.
- **Tags:** `#gru4rec` `#seminal`

### Item2Vec: Neural Item Embedding for Collaborative Filtering
- **Authors:** Barkan & Koenigstein
- **Venue:** RecSys 2016
- **Paper:** [ArXiv](https://arxiv.org/abs/1603.04259)
- **Summary:** Applies word2vec skip-gram to item sequences for learning item embeddings from session co-occurrence, providing a simple but effective foundation for session-aware item similarity.
- **Tags:** `#item2vec` `#embedding`

### Personalizing Session-based Recommendations with Hierarchical Recurrent Neural Networks
- **Authors:** Quadrana et al.
- **Venue:** RecSys 2017
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/3109859.3109896)
- **Code:** [GitHub](https://github.com/mquad/hgru4rec)
- **Summary:** HRNN introduces cross-session user modeling by propagating hidden state across sessions through a hierarchical RNN, bridging session-based and sequential recommendation.
- **Tags:** `#hrnn` `#session`
