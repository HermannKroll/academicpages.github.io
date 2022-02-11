---
title: "Relational Database Systems 2"
category: Lectures
collection: teaching
type: "Graduate Course (M.Sc.)"
permalink: "/teaching/rdb2"
venue: "TU Braunschweig, Institut für Informationssysteme"
date: 2019-04-01
location: Braunschweig, Germany
roles:
  - name: Assistant
    terms:
    - semester: summer
      year: 2019
  
tags: [relational databases]
---


## Terms and Roles
{% for role in page.roles %}
  **{{ role.name }}:** {% for term in role.terms %}{% if term.url %}[{{ term.semester | capitalize }} {{ term.year }}]({{ term.url }}){% else %}{{ term.semester | capitalize }} {{ term.year }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}
{% endfor %}
