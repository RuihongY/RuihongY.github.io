---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a PhD candidate in Electrical and Computer Engineering at the **University of Minnesota**, advised by [Prof. Chris H. Kim](https://scholar.google.com/citations?user=...). My research sits at the intersection of **domain-specific hardware acceleration**, **physics-based computing**, and **software–hardware co-design**.

My current focus is on building Ising computing systems end-to-end: from full-custom mixed-signal chip design and tapeout (TSMC 16/28nm) to FPGA-based accelerators and system-level optimization frameworks that bridge the gap between large-scale combinatorial problems and capacity-constrained hardware.

Before Minnesota, I received my MS from the **University of Washington** and my B.Eng from the **University of Liverpool**, both in Electrical and Computer Engineering. I have also interned at **NVIDIA** (Tegra System Architecture), **MediaTek** (ASIC Design), and **Infineon Technologies** (Digital IC Design).

---

## Research Interests

- Physics-based Ising computing and combinatorial optimization
- Domain-specific acceleration (FPGA / ASIC co-design)
- Software–hardware co-design for emerging computing paradigms
- Mixed-signal VLSI and full-custom chip design

---

## News

- **Summer 2026** — Interning at NVIDIA, Westford MA (Tegra System Architecture)
- **2026** — Paper accepted at ISCA 2026, ASPLOS 2026, and DATE 2026
- **2025** — Paper accepted at ESSERC 2025

---

## Selected Publications

{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
