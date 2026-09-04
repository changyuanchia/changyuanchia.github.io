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


Research Interests
======

- Human-Robot Interaction
- Human-Computer Interaction
- User Experience Design and Research
- Human-Centered Physical AI
- Social robots and avatar robots
- Moral interaction and authoritative presence

Publications
======

<ul>
{% for post in site.publications reversed %}
  <li>
    <strong><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></strong><br>
    {{ post.citation }}
  </li>
{% endfor %}
</ul>

[View all publications]({{ site.baseurl }}/publications/){: .btn .btn--primary} [View CV]({{ site.baseurl }}/cv/){: .btn}
