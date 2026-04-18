# Classic — CTR Prediction & Ranking

Foundational works (2016–2018) that established user-interest modeling, two-tower retrieval, and multi-task learning as pillars of industrial ranking systems.

#### Launch Era

### Deep Neural Networks for YouTube Recommendations
- **Authors:** Covington et al.
- **Venue:** RecSys 2016
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/2959100.2959190)
- **Summary:** Two-stage (candidate generation + ranking) deep learning system deployed at YouTube scale. Established the blueprint for industrial recommender architectures.
- **Tags:** `#youtube` `#two-tower` `#industrial` `#seminal`

### Deep Interest Network for CTR Prediction
- **Authors:** Zhou et al.
- **Venue:** KDD 2018
- **Paper:** [ArXiv](https://arxiv.org/abs/1706.06978)
- **Code:** [GitHub](https://github.com/zhougr1993/DeepInterestNetwork)
- **Summary:** Attention mechanism that adaptively weights historical behaviors relative to the target item, capturing diverse user interests for CTR prediction at Alibaba.
- **Tags:** `#din` `#attention` `#seminal`

### Deep & Cross Network for Ad Click Predictions
- **Authors:** Wang et al.
- **Venue:** ADKDD 2017
- **Paper:** [ArXiv](https://arxiv.org/abs/1708.05123)
- **Summary:** Introduces an explicit cross network that automatically learns bounded-degree feature interactions, combined with a DNN for high-order learning; deployed at Google.
- **Tags:** `#dcn` `#cross-network`

#### Multi-task Foundations

### Entire Space Multi-task Model: An Effective Approach for Estimating Post-Click Conversion Rate
- **Authors:** Ma et al.
- **Venue:** SIGIR 2018
- **Paper:** [ArXiv](https://arxiv.org/abs/1804.07931)
- **Summary:** Models CTR and CVR jointly across the entire sample space using multi-task learning to avoid selection bias in conversion prediction at Alibaba.
- **Tags:** `#esmm` `#multi-task` `#conversion`

### Modeling Task Relationships in Multi-task Learning with Multi-gate Mixture-of-Experts
- **Authors:** Ma et al.
- **Venue:** KDD 2018
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/3219819.3220007)
- **Summary:** MMoE uses multiple expert sub-networks with learned gating to enable flexible task-specific parameter sharing, outperforming hard-sharing baselines across diverse task relationships.
- **Tags:** `#mmoe` `#multi-task` `#seminal`

### Product-based Neural Networks for User Response Prediction
- **Authors:** Qu et al.
- **Venue:** ICDM 2016
- **Paper:** [ArXiv](https://arxiv.org/abs/1611.00144)
- **Code:** [GitHub](https://github.com/Atomu2014/product-nets)
- **Summary:** Introduces inner and outer product layers for capturing feature interactions in CTR prediction; early deep model bridging FM and fully connected networks.
- **Tags:** `#pnn` `#early-ctr`
