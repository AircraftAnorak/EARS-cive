---
title: Radio Amateurs
layout: default
parent: History
nav_order: 2
has_toc: true
---

{% include math.html %}

<h1><b><span style="color:Gold">Radio Amateur Wall of Fame</span></b></h1>

A list of the Radio Amateurs that have been a member of EARS or have been trained by us

<ul>
{% for member in site.data.members %}
  <li>
    <b><a href="https://www.qrz.com/db/{{ member.callsign }}">{{ member.callsign }}</a></b> - {% if member.name %} {{ member.name }} {% endif %} {% if member.role %} ({{ member.role }}) {% endif %}
  </li>
{% endfor %}
</ul>