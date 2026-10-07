# The Curious Engineer Roadmap

> I'm not building a resume. I'm documenting my evolution as an engineer.

This roadmap defines my **24-month journey toward DevOps Engineering with a specialization in Observability**.

The objective is not to collect tools or certificates. The objective is to build engineering depth through **books, official documentation, hands-on labs, troubleshooting, projects, technical writing, and architectural thinking**.

---

# North Star

```text
Engineering Foundations
        ↓
DevOps Engineering
        ↓
Observability Engineering
        ↓
SRE / Reliability
        ↓
Platform Engineering
        ↓
Distributed Systems & Architecture
        ↓
Staff / Principal Engineering
        ↓
Observability / Platform Architecture
```

This roadmap is a direction, not a contract. Technology choices can change as the industry and my work evolve.

---

# Learning Principles

### 1. Fundamentals before tools

I want to understand the operating system, network, runtime, storage and failure modes before hiding them behind a platform.

### 2. Build before claiming knowledge

Every major topic should lead to an experiment, lab, project, or troubleshooting exercise.

### 3. Break things intentionally

A controlled failure is often more educational than a successful deployment.

### 4. Evidence over confidence

I should be able to explain how I know something works, not only say that it works.

### 5. Observability starts with the system

Metrics, logs and traces are not the goal. Understanding system behavior is the goal.

### 6. Cost is part of engineering

An observable system must also be economically sustainable. In observability work, ingestion, cardinality, storage, retention and queries are engineering concerns.

---

# Roadmap

| # | Module | Main Focus | Exit Capability |
|---|---|---|---|
| 01 | Linux & Operating Systems | Processes, memory, I/O, filesystem, systemd, /proc, sockets | Investigate common Linux failures using a systems mental model |
| 02 | Computer Networking | DNS, TCP/UDP, HTTP, TLS, routing, sockets | Trace and troubleshoot a network request end-to-end |
| 03 | Git & Shell | Git internals, branching, recovery, Bash, text processing | Recover from common Git mistakes and automate repetitive work |
| 04 | Programming for DevOps | Python, APIs, JSON, automation, basic Go | Build small reliable automation tools |
| 05 | Containers | Images, layers, namespaces, cgroups, networking, storage | Explain and troubleshoot container isolation and runtime behavior |
| 06 | Kubernetes | Pods, controllers, services, scheduling, probes, resources | Diagnose common Kubernetes workload failures |
| 07 | CI/CD | Build, test, security, artifacts, deployment, rollback | Design and implement a production-oriented pipeline |
| 08 | Terraform / IaC | State, resources, modules, drift, lifecycle | Build reproducible infrastructure with controlled change |
| 09 | GitOps | Reconciliation, desired state, drift, promotion | Manage deployment state declaratively |
| 10 | AWS | VPC, EC2, EKS, IAM, ELB, RDS, CloudWatch, cost | Operate cloud infrastructure with reliability and cost awareness |
| 11 | Observability Fundamentals | Metrics, logs, traces, telemetry, cardinality, RED/USE | Explain what makes a system observable |
| 12 | Prometheus & PromQL | Time series, labels, scraping, recording rules, histograms, queries | Build and interpret meaningful PromQL |
| 13 | Grafana | Dashboards, Explore, variables, correlation, alerting | Design dashboards that support investigation and decisions |
| 14 | OpenTelemetry | API/SDK, OTLP, instrumentation, Collector, context | Design vendor-neutral telemetry pipelines |
| 15 | Alloy & Telemetry Pipelines | Discovery, collection, processing, filtering, routing, export | Reason about telemetry flow and optimization end-to-end |
| 16 | Logs & Tracing | Loki, LogQL, Tempo, trace context, correlation | Investigate incidents across metrics, logs and traces |
| 17 | SRE Fundamentals | Reliability, SLI, SLO, SLA, toil, error budgets | Apply core SRE concepts to a service |
| 18 | SLOs & Alerting | Symptom alerts, burn rates, alert quality, noise | Design alerts around user impact and reliability objectives |
| 19 | Incident Management | Detection, triage, mitigation, postmortems, action items | Lead a structured technical incident investigation |
| 20 | Performance & Capacity | Saturation, queues, latency, DBs, connection pools, capacity | Diagnose performance problems and reason about capacity |
| 21 | Distributed Systems | Consistency, replication, partitioning, retries, timeouts, failure | Explain distributed-system trade-offs and failure modes |
| 22 | Platform Engineering | Developer experience, golden paths, self-service, platform APIs | Explain how a platform reduces developer cognitive load |
| 23 | Software Architecture | Trade-offs, architecture characteristics, ADRs, RFCs | Make and communicate architecture decisions |
| 24 | Capstone — Observability Platform | Integration of the complete journey | Design, build, operate, document and defend an observability platform |

---

# Phase 1 — Engineering Foundations

## Modules 01–04

### 01 — Linux & Operating Systems

Core topics:

