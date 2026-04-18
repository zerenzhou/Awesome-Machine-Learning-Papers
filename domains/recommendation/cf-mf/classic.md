# Classic — Collaborative Filtering & Matrix Factorization

Foundational works (1994–2015) that defined collaborative filtering and matrix factorization. Later deep-learning era papers are in the year files.

## Neighborhood Methods

### GroupLens: An Open Architecture for Collaborative Filtering of Netnews
- **Authors:** Resnick et al.
- **Venue:** CSCW 1994
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/192844.192905)
- **Summary:** Pioneering work introducing user-based collaborative filtering. Proposed using user-user similarity to predict ratings for unrated items. Foundational to modern CF-based recommenders.
- **Tags:** `#user-cf` `#seminal`

### Item-based Collaborative Filtering Recommendation Algorithms
- **Authors:** Sarwar et al.
- **Venue:** WWW 2001
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/371920.372071)
- **Summary:** Introduced item-item similarity-based collaborative filtering. Demonstrated superior scalability and performance compared to user-based CF, particularly for large-scale systems.
- **Tags:** `#item-cf` `#seminal`

### Amazon.com Recommendations: Item-to-Item Collaborative Filtering
- **Authors:** Linden et al.
- **Venue:** IEEE Internet Computing 2003
- **Paper:** [IEEE Xplore](https://ieeexplore.ieee.org/document/1167344)
- **Summary:** Describes the production-scale item-item collaborative filtering system deployed at Amazon. Real-world validation of CF scalability and effectiveness in large e-commerce settings.
- **Tags:** `#item-cf` `#industrial`

### Slope One Predictors for Online Rating-Based Collaborative Filtering
- **Authors:** Lemire & Maclachlan
- **Venue:** SDM 2005
- **Paper:** [ArXiv](https://arxiv.org/abs/cs/0702046)
- **Summary:** Proposes simple yet effective slope-one predictors for CF, using item-pair rating differences. Offers computational simplicity and competitive accuracy.
- **Tags:** `#rating-predictor`

## Latent Factor Models

### Factorization Meets the Neighborhood: a Multifaceted Collaborative Filtering Model
- **Authors:** Koren, Yehuda
- **Venue:** KDD 2008
- **Paper:** [ACM Digital Library](https://dl.acm.org/doi/10.1145/1401890.1401944)
- **Summary:** Introduces SVD++ which combines latent factor models with neighborhood information. Achieved top performance in Netflix Prize competition through joint optimization of user/item factors and implicit feedback.
- **Tags:** `#svdpp` `#implicit-feedback`

### Matrix Factorization Techniques for Recommender Systems
- **Authors:** Koren, Bell, Volinsky
- **Venue:** IEEE Computer 2009
- **Paper:** [IEEE Computer Magazine](https://ieeexplore.ieee.org/document/5197422)
- **Summary:** Canonical comprehensive review of matrix factorization for recommendation. Covers biased MF, temporal dynamics, and damping. Essential reference from Netflix Prize.
- **Tags:** `#mf` `#netflix-prize` `#seminal`

## Ranking-aware Implicit Feedback

### BPR: Bayesian Personalized Ranking from Implicit Feedback
- **Authors:** Rendle et al.
- **Venue:** UAI 2009
- **Paper:** [ArXiv](https://arxiv.org/abs/1205.2618)
- **Summary:** Proposes BPR, a pairwise ranking loss for learning from implicit feedback. Addresses the asymmetry between positive and unobserved interactions, outperforming pointwise losses. Fundamental to modern implicit feedback recommendation.
- **Tags:** `#bpr` `#pairwise-ranking` `#seminal`

### Collaborative Filtering for Implicit Feedback Datasets
- **Authors:** Hu, Koren, Volinsky
- **Venue:** ICDM 2008
- **Paper:** [IEEE Xplore](https://ieeexplore.ieee.org/document/4781145)
- **Summary:** Introduces alternating least squares (ALS) and weighted regression (WRMF) for implicit feedback. Treats all unobserved interactions as negative examples with confidence weighting.
- **Tags:** `#ials` `#wrmf` `#implicit-feedback`

### Fast Matrix Factorization for Online Recommendation with Implicit Feedback
- **Authors:** He et al.
- **Venue:** SIGIR 2016
- **Paper:** [ArXiv](https://arxiv.org/abs/1603.02820)
- **Summary:** Proposes eALS (efficient ALS) with coordinate descent optimization for fast implicit MF training. Enables efficient large-scale implicit feedback recommendation.
- **Tags:** `#eals` `#implicit-feedback`

## Factorization Machines

### Factorization Machines
- **Authors:** Rendle, Steffen
- **Venue:** ICDM 2010
- **Paper:** [IEEE Xplore](https://ieeexplore.ieee.org/document/5694074)
- **Summary:** Introduces factorization machines, a general framework generalizing MF to arbitrary feature interactions. Bridges traditional CF and feature-based learning; foundation for modern deep recommenders (DeepFM, xDeepFM).
- **Tags:** `#fm` `#feature-interaction` `#seminal`
