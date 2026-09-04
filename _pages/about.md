---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a postdocoral researcher in National Taiwan University, supervised by Prof. [Robin Bing-Yu Chen](https://graphics.cmlab.csie.ntu.edu.tw/~robin/). I finished my doctoral study supervised by Prof. [Takayuki Kanda](https://www.robot.soc.i.kyoto-u.ac.jp/~kanda/) and co-advised by Prof. [Daniel J. Rea](https://hci.cs.umanitoba.ca/people/bio/daniel-rea) in Kyoto University, Japan.
<br>
My research interests are Human-Robot Interaction (HRI), Computer-Supported Collaborative Work (CSCW), and Human-Computer Interaction (HCI). I have hands-on experience in robot interface development, teleoperation system integration, field testing, and user behavior analysis. My work bridges system development and empirical research to understand the challenges that arise as robots move into real-world social environments, particularly those involving avatar robots, perceived robot authority, and authoritative presence.
With a multidisciplinary background, I aim to contribute to the application of robots and artificial intelligence through both teaching and research.


<h2 class="open-sans-section">Academic service</h2>
<section>
  <p>I have reviewed papers for CSCW 2020, CHI 2020 late breaking work, HAI 2023, HAI 2024, RO-MAN 2025, HRI 2025, HRI 2026, THRI (Transactions on Human-Robot Interaction), International Journal of Social Robotics</p>
</section>


<h2 class="open-sans-section">Publications</h2>

<style>
  .publication-list {
    display: grid;
    gap: 1.5rem;
    margin: 1.25rem 0 0;
  }

  .page__content .open-sans-section {
    font-family: "Open Sans Condensed", sans-serif;
    font-weight: 300;
  }

  .publication-item {
    display: grid;
    grid-template-columns: minmax(150px, 210px) minmax(0, 1fr);
    gap: 1.25rem;
    align-items: start;
    padding-bottom: 1.5rem;
    border-bottom: 1px solid var(--global-border-color);
  }

  .publication-image {
    width: 100%;
    aspect-ratio: 16 / 10;
    object-fit: cover;
    border-radius: 4px;
  }

  .publication-title .open-sans-section {
    display: block;
    margin-bottom: 0.4rem;
    line-height: 1.35;
  }

  .publication-citation {
    line-height: 1.55;
  }

  .publication-paper-link {
    display: inline-block;
    margin-top: 0.45rem;
  }

  @media (max-width: 600px) {
    .publication-item {
      grid-template-columns: 1fr;
      gap: 0.8rem;
    }

    .publication-image {
      max-height: 240px;
    }
  }
</style>

<div class="publication-list">
{% for post in site.publications reversed %}
  <article class="publication-item">
    {% if post.image %}
      <img class="publication-image" src="{{ site.baseurl }}{{ post.image }}" alt="Image for {{ post.title }}" loading="lazy">
    {% endif %}
    <div>
      <strong class="publication-title">{{ post.title }}</strong>
      <div class="publication-citation">{{ post.citation }}</div>
      {% if post.paperurl %}<a class="publication-paper-link" href="{{ post.paperurl }}" target="_blank" rel="noopener noreferrer">[paper]</a>{% endif %}
    </div>
  </article>
{% endfor %}
</div>
