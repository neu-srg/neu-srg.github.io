---
layout: seminar
talk-title: "Distributed PIR: Scaling Private Messaging via the Users' Machines"
speaker: Yossi Gilad
affiliation: Hebrew University of Jerusalem
speaker-webpage: 
date: Oct 18, 2023
day: Wednesday
time: 3:00 pm
location: 655 ISEC 
online: NO
---

**Abstract:**
This paper presents a new architecture for metadata-private messaging that counters scalability challenges by offloading most of the computational work to the clients. We introduce DPIR, which makes designating work to clients practical by ensuring privacy and availability even if they misbehave. DPIR addresses the privacy challenge by leveraging Private Information Retrieval (PIR), a cryptographic protocol for reading messages where the responder only sees encrypted requests. It addresses the availability challenge by coupling two insights: First, in certain homomorphic encryption schemes, ciphertext arithmetic is implemented via standard algebraic operators over polynomial rings. Second, the PIR protocol can be viewed as an instance of matrix multiplication over these rings. Combining these insights allows a server to verify PIR responses much more efficiently than computing them by applying Freivalds' algorithm.

In DPIR, the server distributes the PIR processing work to clients, verifies their outputs, and removes offending clients. The ability to detect and remove offenders provides an incentive mechanism for honest client behavior by conditioning messaging through DPIR on correctly processing PIR queries from other users. The result is a metadata-private messaging system that asymptotically improves scalability over prior work with the same threat model. We show through experiments on a prototype implementation that DPIR concretely improves performance by 3.25× and 4.31× over prior work and that the performance gap grows with the user base size.

**Bio:**

Yossi Gilad is a Scharf-Ullman endowed Senior Lecturer at the School of Computer Science and Engineering, the Hebrew University of Jerusalem. Prior to the Hebrew University, he was a postdoctoral researcher at the Massachusetts Institute of Technology and Boston University. His research focuses on designing, building, and analyzing secure and scalable protocols and networked systems.


