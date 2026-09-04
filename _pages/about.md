---
permalink: /
title: "Yuan-Chia Chang 張元嘉"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a Human-Robot Interaction (HRI) researcher with an engineering background and hands-on experience in robot interface development, teleoperation system integration, field testing, and user behavior analysis. My work bridges system development and empirical research to understand the challenges that arise when robots move into real-world social environments.
With a multidisciplinary background, I aim to contribute to the application of robots and artificial intelligence through both teaching and research.


Publications
======

<ul>
{% for post in site.publications reversed %}
  <li>
    <strong>{{ post.title }}</strong><br>
    {{ post.citation }}<br>
    {% if post.paperurl %}<a href="{{ post.paperurl }}">[paper]</a>{% endif %}
  </li>
{% endfor %}
</ul>
