---
layout: seminar
talk-title: Isolation in the cloud: control the system calls, control the attackers
speaker: Dan Williams
affiliation: Virginia Tech
speaker-webpage: https://people.cs.vt.edu/djwillia/
date: Jun 29, 2022
day: Wednesday
time: 11:00 am 
location: 366 WVH
online: YES
---

**Abstract:**

The cloud is an environment in which multiple mutually-distrusting
tenants share a host OS and rely on the cloud provider to maintain
isolation.  In this talk I will provide an overview of my research
into limiting access to the host system through system calls in a
cloud environment.  The talk will first discuss approaches that
deprivilege kernel functionality, either by using traditional
virtualization or with process system call filtering.  Then I will
discuss opportunities and issues when filtering system calls on
processes (without deprivileging kernel functionality), highlighting
two recent projects 1) leveraging scheduling and 2) optimizing filter
chains.  I will conclude by stepping back to look more broadly at eBPF
(the safe Linux kernel extension mechanism underlying its system call
filtering mechanism) and the future directions it inspires.

**Bio:**

Dan Williams is an Assistant Professor in the Department of Computer
Science at Virginia Tech, which he joined in August 2021. Prior to
joining VT, he spent 10 years as a Research Staff Member at the IBM
T.J. Watson Research Center in Yorktown Heights, NY. His research
investigates the systems abstractions for running programs securely
and isolated from one another even in shared environments like the
cloud. He is the original author of the Solo5 unikernel execution
environment, and a co-creator of unikernel-inspired Nabla containers.
