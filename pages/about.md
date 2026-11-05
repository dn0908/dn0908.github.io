---
layout: page
title: About
permalink: /about/
weight: 1
---

# **About Me**

<img src="/assets/img/me.png" alt="aboutme" style="width:100%;">

Hi I am **{{ site.author.name }}** :wave:,<br>
I am a PhD student in the Department of Mechanical Engineering at the **Massachusetts Institute of Technology (MIT)**, Cambridge, MA, since Fall 2026, supported by the **2026 Fulbright U.S.-Korea Presidential STEM Initiative Award**.
I work as a research assistant at the [Design Computation and Digital Engineering (DeCoDE) Lab](https://decode.mit.edu/), MIT, led by Prof. Faez Ahmed.

I earned my Master's degree in Mechanical Engineering from Seoul National University in 2026 as a [BK21 FOUR Fellow](/assets/BK21FOUR_Fellowship.pdf), where I worked at the [Biorobotics Lab](https://www.biorobotics.snu.ac.kr/) led by Prof. Kyujin Cho. I earned my Bachelor's degree from the School of Mechanical Engineering, [Yonsei University](https://me.yonsei.ac.kr/me_en/index.do) in 2024.

My research interests lie in robot co-design, developing AI-driven methods that jointly optimize a robot's mechanical design and control, grounded in my hands-on hardware experience from exoskeletons to mobile robots.

<style>
  .affil-grid { display: flex; flex-wrap: wrap; gap: 10px; margin: 8px 0 24px; }
  .affil-box { width: 64px; height: 64px; padding: 8px; background: #fff;
               border: 1px solid rgba(0,0,0,.12); border-radius: 8px;
               display: flex; align-items: center; justify-content: center;
               transition: transform .15s; }
  .affil-box:hover { transform: translateY(-3px); }
  .affil-grid .affil-box img { width: 100%; height: 100% !important; margin: 0 !important;
                               object-fit: contain; }
</style>

<div class="affil-grid">
{% for a in site.data.affiliations %}
  <a class="affil-box" href="{{ a.url }}" target="_blank" rel="noopener" title="{{ a.name }}">
    <img src="{{ a.logo }}" alt="{{ a.name }}">
  </a>
{% endfor %}
</div>

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>