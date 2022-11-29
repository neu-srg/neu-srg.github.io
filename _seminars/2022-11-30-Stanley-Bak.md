---
layout: seminar
talk-title: "Formal Verification for Autonomous Cyber-Physical Systems"
speaker: Stanley Bak
affiliation: Stony Brook University
speaker-webpage: 
date: Nov 30, 2022
day: Wednesday
time: 3:00 pm
location: 
online: YES
---

**Abstract:**
ACAS Xu is an air-to-air collision avoidance system designed for unmanned aircraft that issues horizontal turn advisories to avoid an intruder aircraft. Due the use of a large lookup table in the design, a neural network compression of the policy was proposed. Analysis of this system has spurred a significant body of research in the formal methods community on neural network verification. While many powerful methods have been developed, most work focuses on open-loop properties of the networks, rather than the main point of the system---collision avoidance---which requires closed-loop analysis.

In this talk, we will a recent technique which aims to verify a closed-loop approximation of ACAS Xu using state quantization and backreachability. We use favorable assumptions for the analysis---perfect sensor information, instant following of advisories, ideal aircraft maneuvers and an intruder that only flies straight. When the method fails to prove the system is safe, we refine the quantization parameters until generating counterexamples where the original (non-quantized) system also has collisions.

**Bio:**
Stanley Bak is an assistant professor in the Department of Computer Science at Stony Brook University investigating the verification of autonomy, cyber-physical systems, and neural networks. He received a PhD from the University of Illinois at Urbana-Champaign (UIUC) in 2013, worked at the Air Force Research Laboratory (AFRL) before joining Stony Brook University in 2020. He received the AFOSR Young Investigator Research Program (YIP) award in 2020.

