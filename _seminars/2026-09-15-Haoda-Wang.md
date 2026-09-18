---
layout: seminar
talk-title: "Houston, We Have a Problem: Systems Challenges of Large Scale Spacecraft Deployments"
speaker: Haoda Wang
affiliation: Columbia University
speaker-webpage: https://h313.info/
date: September 15, 2026
day: Tuesday
time: 11:30 am
location: Kariotis 302
online: NO
---

**Abstract:**

The collapsing cost of space launches has disrupted the way satellites are deployed, shifting the industry from a model of a few expensive fault-tolerant high-orbit satellites to arrays of commodity low-cost SmallSats in low-Earth orbit. However, satellite software hasn't kept up with the hardware trends, and missions are still using the ad-hoc flight software infrastructure built for expensive one-off missions in high-altitude orbits, even as constellations of tens or even hundreds of SmallSats come online. This motivates new approaches rooted in verification and language design.

In this talk, I present Orbital, which extends eBPF's symbolic execution to derive tight worst-case execution time bounds for hard real-time multi-tenant scheduling on SmallSats, and Radshield, a programming model that efficiently replicates execution and protects commodity hardware from radiation-induced silent data corruption. I'll also discuss ongoing work with NASA-JPL to adapt WebAssembly as the onboard command DSL for their flight software framework, and open problems at the intersection of software systems and space that this community is well-positioned to tackle.

**Bio:**

Haoda Wang is a PhD candidate at Columbia University developing software systems for spacecraft. Previously, he has worked on flight software for the Mars Perseverance rover, and developed Mars Global Localization, using an onboard commodity chip in a high-radiation environment. He is also a 2024 NSF GRFP fellow and a 2022 DoD NDSEG fellow, and holds a BS in Computer Engineering and Computer Science from the University of Southern California.
