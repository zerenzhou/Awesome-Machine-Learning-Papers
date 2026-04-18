# Classic — LLM for Recommendation

> This paradigm began in late 2022. All 'classic' works are from 2022-2023.

Foundational works that established LLMs as first-class components of recommender systems, from unified prompting frameworks to zero-shot evaluation of frontier models.

#### Paradigm Launch (2022-2023)

### Recommendation as Language Processing: A Unified Pretrain, Personalized Prompt & Predict Paradigm
- **Authors:** Geng et al.
- **Venue:** RecSys 2022
- **Paper:** [ArXiv](https://arxiv.org/abs/2203.13366)
- **Code:** [GitHub](https://github.com/jeykigung/P5)
- **Summary:** P5 frames five recommendation tasks (rating, retrieval, explanation, review, conversation) as text-to-text generation using a shared T5 backbone with personalized prompts, launching the unified LLM-for-rec paradigm.
- **Tags:** `#p5` `#unified-prompt` `#seminal`

### M6-Rec: Generative Pretrained Language Models are Open-Ended Recommender Systems
- **Authors:** Cui et al.
- **Venue:** arXiv 2022
- **Paper:** [ArXiv](https://arxiv.org/abs/2205.08084)
- **Summary:** Adapts Alibaba's M6 large language model to open-ended recommendation via prompt engineering and fine-tuning, demonstrating that generative LLMs can serve as recommenders across diverse item domains.
- **Tags:** `#m6` `#generative`

### Is ChatGPT a Good Recommender? A Preliminary Study
- **Authors:** Liu et al.
- **Venue:** arXiv 2023
- **Paper:** [ArXiv](https://arxiv.org/abs/2304.10149)
- **Summary:** Systematically evaluates ChatGPT as a zero-shot recommender across five recommendation tasks, revealing strengths in cold-start scenarios and limitations in collaborative signal exploitation relative to fine-tuned models.
- **Tags:** `#chatgpt` `#zero-shot` `#evaluation`
