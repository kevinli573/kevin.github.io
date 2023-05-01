---
layout: paper
categories: papers
permalink: papers/robust-arch
id: robust-arch
title: "RobArch: Designing Robust Architectures against Adversarial Attacks"
authors: 
  - ShengYun Peng
  - Weilin Xu
  - Cory Cornelius
  - Kevin Li
  - Rahul Duggal
  - Duen Horng Chau
  - Jason Martin
venue: "arXiv:2301.03110"
venue-shorthand: Arxiv
# location: Washington DC, USA
year: 2023
url: /papers/robust-arch
# pdf: /papers/21-argo-scholar-poster.pdf
# poster: /assets/argo_scholar_poster.pdf
code: https://github.com/ShengYun-Peng/RobArch
# award: Best Poster, Honorable Mention
type: preprint
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

  @article{Peng2023RobArchDR,
    title={RobArch: Designing Robust Architectures against Adversarial Attacks},
    author={Sheng-Hsuan Peng and Weilin Xu and Cory Cornelius and Kevin Li and Rahul Duggal and Duen Horng Chau and Jason Martin},
    journal={ArXiv},
    year={2023},
    volume={abs/2301.03110}
  }
---

Adversarial Training is the most effective approach for improving the robustness of Deep Neural Networks (DNNs). However, compared to the large body of research in optimizing the adversarial training process, there are few investigations into how architecture components affect robustness, and they rarely constrain model capacity. Thus, it is unclear where robustness precisely comes from. In this work, we present the first large-scale systematic study on the robustness of DNN architecture components under fixed parameter budgets. Through our investigation, we distill 18 actionable robust network design guidelines that empower model developers to gain deep insights. We demonstrate these guidelines' effectiveness by introducing the novel Robust Architecture (RobArch) model that instantiates the guidelines to build a family of top-performing models across parameter capacities against strong adversarial attacks. RobArch achieves the new state-of-the-art AutoAttack accuracy on the RobustBench ImageNet leaderboard. The code is available at https://github.com/ShengYun-Peng/RobArch.
