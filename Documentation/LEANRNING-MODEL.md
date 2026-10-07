# Learning Model

The Curious Engineer is built around one loop:

```text
Learn
  ↓
Experiment
  ↓
Break
  ↓
Investigate
  ↓
Build
  ↓
Document
  ↓
Share
  ↓
Revisit
```

---

# Learn

Use a primary source to understand the concept.

Preferred order:

```text
Book
 ↓
Official documentation
 ↓
Source code / examples
```

---

# Experiment

Turn the concept into a small reproducible environment.

Examples:

- VM
- container
- local Kubernetes cluster
- Prometheus
- Grafana
- OpenTelemetry Collector / Alloy

---

# Break

Introduce a controlled failure.

Examples:

- kill a process
- exhaust CPU
- consume memory
- block a port
- break DNS
- fail a readiness probe
- create bad labels
- generate high cardinality

---

# Investigate

Use evidence to determine what happened.

```text
Symptom
   ↓
Observation
   ↓
Hypothesis
   ↓
Test
   ↓
Result
   ↓
Conclusion
```

Avoid changing several variables at once whenever possible.

---

# Build

Create something small enough to show the concept working:

- shell tool
- exporter
- dashboard
- PromQL query
- telemetry pipeline
- Terraform module
- Kubernetes deployment
- incident runbook

---

# Document

Every meaningful experiment should preserve:

- why it exists
- environment
- hypothesis
- procedure
- observed result
- analysis
- lessons learned
- troubleshooting
- evidence
- references

---

# Share

GitHub is the primary technical record.

Social content is derived from the work.

```text
Lab
 ↓
Insight
 ↓
Short reflection
 ↓
Long-form article when warranted
```

---

# Revisit

After several weeks, revisit important concepts.

Ask:

- Can I explain it without notes?
- Can I troubleshoot it?
- Can I connect it to another layer?
- Can I explain when not to use it?

---

# Definition of Understanding

A topic is considered understood when I can:

1. explain the mental model
2. demonstrate it with a lab
3. break it intentionally
4. diagnose the failure
5. explain the trade-offs
6. connect it to a real operational scenario

---

# Anti-Patterns

Avoid:

- collecting courses
- copying tutorials
- installing every tool in the ecosystem
- optimizing before measuring
- building huge projects too early
- publishing shallow content just to maintain a streak
- marking a topic complete because a command worked once

---

# The Core Question

> **What problem does this solve, what happens underneath it, and how would I know when it is failing?**