---
title: Red-Team Your Evidence
tags: evidence, rigor, red-teaming, reliability, skepticism
description: Stress-test claims against bugs, confounds, noise, and alternative explanations; prioritize decisive experiments.
---

## Red-Team Your Evidence

Experimental evidence is where narratives go to die (or become real). Treat red-teaming as mandatory.

### What to do

Adopt the mindset:

- “There is a bug.”
- “My narrative is wrong.”
- “There is a hole in my argument.”
  Find it before others do.

### Evidence quality principles

- **Quality > quantity:** one hard-to-deny experiment beats many weak ones.
- Experiments should **distinguish hypotheses** (provide Bayesian evidence).
- **Reliability:** how surprised would you be if this is wrong due to bug/noise?
- **Strong baselines:** invest effort in tuning baselines.
- **Ablations** for multi-component methods.

### Evidence audit template (per claim)

- Claim: …
- Evidence items: …
  For each evidence item:
- What hypothesis it distinguishes:
- Strongest alternative explanation:
- Reliability risks:
- What replication/alternate pathway would confirm it:
- Follow-up “kill shot” test:

### Checklist

- If I were a skeptical reviewer, where would I poke first?
- Did we preempt obvious confounds?
- Did we rerun / estimate variance / replicate key results?
- Did we tune baselines seriously?

### Common failure modes

- Elegant narrative supported by fragile evidence
- No tests for confounds that a reviewer will immediately suspect
- Baselines treated as an afterthought
