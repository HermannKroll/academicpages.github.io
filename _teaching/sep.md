---
title: "Softwareentwicklungspraktikum"
category: Lab
collection: teaching
type: "Undergraduate Course (B.Sc.)"
permalink: "/teaching/sep"
venue: "TU Braunschweig, Institut für Informationssysteme"
date: 2020-04-01
location: Braunschweig, Germany
roles:
  - name: Supervisor
    terms:
    - semester: summer (SherloQL)
      year: 2020
    - semester: summer (Music Tinder)
      year: 2019
  
tags: [lab]
---


## Terms and Roles
{% for role in page.roles %}
  **{{ role.name }}:** {% for term in role.terms %}{% if term.url %}[{{ term.semester | capitalize }} {{ term.year }}]({{ term.url }}){% else %}{{ term.semester | capitalize }} {{ term.year }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}
{% endfor %}
