---
title: "Over ons"
lead: "Over Community intro tekst."
header: "/assets/img/content/explain_page_header.jpg"
layout: page
order: 5
---

## Visie


## Doelgroep

## Het Team

{% assign members = site.team | sort:"order" %}
<div class="row members">
{% for member in members %}
  <div class="col-md-3 member">
    {% assign imageurl = '/assets/img/content/' | append: member.name | append: '.png' %}
    <img src="{{ imageurl | relative_url }}">
    <div class="name">{{ member.name }}</div>
    <div class="role">{{ member.role }}</div>
  </div>
{% endfor %}
</div>

<div class="row">
  <div class="col-md-6">
    <p>
      {{ site.legal }} is geregistreerd onder {{ site.kvk }}.
    </p>
    <p>
      Wilt u in contact komen met onze vakvereniging, dan staat het formulier hiernaast tot uw beschikking.
    </p>
  </div>
  <div class="col-md-6">
    {% include form-contact.html %}
  </div>
</div>
