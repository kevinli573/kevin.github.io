---
layout: paper
categories: papers
permalink: papers/argo-scholar-demo
id: argo-scholar-demo
title: "Visual Exploration of Literature with Argo Scholar"
authors: 
  - Kevin Li
  - Haoyang Yang
  - Evan Montoya
  - Anish Upadhayay
  - Zhiyan Zhou
  - Jon Saad-Falcon
  - Duen Horng Chau
venue: "ACM International Conference on Information and Knowledge Management"
venue-shorthand: CIKM
location: Atlanta, GA
year: 2022
url: /papers/argo-scholar-demo
pdf: /papers/22-cikm-argo-scholar.pdf
poster: /assets/22-cikm-argoscholar-poster.pdf
code: https://github.com/poloclub/argo-scholar
type: demo
figure: /images/papers/22-argo-scholar.png
doi: "10.1145/3511808.3557177"

# highlight:
selected: false
featured: false
# feature-order: 2
# feature-title: Argo Scholar
# feature-description: Visual Exploration of Literature with Argo Scholar
# image: /images/papers/22-argo-scholar.png

bibtex: |-

  @inproceedings{li2022argoscholar, 
    author = {Li, Kevin and Yang, Haoyang and Montoya, Evan and Upadhayay, Anish and Zhou, Zhiyan and Saad-Falcon, Jon and Chau, Duen Horng},
    title = {Visual Exploration of Literature with Argo Scholar},
    year = {2022},
    isbn = {9781450392365},
    publisher = {Association for Computing Machinery},
    url = {https://doi.org/10.1145/3511808.3557177},
    doi = {10.1145/3511808.3557177}
  }
---

Discovering and making sense of relevant literature is fundamental in any scientific field. Visualization can aid this process; however, existing tools’ adoption and impact are often constrained, such as by their reliance on small, curated paper datasets that quickly become outdated or a lack of support for personalized exploration. We introduce Argo Scholar, an open-source visualization tool designed for interactive exploration of literature and easy sharing of exploration results. Argo Scholar is tightly integrated with Semantic Scholar’s live data of over 200 million papers, enabling users to generate personalized literature exploration results in real-time through flexible, incremental exploration, a common and effective method for researchers to discover relevant work. A large-scale user study of 122 participants from diverse backgrounds and experiences showed that Argo Scholar is effective at helping users find related work and understand paper connections, and incremental graph-based exploration is effective across diverse disciplines. Developed using modern web technologies, our tool is widely available at https://poloclub.github.io/argo-scholar and allows users to easily share their literature search results as a URL.