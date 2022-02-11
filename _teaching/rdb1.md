---
title: "Relational Database Systems 1"
category: Lectures
collection: teaching
type: "Undergraduate Course (B.Sc.)"
permalink: "/teaching/rdb1"
venue: "TU Braunschweig, Institut für Informationssysteme"
date: 2019-10-01
location: Braunschweig, Germany
roles:
  - name: Assistant
    terms:
    - semester: winter
      year: 2018
    - semester: winter
      year: 2019
  
tags: [relational databases]
---


## Terms and Roles
{% for role in page.roles %}
  **{{ role.name }}:** {% for term in role.terms %}{% if term.url %}[{{ term.semester | capitalize }} {{ term.year }}]({{ term.url }}){% else %}{{ term.semester | capitalize }} {{ term.year }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}
{% endfor %}
