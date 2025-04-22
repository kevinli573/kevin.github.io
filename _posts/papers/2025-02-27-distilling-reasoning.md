---
layout: paper
categories: papers
permalink: papers/distilling-reasoning
id: distilling-reasoning
title: "Thinking Slow, Fast: Scaling Inference Compute with Distilled Reasoners"
authors: 
  - Daniele Paliotta*
  - Junxiong Wang*
  - Matteo Pagliardini*
  - Kevin Y. Li*
  - Aviv Bick
  - J. Zico Kolter
  - Albert Gu
  - François Fleuret
  - Tri Dao
venue: arXiv
# venue-shorthand: 
# location: 
year: 2025
url: /papers/distilling-reasoning
pdf: https://arxiv.org/abs/2502.20339
# code: https://github.com/locuslab/llava-token-compression
type: preprint
# figure: /images/papers/21-argo-scholar.png
# doi: "10.48550/arXiv.2110.14060"

# highlight:
selected: false
featured: false
feature-order: 0
# feature-title: 'VLM Inference Scaling Laws'
# feature-description: Scaling laws for VLM inference for balancing image token count and LLM size.
# image: /images/papers/coming-soon.png
# coming-soon: true

bibtex: |-

  @misc{paliotta2025thinkingslowfastscaling,
      title={Thinking Slow, Fast: Scaling Inference Compute with Distilled Reasoners}, 
      author={Daniele Paliotta and Junxiong Wang and Matteo Pagliardini and Kevin Y. Li and Aviv Bick and J. Zico Kolter and Albert Gu and François Fleuret and Tri Dao},
      year={2025},
      eprint={2502.20339},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2502.20339}, 
    }
---

Recent advancements have demonstrated that the performance of large language models (LLMs) can be significantly enhanced by scaling computational resources at test time. A common strategy involves generating multiple Chain-of-Thought (CoT) trajectories and aggregating their outputs through various selection mechanisms. This raises a fundamental question: can models with lower complexity leverage their superior generation throughput to outperform similarly sized Transformers for a fixed computational budget? To address this question and overcome the lack of strong subquadratic reasoners, we distill pure and hybrid Mamba models from pretrained Transformers. Trained on only 8 billion tokens, our distilled models show strong performance and scaling on mathematical reasoning datasets while being much faster at inference for large batches and long sequences. Despite the zero-shot performance hit due to distillation, both pure and hybrid Mamba models can scale their coverage and accuracy performance past their Transformer teacher models under fixed time budgets, opening a new direction for scaling inference compute.