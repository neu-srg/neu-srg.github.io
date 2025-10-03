---
layout: seminar
talk-title: Understanding Stragglers in Large Model Training Using What-if Analysis
speaker: Jinkun Lin
affiliation: Cornell University
speaker-webpage: https://cs.nyu.edu/~jl10439/
date: October 10, 2025
day: Friday
time: 10:00 am
location: Ryder Hall 156
online: YES
---

**Abstract:**

Large language model (LLM) training is one of the most demanding distributed computations today, often requiring thousands of GPUs with frequent synchronization across machines. Such a workload pattern makes it susceptible to stragglers, where the training can be stalled by few slow workers. At ByteDance we find stragglers are not trivially always caused by hardware failures, but can arise from multiple complex factors. This work aims to present a comprehensive study on the straggler issues in LLM training, using a five-month trace collected from our ByteDance LLM training cluster. The core methodology is what-if analysis that simulates the scenario without any stragglers and contrasts with the actual case. We use this method to study the following questions: (1) how often do stragglers affect training jobs, and what effect do they have on job performance; (2) do stragglers exhibit temporal or spatial patterns; and (3) what are the potential root causes for stragglers?

**Bio:**

Jinkun Lin is a postdoc researcher at Cornell University advised by Rachee Singh. He did his PhD candidate at NYU systems group, where he is co-advised by Prof. Aurojit Panda and Jinyang Li. His research interest lies in systems for machine learning, and focuses on addressing reliability and performance challenges in ML systems including ML compilers, LLM training and serving systems.

