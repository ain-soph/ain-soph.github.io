---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: Ren Pang, Hua Shen, Xinyang Zhang, Shouling Ji, Yevgeniy Vorobeychik, Xiapu Luo, Alex Liu, Ting Wang
    title: "A Tale of Evil Twins: Adversarial Inputs versus Poisoned Models"
    booktitle: "ACM CCS'20"
    url: "https://arxiv.org/abs/1911.01559"
  - author: Ren Pang, Xinyang Zhang, Shouling Ji, Xiapu Luo, Ting Wang
    title: "AdvMind: Inferring Adversary Intent of Black-Box Attacks"
    booktitle: "ACM KDD'20"
    url: "https://arxiv.org/abs/2006.09539"
  - author: Xinyang Zhang, Ren Pang, Shouling Ji, Fenglong Ma, Ting Wang
    title: "i-Algebra: Towards Interactive Interpretability of Neural Nets"
    booktitle: "AAAI'21"
    url: "https://arxiv.org/abs/2101.09301"
  - author: Zhaohan Xi, Ren Pang, Shouling Ji, Ting Wang
    title: Graph Backdoor
    booktitle: "USENIX Security '21"
    url: "https://arxiv.org/abs/2006.09539"
preprints:
  - author: Ren Pang, Zheng Zhang, Xiangshan Gao, Zhaohan Xi, Shouling Ji, Cheng Peng, Ting Wang
    title: "TROJANZOO: Everything you ever wanted to know about neural backdoors (but were afraid to ask)"
    url: "https://arxiv.org/abs/2012.09302"
---

# Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}

# Preprints

{% for pub in page.preprints %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}