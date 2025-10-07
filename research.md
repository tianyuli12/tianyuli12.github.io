---
layout: page
permalink: /research/
title: Research
pubs:
    - title:   "Adversarial Agent Collaboration for C to Rust Translation"
      author:  "**Tianyu Li**, Ruishi Li, Bo Wang, Brandon Paulsen, Umang Mathur, Prateek Saxena"
      journal: "Under Review"
      # note:    "To Appear"
      year:    "[Arxiv]"
      url:     "https://arxiv.org/abs/2510.03879"
      
    - title:   "Program Skeletons for Automated Program Translation"
      author:  "Bo Wang, **Tianyu Li (co-first)**, Ruishi Li, Umang Mathur, Prateek Saxena"
      journal: "ACM SIGPLAN Conference on Programming Language Design and Implementation"
      # note:    "To Appear"
      year:    "[co-first][PLDI 2025]"
      url:     "https://arxiv.org/pdf/2504.07483"


    - title:   "Translating C To Rust: Lessons from a User Study"
      author:  "Ruishi Li, Bo Wang, **Tianyu Li**, Prateek Saxena, Ashish Kundu"
      journal: "Network and Distributed System Security (NDSS) Symposiuma"
      # note:    ""
      year:    "[NDSS 2025]"
      url:     "https://www.comp.nus.edu.sg/~prateeks/papers/C-Rust-User-Study.pdf"

      
    - title:   "SPAS: Continuous Release of Data Streams under w-Event Differential Privacy"
      author:  "Xiaochen Li, **Tianyu Li (co-first)**, Yitian Cheng, Chen Gong, Kui Ren, Zhan Qin, Tianhao Wang"
      journal: "International Conference on Management of Data"
      # note:    ""
      year:    "[co-first][SIGMOD 2025]"
      url:     "https://dl.acm.org/doi/pdf/10.1145/3714420"

    
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
