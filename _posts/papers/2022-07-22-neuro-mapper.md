---
layout: paper
categories: papers
permalink: papers/neuromapper
id: neuro-mapper
title: "NeuroMapper: In-browser Visualizer for Neural Network Training"
authors: 
  - Zhiyan Zhou
  - Kevin Li
  - Haekyu Park
  - Megan Dass
  - Austin Wright
  - Nilaksh Das
  - Duen Horng Chau
venue: "IEEE VIS: Visualization & Visual Analytics"
venue-shorthand: IEEE VIS
location: Oklahoma City, OK
year: 2022
url: /papers/neuromapper
# pdf: /papers/21-argo-scholar-poster.pdf
# poster: /assets/argo_scholar_poster.pdf
code: https://github.com/poloclub/NeuroMapper
# award: Best Poster, Honorable Mention
type: poster
figure: /images/papers/22-neuromapper.png
# doi: "10.48550/arXiv.2110.14060"

# highlight:
selected: true
featured: true
feature-order: 2
feature-title: NeuroMapper
feature-description: In-browser Visualization of Neural Network Training
image: /images/papers/22-neuromapper.png
coming-soon: True

# bibtex: |-

#   @article{Li2021ArgoSI,
#     title={Argo Scholar: Interactive Visual Exploration of Literature in Browsers},
#     author={Kevin Li and H. Yang and Anish Upadhayay and Zhiyan Zhou and Jon Saad-Falcon and Duen Horng Chau},
#     journal={ArXiv},
#     year={2021},
#     volume={abs/2110.14060
#   }
---

We present our ongoing work NeuroMapper, an in-browser visualization tool that helps machine learning (ML) developers interpret the evolution of a model during training, providing a new way to monitor the training process and visually discover reasons for suboptimal training. While most existing deep neural networks (DNNs) interpretation tools are designed for already-trained model, NeuroMapper scalably visualizes the evolution of the embeddings of a model's blocks across training epochs, enabling real-time visualization of 40,000 embedded points. To promote the embedding visualizations’ spatial coherence across epochs, NeuroMapper adapts AlignedUMAP, a recent nonlinear dimensionality reduction technique to align the embeddings. With NeuroMapper, users can explore the training dynamics of a Resnet-50 model, and adjust the embedding visualizations' parameters in real time. NeuroMapper is open-sourced at https://github.com/poloclub/NeuroMapper and runs in all modern web browsers. A demo of the tool in action is available at: https://poloclub.github.io/NeuroMapper/.
