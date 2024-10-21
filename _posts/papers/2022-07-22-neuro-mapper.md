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
pdf: /papers/22-vis-neuromapper.pdf
poster: /assets/22-vis-neuromapper-poster.pdf
code: https://github.com/poloclub/NeuroMapper
type: poster
figure: /images/papers/22-neuromapper.png

# highlight:
selected: false
featured: false
# feature-order: 3
feature-title: NeuroMapper
feature-description: In-browser Visualization of Neural Network Training
# image: /images/papers/22-neuromapper.png

bibtex: |-

  @article{Zhou2022NeuroMapperIV,
    title={NeuroMapper: In-browser Visualizer for Neural Network Training},
    author={Zhiyan Zhou and Kevin Li and Haekyu Park and Megan Dass and Austin P. Wright and Nilaksh Das and Duen Horng Chau},
    journal={ArXiv},
    year={2022},
    volume={abs/2210.12492}
  }
---

We present our ongoing work NeuroMapper, an in-browser visualization tool that helps machine learning (ML) developers interpret the evolution of a model during training, providing a new way to monitor the training process and visually discover reasons for suboptimal training. While most existing deep neural networks (DNNs) interpretation tools are designed for already-trained model, NeuroMapper scalably visualizes the evolution of the embeddings of a model's blocks across training epochs, enabling real-time visualization of 40,000 embedded points. To promote the embedding visualizations’ spatial coherence across epochs, NeuroMapper adapts AlignedUMAP, a recent nonlinear dimensionality reduction technique to align the embeddings. With NeuroMapper, users can explore the training dynamics of a Resnet-50 model, and adjust the embedding visualizations' parameters in real time. NeuroMapper is open-sourced at https://github.com/poloclub/NeuroMapper and runs in all modern web browsers. A demo of the tool in action is available at: https://poloclub.github.io/NeuroMapper/.
