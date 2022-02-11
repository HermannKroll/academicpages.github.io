---
title: "Teamproject"
category: Lab
collection: teaching
type: "Undergraduate Course (B.Sc.)"
permalink: "/teaching/tp"
venue: "TU Braunschweig, Institut für Informationssysteme"
date: 2022-02-01
location: Braunschweig, Germany
roles:
  - name: Supervisor
    terms:
    - semester: winter (Narrative Information Access for Pharmacy)
      year: 2022 
    - semester: summer (SherloQL 2.0)
      year: 2021
    - semester: winter (Narrative Query Designer)
      year: 2019
  
tags: [lab]
---


## Terms and Roles
{% for role in page.roles %}
  **{{ role.name }}:** {% for term in role.terms %}{% if term.url %}[{{ term.semester | capitalize }} {{ term.year }}]({{ term.url }}){% else %}{{ term.semester | capitalize }} {{ term.year }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}
{% endfor %}
