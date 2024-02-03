---
layout: paper
categories: papers
permalink: papers/concept-evo
id: concept-evo
title: "Concept Evolution in Deep Learning Training: A Unified Interpretation Framework and Discoveries"
authors: 
  - Haekyu Park
  - Seongmin Lee
  - Benjamin Hoover
  - Austin P. Wright
  - Omar Shaikh
  - Rahul Duggal
  - Nilaksh Das
  - Kevin Li
  - Judy Hoffman
  - Duen Horng Chau
venue: "ACM International Conference on Information and Knowledge Management"
venue-shorthand: CIKM
location: Birmingham, UK
year: 2023
url: /papers/concept-evo
pdf: /papers/23-cikm-conceptevo.pdf
# poster: /assets/argo_scholar_poster.pdf
code: https://github.com/poloclub/ConceptEvo
# award: Best Poster, Honorable Mention
type: conference
# figure: /images/papers/21-argo-scholar.png
# doi: "10.48550/arXiv.2110.14060"

# highlight:
selected: false
featured: false
# feature-order: 1
# feature-title: Vision Transformer Robustness
# feature-description: Evaluating Robustness of Vision Transformers on Imbalanced Datasets
# image: /images/papers/coming-soon.png
# coming-soon: true

bibtex: |-

  @article{Haekyu2023ConceptEvo,
    title = {Concept Evolution in Deep Learning Training: A Unified Interpretation Framework and Discoveries},
    author = {Park, Haekyu and Lee, Seongmin and Hoover, Benjamin and Wright, Austin P. and Shaikh, Omar and Duggal, Rahul and Das, Nilaksh and Li, Kevin and Hoffman, Judy and Chau, Duen Horng},
    journal={ArXiv},
    year = {2023},
    volume={abs/2301.03110}.
    isbn = {9798400701245},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    url = {https://doi.org/10.1145/3583780.3614819},
    doi = {10.1145/3583780.3614819},
    booktitle = {Proceedings of the 32nd ACM International Conference on Information and Knowledge Management},
    pages = {2044–2054},
    series = {CIKM '23}
  }
---

We present ConceptEvo, a unified interpretation framework for deep neural networks (DNNs) that reveals the inception and evolution of learned concepts during training. Our work addresses a critical gap in DNN interpretation research, as existing methods primarily focus on post-training interpretation. ConceptEvo introduces two novel technical contributions: (1) an algorithm that generates a unified semantic space, enabling side-by-side comparison of different models during training, and (2) an algorithm that discovers and quantifies important concept evolutions for class predictions. Through a large-scale human evaluation and quantitative experiments, we demonstrate that ConceptEvo successfully identifies concept evolutions across different models, which are not only comprehensible to humans but also crucial for class predictions. ConceptEvo is applicable to both modern DNN architectures, such as ConvNeXt, and classic DNNs, such as VGGs and InceptionV3.