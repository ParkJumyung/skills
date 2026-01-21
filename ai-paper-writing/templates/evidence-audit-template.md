---
title: Evidence Audit Template
tags: template, evidence, red-teaming, rigor, experiments
description: Fill-in template to map claims to evidence, identify vulnerabilities, and plan decisive follow-up experiments.
---

## Evidence Audit Template

Use this to stress-test whether the evidence genuinely supports the narrative and survives skeptical scrutiny.

### How to use

- For each claim, list evidence and actively search for:
  - confounds
  - bugs
  - alternative explanations
  - weak baselines
  - missing ablations
- Prefer at least one “hard to deny” experiment per claim.

### Fill-in

## Claim 1

- Claim:
- Strength level (existence/systematic/hedged/narrow/guarantee):
- Scope:
- What would falsify it?

### Evidence items (1–3)

1. **Experiment / analysis name:**
   - Hypotheses it discriminates:
   - Key result (include numbers if possible):
   - Baselines used (and tuning effort):
   - Ablations:
   - Reliability risks (bugs/leakage/confounds/noise):
   - Strongest alternative explanation:
   - Best replication / alternate pathway check:
   - “Kill shot” follow-up test:

2. (repeat)
3. (repeat)

## Claim 2 (optional)

- (repeat structure)

## Claim 3 (optional)

- (repeat structure)

## Top vulnerabilities (ranked)

1.
2.
3.
4.
5.

## Patch plan (next experiments)

- Experiment:
- What it would clarify:
- Expected outcomes under competing hypotheses:
- Cost (time/compute) and priority:
