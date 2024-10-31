---
layout: page
permalink: /research/
title: Research
pubs:

    
    - title:   "SPAS: Continuous Release of Data Streams under w-Event Differential Privacy"
      author:  "Xiaochen Li, **Tianyu Li (co-first)**, Yitian Cheng, Chen Gong, Kui Ren, Zhan Qin, Tianhao Wang"
      journal: "International Conference on Management of Data"
      note:    "To appear"
      year:    "[co-first][SIGMOD 2025]"

    
    - title:   "MagTracer: Detecting GPU Cryptojacking Attacks via Magnetic Leakage Signals"
      author:  "Rui Xiao, **Tianyu Li**, Soundarya Ramesh, Jun Han, and Jinsong Han"
      journal: "International Conference on Mobile Computing and Networking"
      # note:    ""
      year:    "[MobiCom 2023]"
      url:     "https://dl.acm.org/doi/abs/10.1145/3570361.3613283#:~:text=MagTracer%20utilizes%20a%20small%20magnetic,the%20victim%20about%20potential%20cryptojacking."
      doi:     "https://doi.org/10.1145/3570361.3613283"



---

## Publications

{% assign thumbnail="left" %}

{% for pub in page.pubs %}

{{pub.year}} [**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})* {% endif %} 

{% endfor %}
