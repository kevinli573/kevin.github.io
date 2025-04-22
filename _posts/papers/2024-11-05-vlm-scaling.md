---
layout: paper
categories: papers
permalink: papers/vlm-scaling
id: vlm-scaling
title: "Inference Optimal VLMs Need Fewer Visual Tokens and More Parameters"
authors: 
  - Kevin Y. Li*
  - Sachin Goyal*
  - Joao D. Semedo
  - J. Zico Kolter
venue: "International Conference on Learning Representations"
venue-shorthand: ICLR
location: Singapore
year: 2025
url: /papers/vlm-scaling
pdf: https://arxiv.org/abs/2411.03312
code: https://github.com/locuslab/llava-token-compression
type: conference
# figure: /images/papers/21-argo-scholar.png
# doi: "10.48550/arXiv.2110.14060"

# highlight:
selected: true
featured: true
feature-order: 0
feature-title: 'VLM Inference Scaling Laws'
feature-description: Scaling laws for VLM inference for balancing image token count and LLM size.
# image: /images/papers/coming-soon.png
# coming-soon: true

bibtex: |-

  @misc{li2025inferenceoptimalvlmsneed,
      title={Inference Optimal VLMs Need Fewer Visual Tokens and More Parameters}, 
      author={Kevin Y. Li and Sachin Goyal and Joao D. Semedo and J. Zico Kolter},
      year={2025},
      eprint={2411.03312},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2411.03312}, 
    }
---

Vision Language Models (VLMs) have demonstrated strong capabilities across various visual understanding and reasoning tasks, driven by incorporating image representations into the token inputs of Large Language Models (LLMs). However, their real-world deployment is often constrained by high latency during inference due to the substantial compute required by the LLM to process the large number of input tokens, predominantly arising from the image. To reduce inference costs, one can either downsize the LLM or reduce the number of input tokens needed to represent the image, the latter of which has been the focus of many recent efforts around token compression. However, it is unclear what the optimal trade-off is given a fixed inference budget. We first characterize this optimal trade-off between the number of visual tokens and LLM parameters by establishing scaling laws that capture variations in performance with these two factors. Our results reveal a surprising trend: for visual reasoning tasks, the inference-optimal behavior in VLMs is achieved by using the largest LLM that fits within the inference budget while minimizing visual token count - often to a single token. While the token reduction literature has mainly focused on maintaining base model performance by modestly reducing the token count (e.g., 5−10x), our results indicate that the compute-optimal inference regime requires operating under even higher token compression ratios. Based on these insights, we take the first steps toward designing token compression algorithms tailored for high-compression settings, utilizing prompt-based compression of tokens. Our work underscores the performance and efficiency benefits of operating in low visual token regimes and the importance of developing tailored token reduction algorithms for such conditions.