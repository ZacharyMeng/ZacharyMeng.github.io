---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>
# About me
Weikang (Zachary) is a third-year Ph.D. candidate (2023-) at [SMULL Group](https://cszhengzhang.cn/SMULL/) of [HITsz CS](http://cs.hitsz.edu.cn) advised by Prof. [Zheng Zhang](https://cszhengzhang.cn/). He received his B.S. degree in Information and Computational Science at [Harbin Institute of Technology](https://www.hit.edu.cn/) in 2023. His research interests lie in efficient training and inference algorithms for large-scale foundation models, particularly linear attentions.


# News
- *2026.01*: &nbsp;📮📮 Our new work "[STILL: Selecting Tokens for Intra-Layer Hybrid Attention to Linearize LLMs](https://arxiv.org/abs/2602.02180)" has been uploaded to arXiv.
- *2026.01*: &nbsp;📮📮 Our new work "[MirrorLA: Reflecting Feature Map for Vision Linear Attention](https://arxiv.org/abs/2602.04346)" has been uploaded to arXiv.
- *2025.06*: &nbsp;📮📮 Our new work "[Norm×Direction: Restoring the Missing Query Norm in Vision Linear Attention](https://arxiv.org/abs/2506.21137)" has been uploaded to arXiv.
- *2025.01*: &nbsp;🎉🎉 "[PolaFormer: Polarity-aware Linear Attention for Vision Transformers](https://arxiv.org/abs/2501.15061)" is accepted to ICLR'25. 

# Publications 

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">New Work</div>
      <img src='../images/stillmainfig.jpg' alt="STILL" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">
    <div class="paper-title">STILL: Selecting Tokens for Intra-Layer Hybrid Attention to Linearize LLMs.</div>
    <div class="paper-links">[[paper](https://arxiv.org/pdf/2602.02180)] [[code](https://github.com/ZacharyMeng/STILL)]</div>
    <div class="paper-authors">**Weikang Meng**, Liangyu Huo, Yadan Luo, Jiawen Guan, Jingyi Zhang, Yingjian Li, Zheng Zhang</div>
    <div class="paper-desc">
      This work proposes STILL, an intra-layer hybrid attention framework to efficiently linearize pretrained LLMs while preserving their original capabilities. STILL introduces a Self-Saliency Score with strong local-global consistency to select a small set of globally important tokens for sparse softmax attention, while summarizing the remaining context with linear attention. To mitigate distribution shift during linearization, it further proposes a Norm-Preserved Feature Map (NP-Map) that decouples direction from magnitude and reinjects the pretrained norms, and adopts a unified chunk-wise delayed selection strategy to improve training and inference efficiency for long-context generation.
    </div>
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">New Work</div>
      <img src='../images/mirrorlamainfig.jpg' alt="MirrorLA" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">
    <div class="paper-title">MirrorLA: Reflecting Feature Map for Vision Linear Attention.</div>
    <div class="paper-links">[[paper](https://arxiv.org/pdf/2602.04346)]</div>
    <div class="paper-authors">**Weikang Meng**, Liangyu Huo, Yadan Luo, Yaowei Wang, Yingjian Li, Zheng Zhang</div>
    <div class="paper-desc">
      This work proposes MirrorLA, a linear attention framework that improves the expressivity of non-negative kernel feature maps by replacing passive truncation with active geometric reorientation. It introduces learnable Householder reflections to rotate informative components into the non-negative region while preserving inner-product structure, reducing information loss and stabilizing long-context behavior. MirrorLA further extends this idea with block-wise and cross-head geometric modulations, achieving stronger performance without sacrificing linear-time attention.
    </div>
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">New Work</div>
      <img src='../images/nalaformermainfig.jpg' alt="NaLaFormer" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">
    <div class="paper-title">Norm×Direction: Restoring the Missing Query Norm in Vision Linear Attention.</div>
    <div class="paper-links">[[paper](https://arxiv.org/abs/2506.21137)]</div>
    <div class="paper-authors">**Weikang Meng**, Yadan Luo, Liangyu Huo, Yaowei Wang, Xin Li, Zheng Zhang</div>
    <div class="paper-desc">
      This work introduces NaLaFormer, a linear attention mechanism for Transformer-based vision models. Based on Positive Sequence Entropy (PSE), it theoretically analyzes the dynamic entropy reduction of softmax attention controlled by query norm and proposes a norm-aware kernel function. In addition, NaLaFormer leverages Ptolemy’s theorem to preserve the non-negative constraint of attention weights.
    </div>
  </div>
</div>

<div class='paper-box'>
  <div class='paper-box-image'>
    <div>
      <div class="badge">ICLR 2025</div>
      <img src='../images/ICLR25mainfig.jpg' alt="PolaFormer" width="100%">
    </div>
  </div>
  <div class='paper-box-text' markdown="1">
    <div class="paper-title">PolaFormer: Polarity-aware Linear Attention for Vision Transformers.</div>
    <div class="paper-links">[[paper](https://arxiv.org/abs/2501.15061)] [[code](https://github.com/ZacharyMeng/PolaFormer)]</div>
    <div class="paper-authors">**Weikang Meng**, Yadan Luo, Xin Li, Dongmei Jiang, Zheng Zhang</div>
    <div class="paper-desc">
      This work presents PolaFormer, a linear-complexity attention mechanism for vision Transformers. PolaFormer computes similarity in a polarity-aware manner to avoid neglecting negative interactions. It further proposes a family of element-wise functions to produce spikier attention distributions, and adopts a learnable power function for simplicity and adaptive rescaling.
    </div>
  </div>
</div>


# Honors and Awards
- *2018.09*, National High School Mathematics League, Provincial first prize

# Educations
- *2023.08 - now*, Ph.D student, Harbin Institute of Technology, Shenzhen, School of Computer Science and Technology, Computer Science and Technology
- *2019.08 - 2023.07*, Undergrauate student, Harbin Institute of Technology, School of Mathematics, Information and Computational Science
- *2016.08 - 2019.07*, Harbin NO.3 High School



