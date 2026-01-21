---
title: Design Experiments That Discriminate Hypotheses
tags: experiments, hypotheses, baselines, ablations, methodology
description: Prefer experiments that strongly distinguish competing explanations and include strong baselines and ablations.
---

## Design Experiments That Discriminate Hypotheses

Good experiments create outcomes that differ significantly depending on which hypothesis is true.

### What to do

1. List plausible hypotheses.
2. Design experiments where expected results differ across hypotheses.
3. Ensure reliability (repeatability, noise estimates, implementation confidence).
4. Use **strong baselines** and **ablations**.

### Baselines (critical)

A common mistake is showing “decent” results instead of showing “better than plausible alternatives.”

- Compare against strong alternatives people would actually use.
- Put effort into tuning baselines (hyperparams, prompts, scaffolding).

### Ablations (critical)

If a method has parts A/B/C:

- baseline
- A only, B only, C only
- combinations as needed
  so readers can see what matters.

### Checklist

- What alternative explanation would make this result uninteresting?
- Is there a decisive experiment that would change my mind?
- Are baselines tuned as carefully as the proposed method?
- Can readers identify which component caused the gain?

### Common failure modes

- Many experiments that don’t distinguish hypotheses
- Weak baselines
- No ablations for multi-part methods
