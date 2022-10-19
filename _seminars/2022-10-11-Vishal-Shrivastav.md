---
layout: seminar
talk-title: "Enabling Stateful In-Network Computing at Multi-Terabit Line Rates"
speaker: Vishal Shrivastav
affiliation: Purdue University
speaker-webpage: 
date: Oct 11, 2022
day: Tuesday
time: 10:30 am
location: 655 ISEC
online: YES
---

**Abstract:**
Stateful in-network computing in the network data plane, powered by programmable switches such as Tofino, has shown to improve the performance of a wide variety of distributed applications, ranging from network applications, such as load balancing and congestion control, to network caching, to distributed consensus, to database queries, to machine learning, to name a few. However,  as the network data plane speeds have already  reached 10s of terabits per second and continue to increase further, scaling stateful in-network applications to run at such line rates is becoming increasingly challenging. This is primarily because to achieve multi-terabit line rates, programmable switches have to employ multiple parallel packet processing pipelines, as the clock speed of a single packet processing pipeline has saturated due to the slowdown in transistor scaling. This leads to the fundamental tension in parallel computing between performance and functional correctness.
 
In this talk, I will present MP5, which takes the first step towards resolving this classic tension between performance and functional correctness within a new context of multi-pipelined programmable switches. MP5 is a new programmable switch design, that extends the existing programmable switch hardware architecture, compiler, and runtime, to guarantee that the runtime behavior of a program running on a multi-pipelined switch will be functionally equivalent to a single-pipelined switch, while also achieving close to ideal packet processing rate. I will conclude this talk by discussing some of the limitations of MP5 and some open research problems in this domain.

**Bio:**
Vishal Shrivastav is an Assistant Professor of Electrical and Computer Engineering at Purdue University. His research interests lie at the intersection of computer networks, systems, and hardware architecture. His current research focuses on designing new hardware architectures for programmable switches, and leveraging them to improve the state of in-network computing in general. Vishal holds a Ph.D. and an M.S., both in Computer Science, from Cornell University and a B.Tech. in Computer Science and Engineering from the Indian Institute of Technology, Kharagpur.


