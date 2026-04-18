# Classic — Deep Recommenders

> This paradigm is post-2015; 'classic' works are the 2016-2017 papers that defined it.

Foundational works that launched the deep recommender era, replacing hand-crafted feature engineering with learned deep feature interactions.

#### Launch Era 2016-2017

### Neural Collaborative Filtering
- **Authors:** He et al.
- **Venue:** WWW 2017
- **Paper:** [ArXiv](https://arxiv.org/abs/1708.05031)
- **Code:** [GitHub](https://github.com/hexiangnan/neural_collaborative_filtering)
- **Summary:** Replaces inner-product CF with MLP over user/item embeddings, enabling non-linear interaction modeling for collaborative filtering.
- **Tags:** `#ncf` `#mlp`

### Wide & Deep Learning for Recommender Systems
- **Authors:** Cheng et al.
- **Venue:** DLRS 2016
- **Paper:** [ArXiv](https://arxiv.org/abs/1606.07792)
- **Summary:** Joint linear (memorization) and deep (generalization) training; launched deep-rec era. Deployed at Google Play with significant production impact.
- **Tags:** `#wide-deep` `#seminal`

### DeepFM: A Factorization-Machine based Neural Network for CTR Prediction
- **Authors:** Guo et al.
- **Venue:** IJCAI 2017
- **Paper:** [ArXiv](https://arxiv.org/abs/1703.04247)
- **Code:** [GitHub](https://github.com/ChenglongChen/tensorflow-DeepFM)
- **Summary:** End-to-end FM + DNN on shared embedding; eliminated manual feature engineering while capturing both low- and high-order feature interactions.
- **Tags:** `#deepfm` `#fm` `#seminal`

### Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features
- **Authors:** Shan et al.
- **Venue:** KDD 2016
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/2939672.2939704)
- **Summary:** Residual network for ad click prediction; early deep CTR model demonstrating automatic combinatorial feature learning without manual engineering.
- **Tags:** `#residual` `#early-deep`
