---
layout: seminar
talk-title: GEMINI - Fast Failure Recovery in Distributed Training with In-Memory Checkpoints
speaker: Zhuang Wang
affiliation: Amazon Web Services AI
speaker-webpage: https://zhuangwang93.github.io/
date: October 17, 2025
day: Friday
time: 10:00 am
location: Ryder Hall 156
online: YES
---

**Abstract:**

Frequent failures are observed during large model training due to large-scale resources involved and extended training time. This talk presents Gemini, a distributed training system that enables fast failure recovery for large model training by checkpointing to CPU memory of the host machines with much larger aggregated bandwidth. However, two challenges prevent naïvely checkpointing to CPU memory. First, the availability of checkpoints in CPU memory cannot be guaranteed when failures occur. Second, since the communication traffic for training and checkpointing share the same network, checkpoint traffic can interfere with training traffic and harm training throughput. To address these two challenges, we propose: 1) a provably near-optimal checkpoint placement strategy to maximize the probability of failure recovery from checkpoints in CPU memory; and 2) a checkpoint traffic scheduling algorithm to minimize, if not eliminate, the interference of checkpoint traffic on model training. Our evaluation shows that Gemini achieves optimal checkpoint frequency, i.e., every iteration, and incurs no overhead on training throughput for large model training.

**Bio:**

Zhuang Wang is an Applied Scientist at Amazon Web Services AI. He received his Ph.D. degree in Computer Science from Rice University in 2023, fortunately advised by Prof. T. S. Eugene Ng. His current research interests focus on efficient training and inference systems for large language models.