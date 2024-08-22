---
layout: seminar
talk-title: "XRP: In-Kernel Storage Functions with eBPF"
speaker: Yuhong Zhong
affiliation: Columbia University
speaker-webpage:
date: April 19, 2024
day: Friday
time: 12:30 0m 
location: WVH 362
online: NO
---

**Abstract:**

With the emergence of microsecond-scale NVMe storage devices, the Linux kernel storage stack overhead has become significant, almost doubling access times. We present XRP, a framework that allows applications to execute user-defined storage functions, such as index lookups or aggregations, from an eBPF hook in the NVMe driver, safely bypassing most of the kernel’s storage stack. To preserve file system semantics, XRP propagates a small amount of kernel state to its NVMe driver hook where the user-registered eBPF functions are called. We show how two key-value stores, BPF-KV, a simple B+-tree key-value store, and WiredTiger, a popular log-structured merge tree storage engine, can leverage XRP to significantly improve throughput and latency.


**Bio:**

Yuhong Zhong is a second-year PhD student in Computer Science at Columbia University, advised by Asaf Cidon. He is broadly interested in computer systems, especially CXL, memory tiering, storage systems, and eBPF. His research was recognized with the Best Paper Award at OSDI '22. Before starting his PhD, Yuhong was a software engineer at VMware in the vSAN group.

