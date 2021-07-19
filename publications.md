---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: __Ren Pang__, Hua Shen, Xinyang Zhang, Shouling Ji, Yevgeniy Vorobeychik, Xiapu Luo, Alex Liu, Ting Wang
    title: "A Tale of Evil Twins: Adversarial Inputs versus Poisoned Models"
    booktitle: "ACM CCS'20"
    url: "https://arxiv.org/abs/1911.01559"
  - author: __Ren Pang__, Xinyang Zhang, Shouling Ji, Xiapu Luo, Ting Wang
    title: "AdvMind: Inferring Adversary Intent of Black-Box Attacks"
    booktitle: "ACM KDD'20"
    url: "https://arxiv.org/abs/2006.09539"
  - author: Xinyang Zhang, __Ren Pang__, Shouling Ji, Fenglong Ma, Ting Wang
    title: "i-Algebra: Towards Interactive Interpretability of Neural Nets"
    booktitle: "AAAI'21"
    url: "https://arxiv.org/abs/2101.09301"
  - author: Zhaohan Xi, __Ren Pang__, Shouling Ji, Ting Wang
    title: Graph Backdoor
    booktitle: "USENIX Security '21"
    url: "https://arxiv.org/abs/2006.09539"
preprints:
  - author: __Ren Pang__, Zheng Zhang, Xiangshan Gao, Zhaohan Xi, Shouling Ji, Cheng Peng, Ting Wang
    title: "TROJANZOO: Everything you ever wanted to know about neural backdoors (but were afraid to ask)"
    url: "https://arxiv.org/abs/2012.09302"
---

# Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}})
    {% else %} {{pub.title}}
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}<br>
    {% if pub.address %}{{pub.address}}
    {% endif %}{% if pub.slides %}[Slides]({{pub.slides}})
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}})
    {% endif %}
{% endunless %}
{% endfor %}


# Preprints

{% for preprint in page.preprints %}
{% unless preprint.hidden %}
  - {% if preprint.url %} [{{preprint.title}}]({{preprint.url}})
    {% else %} {{preprint.title}}
    {% endif %}{% if preprint.type %}({{preprint.type}})
    {% endif %}<br>
    {{preprint.author}}<br>
    {% if preprint.type == 'Technical Report' %}{{preprint.number}}
    {% endif %}{{preprint.booktitle}}{{preprint.school}}{{preprint.journal}}<br>
    {% if preprint.address %}{{preprint.address}}
    {% endif %}{% if preprint.slides %}[Slides]({{preprint.slides}})
    {% endif %}{% if preprint.bibtex %}[Bibtex]({{preprint.bibtex}})
    {% endif %}
{% endunless %}
{% endfor %}