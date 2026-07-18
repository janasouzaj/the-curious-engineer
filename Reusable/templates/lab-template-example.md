# Lab XX — <Lab Title>

---

# Goal

What am I trying to understand? Describe the objective of this lab in one or two paragraphs.

**Examples:**
- Understand how the Linux boot process works.
- Investigate how DNS resolution happens inside a Kubernetes Pod.
- Observe how prometheus discovers new targets.

---

# Background

Briefly explain the concept behind this experiment.

- Why is this important?
- Where is it used in real-world environments?
- What problem does it solve?

---

# Environment

| Component | Details |
|----------|----------|
| Operating System | |
| Distribution | |
| Kernel Version | |
| Infrastructure | |
| Virtualization | |
| Cloud Provider | |
| Kubernetes Version | |
| Docker Version | |
| Tools | |

---

# Prerequisites

- [ ] Required software installed
- [ ] Access to the environment
- [ ] Documentation reviewed
- [ ] Dependencies available

---

# Hypothesis

Before executing the lab, answer:

> **What do I expect to happen?**

Example:

> I expect the linux kernel to load the initramfs before starting systemd.

---

# Procedure

Document every step performed.

## Step 1

Description

```bash
command_here
```

---

## Step 2

Description

```bash
command_here
```

---

## Step 3

Description

```bash
command_here
```

---

# Expected Result

Describe what should happen if everything works correctly.

Example:
- Kernel loads successfully.
- systemd becomes PID 1.
- Login prompt appears.

---

# Observed Result

What actually happened?

Include:
- Terminal output
- Screenshots
- Logs
- Errors
- Unexpected behavior

---

# Analysis

Compare the observed result with your original hypothesis. Questions to answer:
- Was my hypothesis correct?
- Why?
- What happened differently?
- What did I misunderstand?

---

# Lessons Learned

Summarize the most important discoveries.

Example:
- I learned that GRUB is only responsible for loading the kernel.
- systemd does not initialize until after the kernel finishes mounting the root filesystem.
- The kernel can boot without a graphical interface.

---

# Challenges

What was difficult?

- Configuration issues
- Missing dependencies
- Unexpected errors
- Wrong assumptions

---

# Troubleshooting

Document every problem encountered.

| Problem | Cause | Solution |
|----------|-------|----------|
| | | |

---

# Evidence

Attach relevant material.

- Screenshots
- Diagrams
- Terminal output
- Architecture drawings

---

# References

- Books
- Official documentation
- Articles
- Videos

---

# Next Steps

After completing this lab, I should explore:
-
-
-

---

# Completion Checklist

- [ ] Goal achieved
- [ ] Hypothesis validated
- [ ] Commands documented
- [ ] Notes updated
- [ ] Evidence collected
- [ ] References added
- [ ] README reviewed
- [ ] Commit pushed to GitHub

---

# Personal Reflection

Write a few sentences about the experience. Suggested questions:
- What surprised me?
- What concept became clearer?
- What still confuses me?
- If I had to explain this to someone else, could I?

---

**Lab Status**

- [ ] Planned
- [ ] In Progress
- [ ] Completed
- [ ] Reviewed