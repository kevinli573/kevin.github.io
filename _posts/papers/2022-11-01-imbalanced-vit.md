---
layout: paper
categories: papers
permalink: papers/imbalanced-vit
id: imbalanced-vit
title: "Evaluating Robustness of Vision Transformers on Imbalanced Datasets"
authors: 
  - Kevin Li
  - Rahul Duggal
  - Duen Horng Chau
venue: "Association for the Advancement of Artificial Intelligence"
venue-shorthand: AAAI
location: Washington DC, USA
year: 2023
url: /papers/imbalanced-vit
# pdf: /papers/21-argo-scholar-poster.pdf
# poster: /assets/argo_scholar_poster.pdf
# code: https://github.com/poloclub/argo-scholar
# award: Best Poster, Honorable Mention
type: poster
# figure: /images/papers/21-argo-scholar.png
# doi: "10.48550/arXiv.2110.14060"

# highlight:
selected: true
featured: true
feature-order: 1
feature-title: Vision Transformer Robustness
feature-description: Evaluating Robustness of Vision Transformers on Imbalanced Datasets
image: /images/papers/coming-soon.png
coming-soon: true

# bibtex: |-

#   @article{Li2021ArgoSI,
#     title={Argo Scholar: Interactive Visual Exploration of Literature in Browsers},
#     author={Kevin Li and H. Yang and Anish Upadhayay and Zhiyan Zhou and Jon Saad-Falcon and Duen Horng Chau},
#     journal={ArXiv},
#     year={2021},
#     volume={abs/2110.14060
#   }
---

Data in the real world is commonly imbalanced across classes. Training neural networks on imbalanced datasets often leads to poor performance on rare classes. Existing work in this area has primarily focused on Convolution Neural Networks (CNN), which are increasingly being replaced by Self-Attention-based Vision Transformers (ViT). Fundamentally, ViTs differ from CNNs in that they offer the flexibility in learning the appropriate inductive bias conducive to improving performance. This work is among the first to evaluate the performance of ViTs under class imbalance. We find that accuracy degradation in the presence of class imbalance is much more prominent in ViTs compared to CNNs. This degradation can be partially mitigated through loss reweighting - a popular strategy that increases the loss contributed by rare classes. We investigate the impact of loss reweighting on different components of a ViT, namely, the patch embedding, self-attention backbone, and linear classifier. Our ongoing investigations reveal that loss reweighting impacts mostly the linear classifier and self-attention backbone while having a small and negligible effect on the embedding layer.