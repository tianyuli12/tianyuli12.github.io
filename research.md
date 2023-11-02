---
layout: page
permalink: /research/
title: Research
pubs:

    - title:   "[2023] MagTracer: Detecting GPU Cryptojacking Attacks via Magnetic Leakage Signals"
      author:  "Rui Xiao, **Tianyu Li**, Soundarya Ramesh, Jun Han, and Jinsong Han"
      journal: "29th International Conference on Mobile Computing and Networking (MobiCom 2023)"
      # note:    ""
      # year:    "2023"
      url:     "https://dl.acm.org/doi/abs/10.1145/3570361.3613283#:~:text=MagTracer%20utilizes%20a%20small%20magnetic,the%20victim%20about%20potential%20cryptojacking."
      doi:     "https://doi.org/10.1145/3570361.3613283"


---

## Publications

{% assign thumbnail="left" %}

{% for pub in page.pubs %}
{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %}
