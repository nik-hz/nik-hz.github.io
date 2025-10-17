---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
---

## Education

- **Columbia University**, New York, US  
  *PhD in Computer Science*
  *M.S. in Computer Science (Feb 2026)*  
  *B.A. in Computer Science (May 2024, GPA: 3.73)*  
  Honors: Academic Scholarship, Dean’s List  

- **Institut d'études Politiques (IEP) de Paris**, Paris, FR  
  *B.A. in Economics (May 2024, GPA: 4.00)*

---

## Experience

- **Columbia University**, Research Assistant — *New York, US*  
  *Jan 2024 – May 2025*  
  Formal Verification, Program Synthesis, and AI.  
  - Applied synthesis methods to increase safety and predictability of LLM-generated code.  
  - Used natural language to generate complex arbiters through LLMs.

- **Columbia University**, Research Assistant — *New York, US*  
  *Aug 2023 – May 2025*  
  Deep Reinforcement Learning for Finance.  
  - Lead RA on SIRS/STAR-funded project improving LLM understanding of code and tabular data.  
  - Built GPU-parallel RL frameworks for financial trading.  
  - Managed team of six researchers and coordinated ICAIF’24 financial AI competition.

- **IBM Research**, Research Assistant — *New York, US*  
  *Oct 2024 – Dec 2024*  
  Co-design of resistive processing units (RPU) for analog in-memory compute systems.  
  - Improving energy-efficient AI through neural architecture search (NAS) using IBM AIHWKit.  
  - Developing robust analog deep learning architectures accounting for nonlinearities.

- **Columbia University**, Course Assistant — *Data Structures and Algorithms*  
  *Sep 2023 – May 2024*  
  - Assisted in course delivery for 400+ students; ran review sessions and recitations.

- **Baqend GmbH**, Full-Stack Developer Intern — *Hamburg, DE*  
  *Aug 2020 – Sep 2021*  
  - Built proof-of-concept full-stack apps for five enterprise clients.  
  - Supported production systems used by millions of users weekly.

---

## Publications

{% bibliography --file publications %}

---

## Teaching

{% assign teaching = site.teaching | sort: 'date' | reverse %}
{% for item in teaching %}
  {% include archive-single.html %}
{% endfor %}

---

## Talks

{% assign talks = site.talks | sort: 'date' | reverse %}
{% for item in talks %}
  {% include archive-single.html %}
{% endfor %}
