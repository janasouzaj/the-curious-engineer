# Baseline Assessment

**Date:** October 7, 2026

The purpose of this assessment is to distinguish **practical familiarity** from **underlying engineering understanding** and to identify the highest-value study gaps.

---

# Executive Summary

Current profile:

> **Practical DevOps exposure with a promising troubleshooting mindset, but foundational gaps that must be strengthened to reach observability engineering depth.**

The roadmap therefore does not start from zero. It starts by making the mental models underneath existing practical experience stronger.

---

# Area Assessment

| Area | Baseline | Priority |
|---|---|---|
| Linux / systems | Basic | High |
| Networking | Basic | Very High |
| Git / Shell | Basic | Medium |
| Containers | Basic | High |
| Kubernetes | Basic practical familiarity | High |
| CI/CD | Basic | High |
| IaC | Basic | High |
| Cloud / AWS | Practical exposure | Medium |
| Observability | Basic → Intermediate | Very High |
| Prometheus / PromQL | Basic | Very High |
| Grafana | Practical familiarity | High |
| OpenTelemetry | Basic | High |
| SRE | Basic | Very High |
| Incident response | Emerging | High |
| Distributed systems | Basic | Medium |
| Architecture | Basic | Medium |
| Engineering reasoning | Promising | Keep developing |

---

# Strengths Observed

## Troubleshooting instinct

When faced with a Kubernetes failure, the natural instinct was to inspect events and logs. That is a good foundation for evidence-driven investigation.

```text
Symptom
  ↓
Evidence
  ↓
Hypothesis
  ↓
Validation
```

## Operational context

The assessment considered application identity, criticality and customer expectations before choosing what to monitor.

## Awareness of cost and cardinality

Cardinality and telemetry cost are already recognized as relevant topics. The next step is to understand their mechanisms deeply enough to reason about trade-offs.

---

# Priority Gaps

## Linux

Processes, threads, CPU, load average, memory, I/O, file descriptors, `/proc`, systemd, journald and sockets.

## Networking

Build the complete request model:

```text
Application
    ↓
DNS
    ↓
Socket
    ↓
TCP
    ↓
TLS
    ↓
HTTP
    ↓
Server
    ↓
Response
```

## Containers / Kubernetes

Consolidate the architecture and runtime mechanics behind the tools already used.

## Prometheus / PromQL

Priority concepts:

- time series
- labels
- counters
- gauges
- histograms
- `rate()`
- `increase()`
- aggregation
- cardinality
- quantiles

Important baseline correction:

```promql
rate(http_requests_total[5m])
```

estimates the per-second rate of increase of the counter over that range; it is not the maximum value in the window.

## SRE

Build practical understanding of:

- SLI
- SLO
- SLA
- error budget
- alert quality
- burn rate
- toil
- reliability

## Incident investigation

Evolve from selecting a dramatic possible cause to prioritizing the hypothesis best supported by the observed signals.

---

# Reassessment Points

Repeat a shorter assessment after:

- Module 04
- Module 10
- Module 16
- Module 20
- Module 24

The goal is to measure improvement in mental models and independent troubleshooting, not test memorization.