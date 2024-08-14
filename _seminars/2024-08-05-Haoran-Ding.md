---
layout: seminar
talk-title: Automated Verification of Idempotence for Serverless Applications
speaker: Haoran Ding
affiliation: SJTU
speaker-webpage:
date: August 5, 2024
day: Monday
time: 10:30 am 
location: WVH 366
online: NO
---

**Abstract:**
Serverless computing is a promising cloud computing paradigm. It tolerates failures by retrying failed applications. To avoid errors from retries (e.g., duplicate charge), prior works log all operations to achieve idempotence, which means that applications expose the same behavior regardless of retries. However, logs introduce a heavy performance burden.

This talk will present Flux, the first toolkit that automatically verifies the idempotence of serverless applications. Flux proposes a new formal definition, idempotence consistency, which stipulates that retries are transparent to users. To verify idempotence consistency, Flux proposes idempotence simulation and failure reduction to automatically reason about unbounded interleavings posed by concurrency and failures.

For 27 representative serverless applications, Flux proves that logging only 33% operations can ensure idempotence. Compared to prior works that log all operations, Flux brings up to 10x higher peak throughput.


**Bio:**
Haoran Ding is a PhD candidate at the Institute of Parallel and Distributed Systems (IPADS) of Shanghai Jiao Tong University. His research focuses on the intersection of formal verification and systems software, aiming to develop practical theories and tools that can enhance both system correctness and performance. His research has been published in OSDI, SOSP, and SIGMOD.
