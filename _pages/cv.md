---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

[Download CV as PDF]({{ '/cv/cv.pdf' | relative_url }})

## Education

- **Ph.D. in Computer Science and Technology**, Nanjing University, September 2024–present. Advisor: [Yu Huang](https://cs.nju.edu.cn/yuhuang/).
- **B.S. in Computer Science and Technology**, Nanjing University, September 2020–June 2024.

## Research Interests

I use AI agents to write formal specifications, check concurrent and distributed systems for bugs, and prove properties of those systems with TLA+.

## Publications

{% assign papers = site.publications | sort: 'date' | reverse %}
{% for paper in papers %}- [{{ paper.title }}]({{ paper.url | relative_url }}). *{{ paper.venue }}*, {{ paper.date | date: '%Y' }}.
{% endfor %}

## Projects

- [Specular](https://specularhq.ai/) (formerly Specula) generates TLA+ specifications from system code, checks them for bugs, and reproduces the findings in the implementation.
- [TLAPS-Bench](https://specular-org.github.io/tlaps-bench-website/) evaluates AI agents on machine-checked proofs for real-world TLA+ specifications.
- [SysMoBench](https://sysmobench.com/) evaluates AI agents on writing formal specifications that match system implementations.
- [System Intelligence Benchmark](https://github.com/sys-intelligence/system-intelligence-benchmark) evaluates AI capabilities across computing systems tasks.
- [Fluid](https://fluid-cloudnative.github.io/) is a CNCF project for data orchestration and acceleration on Kubernetes.

## Talks

{% for talk in site.talks reversed %}- [{{ talk.title }}]({{ talk.link }}). {{ talk.venue }}, {{ talk.date | date: '%B %Y' }}.
{% endfor %}

## Awards and Honors

- **TLAi+ Challenge**, first place with Specula, 2025.
- **18th Challenge Cup**, National First Prize with Fluid, 2023.

## Languages

- Chinese (native)

## Contact

Department of Computer Science, Nanjing University, Nanjing, Jiangsu, China.

[cq@smail.nju.edu.cn](mailto:cq@smail.nju.edu.cn) · [GitHub](https://github.com/Qian-Cheng-nju)
