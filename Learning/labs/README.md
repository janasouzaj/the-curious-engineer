# Labs

> To think: Theory tells you how things should work. Labs show you how they actually behave.

Welcome to the **Labs** section of **The Curious Engineer**. This directory contains all hands-on experiments completed throughout my "Platform Engineering & Observability Residency". The goal isn't simply to follow tutorials, it's to explore, break, troubleshoot, document, and truly understand how modern systems work.

---

# Objectives

Each lab is designed to answer one simple question: "What happens if...?". Rather than memorizing commands, every experiment aims to understand the behavior behind the technology.

Examples:
- What happens if the kernel can't find `init`?
- What happens when a pod loses network connectivity?
- How does prometheus behave when a target disappears?
- What happens if etcd becomes unavailable?
- How does loki react when storage becomes unavailable?

Curiosity drives every lab.

---

# Every Lab Contains

Every experiment follows the same structure:

```text
01-lab000/

README.md
commands.sh
notes.md
assets/
```

---

# Lab Workflow

Every experiment follows the same process:

```text
Read
↓
Prepare
↓
Execute
↓
Break Something
↓
Investigate
↓
Fix
↓
Document
↓
Reflect
```

Learning happens during troubleshooting, not when everything works.

---

# Rules

Every lab must be:
- Reproducible
- Documented
- Version controlled
- Based on official documentation
- Focused on understanding

No copy-and-paste, no magic. If I can't explain it, I don't understand it.