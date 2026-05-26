---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Education

**University of Minnesota** — PhD, Electrical and Computer Engineering (Sep 2023 – Jun 2027)

**University of Washington** — MS, Electrical and Computer Engineering (Sep 2021 – Jun 2023)

**University of Liverpool** — B.Eng, Electrical and Computer Engineering (Sep 2017 – Jun 2021)

---

## Industry Experience

**NVIDIA** — Tegra System Architecture Intern, Westford MA (Summer 2026)

**MediaTek** — ASIC Design Engineer Intern, Austin TX (Mar 2023 – Jun 2023)

**Infineon Technologies** — Digital IC Design Intern, Lynnwood WA (Jan 2023 – Mar 2023)

---

## Publications

{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
