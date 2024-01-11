---
layout: seminar
talk-title: "Toward Practical Kernel Bypass for Datacenter Computing"
speaker: Joshua Fried
affiliation: MIT
speaker-webpage: 
date: November 30, 2023
day: Thursday
time: 2:50 pm
location: Hastings Suite 107 
online: NO
---

**Abstract:**

Kernel bypass systems have demonstrated that they can significantly improve throughput, latency, and efficiency for I/O intensive datacenter applications relative to traditional operating systems. However, bypassing the kernel has its downsides: it typically requires dedicating resources (e.g. cores, memory) and rewriting applications to use new interfaces. Dedicating resources is undesirable to datacenter operators because these resources may be underutilized as demand shifts over time, and rewriting software is both costly and wastes existing investments in software.
In this talk, I will present Junction, a new system that brings the benefits of kernel bypass to unmodified applications, while maintaining a minimal resource footprint for each application. Junction leverages modern network card features to reduce both memory overheads and monitoring overheads, allowing it to pack thousands of instances on one machine. Junction includes a library operating system that provides compatibility with existing applications through an implementation of the Linux system call interface. The implementation embraces kernel bypass to support common OS functionality with minimal reliance on the host kernel. Junction is able to match or exceed the performance of state-of-the-art kernel bypass systems without requiring application porting. Junction delivers improvements in throughput, latency, and CPU efficiency for unmodified network-intensive datacenter applications and supports commonly used frameworks such as Go, Python, and Java without requiring modifications.

**Bio:**

Joshua Fried is a final year PhD student at MIT advised by Adam Belay. He is broadly interested in operating systems and networks, and distributed systems, with a focus on improving performance and efficiency in datacenters through better operating system design.


