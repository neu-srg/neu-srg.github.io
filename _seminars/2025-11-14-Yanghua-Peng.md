---
layout: seminar
talk-title: Large-Scale Multimodal LLM Training in Production
speaker: Yanghua Peng
affiliation: ByteDance
speaker-webpage: https://sites.google.com/view/yanghuapeng/
date: November 14, 2025
day: Friday
time: 10:00 am
location: Ryder Hall 156
online: YES
---

**Abstract:**

Building multimodal LLMs at production scale requires more than raw compute—it demands systems that deliver efficiency, robustness, and adaptability across thousands of GPUs. This talk highlights recent advances that make such training feasible in real-world environments. We present distributed framework designs for training multimodal LLMs efficiently, enabling heterogeneous encoder–LLM pipelines to run with minimal idle time. We introduce parallelism strategies tailored to attention and feed-forward layers of MoE, and efficiently overlaps communication with computation at both operator and pipeline levels. Finally, we show how these optimizations integrate into a cluster-scale orchestration framework that maintains stable training across hundreds of thousand GPUs, achieving strong utilization while tolerating faults, stragglers, and dynamic resource changes.

**Bio:**

Yanghua Peng is a Research Scientist and Engineering Lead at Seed, ByteDance, based in Seattle. He received his Ph.D. in Computer Science from the University of Hong Kong, where he was advised by Prof. Chuan Wu. His research focuses on optimizing large-scale training of foundation and multi-modal LLMs, as well as video generation models. He has extensive experience in developing advanced AI infrastructure, including system co-design, computation and communication optimizations, 5D parallelism, fast checkpointing and data I/O, fault tolerance, and other cross-stack innovations.