---
layout: page
permalink: /publications/index.html
title: Publications
pubs:

  - author: Changjiang Li, __Ren Pang__, Bochuan Cao, Jinghui Chen, Shouling Ji, Ting Wang
    title: "On the Difficulty of Defending Contrastive Learning against Backdoor Attacks"
    booktitle: "USENIX Security'24"
    url: "https://arxiv.org/abs/2312.09057"
  - author: Zhaohan Xi, Tianyu Du, Changjiang Li, __Ren Pang__, Shouling Ji, Jinghui Chen, Fenglong Ma, Ting Wang
    title: "Defending Pre-trained Language Models as Few-shot Learners Against Backdoor Attacks"
    booktitle: "NeurIPS'23"
    url: "https://arxiv.org/abs/2309.13256"
  - author: Changjiang Li, __Ren Pang__, Zhaohan Xi, Tianyu Du, Shouling Ji, Yuan Yao, Ting Wang
    title: "An Embarrassingly Simple Backdoor Attack against Self-supervised Learning"
    booktitle: "ICCV'23"
    url: "https://arxiv.org/abs/2210.07346"
  - author: Zhaohan Xi, Tianyu Du, Changjiang Li, __Ren Pang__, Shouling Ji, Xiapu Luo, Xusheng Xiao, Fenglong Ma, Ting Wang
    title: "On the Security Risks of Knowledge Graph Reasoning"
    booktitle: "USENIX Security'23"
    url: "https://arxiv.org/abs/2305.02383"
  - author: __Ren Pang__, Changjiang Li, Zhaohan Xi, Shouling Ji, Ting Wang
    title: "The Dark Side of AutoML: Towards Architectural Backdoor Search"
    booktitle: "ICLR'23"
    url: "https://arxiv.org/abs/2210.12179"
  - author: __Ren Pang__, Zheng Zhang, Xiangshan Gao, Zhaohan Xi, Shouling Ji, Cheng Peng, Ting Wang
    title: "TrojanZoo: Towards Unified, Holistic, and Practical Evaluation of Neural Backdoors"
    booktitle: "IEEE EuroS&P'22"
    url: "https://arxiv.org/abs/2012.09302"
  - author: __Ren Pang__, Zhaohan Xi, Shouling Ji, Xiapu Luo, Ting Wang
    title: On the Security Risks of AutoML
    booktitle: "USENIX Security'22"
    url: "https://arxiv.org/abs/2110.06018"
  - author: Zhaohan Xi, __Ren Pang__, Shouling Ji, Ting Wang
    title: Graph Backdoor
    booktitle: "USENIX Security'21"
    url: "https://arxiv.org/abs/2006.09539"
  - author: Xinyang Zhang, __Ren Pang__, Shouling Ji, Fenglong Ma, Ting Wang
    title: "i-Algebra: Towards Interactive Interpretability of Neural Nets"
    booktitle: "AAAI'21"
    url: "https://arxiv.org/abs/2101.09301"
  - author: __Ren Pang__, Xinyang Zhang, Shouling Ji, Xiapu Luo, Ting Wang
    title: "AdvMind: Inferring Adversary Intent of Black-Box Attacks"
    booktitle: "ACM KDD'20"
    url: "https://arxiv.org/abs/2006.09539"
  - author: __Ren Pang__, Hua Shen, Xinyang Zhang, Shouling Ji, Yevgeniy Vorobeychik, Xiapu Luo, Alex Liu, Ting Wang
    title: "A Tale of Evil Twins: Adversarial Inputs versus Poisoned Models"
    booktitle: "ACM CCS'20"
    url: "https://arxiv.org/abs/1911.01559"

preprints:
  - author: Zhaohan Xi, __Ren Pang__, Changjiang Li, Tianyu Du, Shouling Ji, Fenglong Ma, Ting Wang
    title: "Reasoning over Multi-view Knowledge Graphs"
    url: "https://arxiv.org/abs/2209.13702"
---

# Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %}<a href="{{pub.url}}"><span style="color:#ee4c2c">{{pub.title}}</span></a>
    {% else %}<span style="color:#ee4c2c">{{pub.title}}</span>{% endif %}<br>
    {{pub.author}}<br>
    <span style="color:#792fe4">{{pub.booktitle}}{{pub.school}}{{pub.journal}}<br></span>
    {% if pub.slides %}[Slides]({{pub.slides}}){% endif %}
    {% if pub.bibtex %}[Bibtex]({{pub.bibtex}}){% endif %}
{% endunless %}
{% endfor %}

<!-- 
# Preprints

{% for preprint in page.preprints %}
{% unless preprint.hidden %}
  - {% if preprint.url %}<a href="{{preprint.url}}"><span style="color:#ee4c2c">{{preprint.title}}</span></a>
    {% else %}<span style="color:#ee4c2c">{{preprint.title}}</span>{% endif %}<br>
    {{preprint.author}}<br>
    {% if preprint.slides %}[Slides]({{preprint.slides}}){% endif %}
    {% if preprint.bibtex %}[Bibtex]({{preprint.bibtex}}){% endif %}
{% endunless %}
{% endfor %}
 -->