- kernel and user space
- processes and threads
- CPU and load average
- memory
- filesystem
- I/O
- permissions
- file descriptors
- `/proc`
- systemd
- journald
- sockets
- troubleshooting

---

### 02 — Computer Networking

Core topics:

- TCP/IP
- DNS
- ports and sockets
- TCP handshake
- UDP
- routing
- NAT
- TLS
- HTTP
- proxies
- load balancers

---

### 03 — Git & Shell

Core topics:

- Git object model
- branches
- merge and rebase
- reset/revert
- stash
- cherry-pick
- reflog
- Bash
- pipes
- redirection
- grep/find/sed/awk/xargs

Deliverable:

**DevOps Shell Toolkit**

---

### 04 — Programming for DevOps

Primary language:

**Python**

Secondary language:

**Go**

Topics:

- automation
- APIs
- JSON/YAML
- subprocesses
- files
- error handling
- testing
- command-line interfaces

---

# Phase 2 — DevOps Core

## Modules 05–10

Focus:

```text
Containers
      ↓
Kubernetes
      ↓
CI/CD
      ↓
Terraform
      ↓
GitOps
      ↓
AWS
```

The objective is to understand the system underneath the platform, not simply memorize commands.

---

# Phase 3 — Observability Engineering

## Modules 11–16

This is the main specialization track.

```text
System
  ↓
Telemetry
  ↓
Collection
  ↓
Processing
  ↓
Storage
  ↓
Query
  ↓
Visualization
  ↓
Alerting
  ↓
Investigation
```

Topics include:

- metrics
- logs
- traces
- time series
- labels
- cardinality
- instrumentation
- PromQL
- histograms
- OpenTelemetry
- Alloy
- Grafana
- Loki
- Tempo
- Mimir

---

# Cross-Cutting Track — Observability Cost Engineering

This is not a separate month. It runs alongside Modules 11–16.

```text
Application
   ↓
Telemetry generation
   ↓
Instrumentation
   ↓
Collection
   ↓
Filtering / transformation
   ↓
Ingestion
   ↓
Storage / retention
   ↓
Query
   ↓
Visualization / alerting
   ↓
Cost
```

Questions to ask:

- Which telemetry has real operational value?
- Where is cardinality exploding?
- Are high-cardinality labels being generated?
- Are we collecting redundant data?
- What is the collection frequency?
- How much data is ingested?
- How long is it retained?
- Which queries are expensive or excessive?
- Which telemetry could be filtered, sampled or aggregated?
- Does the cost match the value?

---

# Phase 4 — Reliability Engineering

## Modules 17–20

```text
Observability
      ↓
Reliability
      ↓
SLOs
      ↓
Alerting
      ↓
Incidents
      ↓
Performance
```

The emphasis shifts from:

> "Can I see the system?"

to:

> "Can I know whether users are being affected, detect it quickly, mitigate it safely, and learn from it?"

---

# Phase 5 — Systems, Platforms & Architecture

## Modules 21–23

Focus:

- distributed systems
- failure modes
- consistency
- scalability
- platform boundaries
- developer experience
- internal platforms
- architecture decisions
- trade-offs
- ADRs
- RFCs
- technical direction

---

# Phase 6 — Capstone

## Module 24 — Observability Platform

Target architecture:

```text
Applications
      ↓
OpenTelemetry
      ↓
Grafana Alloy
      ├── Metrics → Prometheus / Mimir
      ├── Logs → Loki
      └── Traces → Tempo
                    ↓
                 Grafana
                 /     \\
              Alerts   SLOs
```

The capstone must document:

- architecture
- telemetry flow
- instrumentation
- data lifecycle
- cardinality strategy
- retention
- alerting
- SLOs
- troubleshooting
- failure modes
- security considerations
- scalability
- operational model
- cost model
- trade-offs
- ADRs
- runbooks

---

# Exit Criteria

By the end of the journey, the evidence should show that I can:

### Operate

Run and troubleshoot Linux, containers, Kubernetes and cloud infrastructure.

### Automate

Build repeatable workflows using Bash, Python, Go, Terraform and GitOps.

### Observe

Instrument, collect, query, correlate and visualize metrics, logs and traces.

### Investigate

Use telemetry to formulate and validate hypotheses during incidents.

### Improve reliability

Define SLOs, design actionable alerts and reduce operational noise.

### Design

Reason about distributed systems, platforms and architectural trade-offs.

### Communicate

Write clear technical documentation, ADRs, RFCs, incident reports and architecture diagrams.

---

# Definition of Done for the Repository

This repository is successful when it contains evidence of capability, not when every checkbox is green.

The final body of work should include:

- technical notes
- books and reading notes
- official documentation references
- hands-on labs
- intentionally broken systems
- troubleshooting guides
- automation scripts
- Terraform
- Kubernetes manifests
- dashboards
- PromQL examples
- telemetry pipelines
- incident simulations
- SLO definitions
- architecture diagrams
- ADRs
- RFCs
- technical articles
- project documentation
- personal reflections

The repository is not meant to be finished.

It is meant to evolve.