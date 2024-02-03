---
layout: paper
categories: papers
permalink: papers/robust-arch
id: robust-arch
title: "Robust Principles: Architectural Design Principles for Adversarially Robust CNNs"
authors: 
  - ShengYun Peng
  - Weilin Xu
  - Cory Cornelius
  - Matthew Hull
  - Kevin Li
  - Rahul Duggal
  - Duen Horng Chau
  - Jason Martin
venue: "British Machine Vision Conference"
venue-shorthand: BMVC
location: Aberdeen, UK
year: 2023
url: /papers/robust-arch
pdf: /papers/23-bmvc-robarch.pdf
# poster: /assets/argo_scholar_poster.pdf
code: https://github.com/poloclub/robust-principles
award: Best Poster
type: conference
# figure: /images/papers/21-argo-scholar.png
# doi: "10.48550/arXiv.2110.14060"

# highlight:
selected: true
featured: true
feature-order: 0
feature-title: Designing Adversarially Robust Architectures
feature-description: A suite of generalizable robust architectural design principles
# image: /images/papers/coming-soon.png
# coming-soon: false

bibtex: |-

  @inproceedings{Peng_2023_BMVC,
    author    = {ShengYun Peng and Weilin Xu and Cory Cornelius and Matthew Hull and Kevin Li and Rahul Duggal and Mansi Phute and Jason Martin and Duen Horng Chau},
    title     = {Robust Principles: Architectural Design Principles for Adversarially Robust CNNs},
    booktitle = {34th British Machine Vision Conference 2023, {BMVC} 2023, Aberdeen, UK, November 20-24, 2023},
    publisher = {BMVA},
    year      = {2023},
    url       = {https://papers.bmvc2023.org/0739.pdf}
  }
---

We aim to unify existing works’ diverging opinions on how architectural components affect the adversarial robustness of CNNs. To achieve our goal, we synthesize a suite of generalizable robust architectural design principles: (a) optimal range for depth and width configurations, (b) preferring convolutional over patchify stem stage, and (c) robust residual block design by adopting squeeze and excitation blocks, and non-parametric smooth activation functions. Through extensive experiments across a wide spectrum of dataset scales, adversarial training methods, model parameters, and network design spaces, our principles consistently and markedly improve AutoAttack accuracy: 1–3 percentage points (pp) on CIFAR-10 and CIFAR-100, and 4–9 pp on ImageNet. The code is publicly available at https://github.com/poloclub/robust-principles.
