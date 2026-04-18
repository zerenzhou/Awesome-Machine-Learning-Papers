# Classic — Graph-based Recommendation

> The GNN foundations (GCN, GraphSAGE, GAT) are in `domains/graph/classic.md`.

Foundational works (2018–2019) that established GNN-based recommendation on user-item bipartite graphs, moving from random-walk and spectral methods to scalable message-passing frameworks.

#### Launch Era

### Graph Convolutional Neural Networks for Web-Scale Recommender Systems
- **Authors:** Ying et al.
- **Venue:** KDD 2018
- **Paper:** [ArXiv](https://arxiv.org/abs/1806.01973)
- **Summary:** PinSage applies GraphSAGE-style random-walk sampling and convolutional aggregation to Pinterest's billion-node user-item graph, establishing the blueprint for industrial GNN-based recommendation.
- **Tags:** `#pinsage` `#industrial` `#seminal`

### Graph Convolutional Matrix Completion
- **Authors:** van den Berg et al.
- **Venue:** KDD Workshop 2018
- **Paper:** [ArXiv](https://arxiv.org/abs/1706.02263)
- **Code:** [GitHub](https://github.com/riannevdberg/gc-mc)
- **Summary:** GC-MC formulates collaborative filtering as link prediction on a bipartite user-item graph and applies graph auto-encoders for matrix completion, connecting GNN research to recommender systems.
- **Tags:** `#gc-mc` `#matrix-completion`

### Neural Graph Collaborative Filtering
- **Authors:** Wang et al.
- **Venue:** SIGIR 2019
- **Paper:** [ArXiv](https://arxiv.org/abs/1905.08108)
- **Code:** [GitHub](https://github.com/xiangwang1223/neural_graph_collaborative_filtering)
- **Summary:** NGCF propagates embeddings over the user-item interaction graph via multi-layer graph convolution, explicitly capturing high-order connectivity and collaborative signals.
- **Tags:** `#ngcf` `#bipartite`
