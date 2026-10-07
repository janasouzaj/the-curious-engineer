# Module 01 — Linux & Operating Systems

**Status:** Restarting  
**Planned:** October 2026

---

# Purpose

Build a deeper mental model of Linux so that production symptoms can be connected to what the operating system is actually doing.

The objective is not command memorization.

The objective is:

```text
Symptom
  ↓
System concept
  ↓
Evidence
  ↓
Diagnosis
```

---

# Learning Objectives

By the end of this module, I should be able to explain and investigate:

- kernel vs. user space
- processes
- threads
- process states
- signals
- CPU usage
- load average
- memory
- virtual memory
- filesystem basics
- I/O
- file descriptors
- `/proc`
- permissions
- systemd
- journald
- sockets

---

# Primary Book

**How Linux Works, 3rd Edition — Brian Ward**

https://nostarch.com/howlinuxworks3

---

# Official Documentation

- Linux kernel: https://kernel.org/
- systemd: https://systemd.io/
- man pages: https://man7.org/linux/man-pages/

---

# Study Path

## Week 1 — Linux mental model

Topics:

- hardware
- kernel
- user space
- system calls
- processes
- filesystem

Evidence to collect:

```bash
uname -a
ps aux
ls /proc
cat /proc/<pid>/status
```

## Week 2 — Processes, CPU and memory

Topics:

- process lifecycle
- threads
- CPU time
- load average
- memory usage
- virtual memory

Labs:

- CPU stress
- load average
- process investigation
- memory pressure

## Week 3 — I/O, files and services

Topics:

- file descriptors
- filesystem
- disk usage
- I/O
- systemd
- journald

Labs:

- open file descriptors
- disk pressure
- failing systemd service
- journald investigation

## Week 4 — Networking bridge

Topics:

- sockets
- listening ports
- processes and network connections
- `/proc/net`
- connection investigation

Lab:

**Which process owns this port?**

---

# First Project

## Linux Troubleshooting Lab

Create controlled failures and investigate them.

```text
CPU high
Load average high
Memory pressure
Disk full
Permission denied
Service failed
Port already in use
Unexpected process state
```

---

# Exit Criteria

I should be able to answer without a tutorial:

1. What is a process?
2. What is a thread?
3. What does load average represent?
4. Why can load be high while CPU is not saturated?
5. Where can I inspect process information?
6. What is a file descriptor?
7. How does systemd manage a service?
8. Where do I look for service logs?
9. How do I find which process owns a listening socket?
10. How would I approach a CPU, memory or disk incident?

---

# Reflection

Before moving to Module 02, write a short reflection:

> What changed in the way I think about Linux after investigating it instead of merely using it?