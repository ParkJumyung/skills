---
name: ai-paper-writing
description: Modular toolkit for writing and reviewing AI papers: compress to 1–3 claims, motivate impact, position novelty, design/red-team evidence, and structure abstract/intro/figures/main body. Use when drafting, revising, or reviewing AI research papers.
---

# AI Paper Writing

A modular skill bundle distilled from “Highly Opinionated Advice on How to Write AI Papers” (Neel Nanda).  
The goal is to help you produce papers where readers **understand**, **remember**, and **believe** the narrative.

## North star

An ideal paper is a short, rigorous, evidence-based technical story with a takeaway the reader cares about:

- **What?** 1–3 concrete claims that contribute to knowledge
- **Why?** rigorous evidence that supports the claims
- **So what?** motivation + impact: why the reader should care

## How to use

Pick a workflow below, or jump straight to a module. Each module is independent.

### Common inputs

- Your paper text (or section)
- Or: a project summary + key results + experiments list

### Common outputs

- claim list (1–3 claims + scope + confidence level)
- evidence map (claim → experiments → risks)
- rewritten abstract/intro
- experiment fixes (baselines, ablations, stronger discriminators)
- figure + caption guidance
- limitations + discussion guidance

---

## Workflows

### A) Drafting from scratch (recommended order)

1. [Compress to claims](modules/01-compress-to-claims.md)
2. [Motivation & impact](modules/02-motivation-impact.md)
3. [Novelty & positioning](modules/03-novelty-positioning.md)
4. [Evidence & red-teaming](modules/04-evidence-redteaming.md)
5. [Paper structure overview](modules/00-overview.md)
6. [Abstract](modules/07-structure-abstract.md)
7. [Introduction](modules/08-structure-introduction.md)
8. [Figures](modules/09-figures.md)
9. [Main body layering](modules/10-main-body.md)
10. [Discussion & limitations](modules/12-discussion-limitations.md)
11. [Related work](modules/11-related-work.md)

### B) Reviewing a draft

1. [Compress to claims](modules/01-compress-to-claims.md) (extract what the paper _actually_ claims)
2. [Evidence & red-teaming](modules/04-evidence-redteaming.md)
3. [Avoid misleading evidence](modules/06-avoid-misleading.md)
4. [Abstract](modules/07-structure-abstract.md)
5. [Introduction](modules/08-structure-introduction.md)
6. [Common pitfalls](modules/14-common-pitfalls.md)

### C) Strengthening experiments

1. [Experiments design](modules/05-experiments-design.md)
2. [Baselines + ablations](modules/05-experiments-design.md#baselines--ablations)
3. [Avoid misleading evidence](modules/06-avoid-misleading.md)
4. [Evidence & red-teaming](modules/04-evidence-redteaming.md)

### D) Tightening narrative + clarity

1. [Compress to claims](modules/01-compress-to-claims.md)
2. [Motivation & impact](modules/02-motivation-impact.md)
3. [Abstract](modules/07-structure-abstract.md)
4. [Introduction](modules/08-structure-introduction.md)
5. [Definitions & layering](modules/10-main-body.md)

---

## Templates

- [Abstract template](templates/abstract-template.md)
- [Intro template](templates/intro-template.md)
- [Paper outline template](templates/paper-outline-template.md)
- [Evidence audit template](templates/evidence-audit-template.md)
- [Figure caption template](templates/figure-caption-template.md)

---

## Modules index

- [00 Overview](modules/00-overview.md)
- [01 Compress to claims](modules/01-compress-to-claims.md)
- [02 Motivation & impact](modules/02-motivation-impact.md)
- [03 Novelty & positioning](modules/03-novelty-positioning.md)
- [04 Evidence & red-teaming](modules/04-evidence-redteaming.md)
- [05 Experiments design](modules/05-experiments-design.md)
- [06 Avoid misleading evidence](modules/06-avoid-misleading.md)
- [07 Structure: Abstract](modules/07-structure-abstract.md)
- [08 Structure: Introduction](modules/08-structure-introduction.md)
- [09 Figures](modules/09-figures.md)
- [10 Main body](modules/10-main-body.md)
- [11 Related work](modules/11-related-work.md)
- [12 Discussion & limitations](modules/12-discussion-limitations.md)
- [13 Writing process](modules/13-writing-process.md)
- [14 Common pitfalls](modules/14-common-pitfalls.md)
- [15 Checklists](modules/15-checklists.md)

---

## Acknowledgements

This was compiled from Neel Nanda's article (Highly Opinionated Advice on How to Write AI Papers)[https://www.alignmentforum.org/s/5GT3yoYM9gRmMEKqL/p/eJGptPbbFPZGLpjsp]

---

## metadata.json

---

_Source: `metadata.json`_

```json
{
  "version": "1.0.0",
  "organization": "Jumyung Park",
  "date": "January 2026",
  "abstract": "A modular, rule-based guide for writing and reviewing machine learning research papers, distilled from highly opinionated best practices from Neel Nanda. Designed for AI agents and LLM-assisted workflows, this skill emphasizes narrative clarity, precise claims, rigorous experimental evidence, and scientific integrity. The repository is structured as independent rules and templates covering claim compression, motivation and impact, novelty positioning, experiment design and red-teaming, paper structure (abstract, introduction, figures, main body), limitations, and iterative writing process. Optimized for truth-seeking, reader comprehension, and reproducibility rather than hype or conference-driven incentives.",
  "references": [
    "https://www.alignmentforum.org/posts/eJGptPbbFPZGLpjsp/highly-opinionated-advice-on-how-to-write-AI-papers"
  ]
}
```

---

## Modules

---

The following modules are included in sorted order.

---

## modules/00-overview.md

---

_Source: `modules/00-overview.md`_

---

title: The Paper Is a Narrative
tags: narrative, claims, evidence, impact, structure
description: Treat the paper as a short, evidence-backed story built around 1–3 claims with a clear takeaway the reader cares about.

---

## The Paper Is a Narrative

An ideal AI paper is a short, rigorous, evidence-based technical story with a takeaway the reader cares about.

### What to do

Build the entire paper around:

- **What?** 1–3 concrete claims (your contribution to knowledge)
- **Why?** rigorous evidence that supports those claims
- **So what?** motivation + impact (why a reader should care)

Everything else exists to support this narrative.

### Reader reality

Many readers only see:
**title → abstract → intro/figures skim → stop**.

So optimize for:

- clarity of narrative
- credibility of evidence
- memorability of takeaway

### Checklist

- Can I state the paper’s narrative in 2–5 sentences?
- Are there 1–3 explicit claims?
- Does every major section support the claims?
- Do the abstract + intro + figures stand alone as a coherent summary?
- Is the evidence strong enough for a skeptical reader?

---

## modules/01-compress-to-claims.md

---

_Source: `modules/01-compress-to-claims.md`_

---

title: Compress Your Work Into 1–3 Claims
tags: narrative, claims, scoping, writing-process
description: Distill the project into 1–3 concrete, scoped claims with an explicit strength level and falsification conditions.

---

## Compress Your Work Into 1–3 Claims

A paper’s narrative is fundamentally a contribution to our body of knowledge: **one to three specific claims** that fit a cohesive theme.

### What to do

1. Write a raw list of what you learned.
2. Choose the 1–3 most important items:
   - most exciting or important
   - hardest / most non-trivial
   - likely to matter to others
3. Turn each into a crisp claim with **scope** and **strength**.
4. State what would falsify each claim.

### Claim strength ladder (pick one)

- **Existence proof:** “We found at least one example where X happens.”
- **Systematic:** “X generally happens across a wide range of contexts.”
- **Hedged:** “There is suggestive/compelling/tentative evidence that X is true.”
- **Narrow:** “X is best in situations V/W for objective Y.”
- **Guarantee:** “X is always true.” (rare in deep learning)

### Claim template

- **Claim:** …
- **Scope:** models/tasks/data/regimes …
- **Strength:** existence/systematic/hedged/narrow/guarantee
- **Falsifier:** what result would make me retract/modify it?
- **Key evidence:** 1–3 experiments/analyses

### Common failure modes

- Too many claims (grab-bag paper)
- Vague claims (“improves performance” without scope/metric)
- Strong claims with weak evidence (overclaiming)

---

## modules/02-motivation-impact.md

---

_Source: `modules/02-motivation-impact.md`_

---

title: Make the Reader Care
tags: motivation, impact, framing, takeaway
description: Explicitly connect claims to context, the problem, and a takeaway that matters.

---

## Make the Reader Care

Your narrative needs motivation and impact. Always answer: **Why should anyone care?**

### What to do

For each claim, write three pieces:

1. **Context:** Where does this sit in AI / why this topic is real?
2. **Need/gap:** What’s unknown, missing, or wrong?
3. **Impact:** What changes if your claim is true? Who should update beliefs or behavior?

### Output template

- **Motivation (context):** …
- **Problem / gap:** …
- **Impact / takeaway:** …
- **Who cares:** …

### Checklist

- Is motivation specific (not generic “X is important”)?
- Does impact follow from the actual claim, not vibes?
- Could a reader repeat the takeaway in one sentence?

### Common failure modes

- Generic framing, no concrete gap
- Impact not tied to evidence scope
- Overselling implications without limitations

---

## modules/03-novelty-positioning.md

---

_Source: `modules/03-novelty-positioning.md`_

---

title: Be Explicit About What’s Novel
tags: novelty, positioning, citations, related-work, professionalism
description: Clearly label what is new, what builds on prior work, and why the contribution expands knowledge.

---

## Be Explicit About What’s Novel

Novelty means your work expands our knowledge. Make it easy for readers (and reviewers) to tell what changed because of your paper.

### What to do

1. Identify the closest prior work (top 5).
2. For each prior work:
   - what they showed
   - what you reuse/build on
   - what you do differently
   - why that difference matters
3. In the intro, explicitly label:
   - **Builds on:** …
   - **Novel contribution:** …
4. If criticizing prior work:
   - stay professional
   - specify the flaw and why it matters
   - show how your method resolves it

### Novelty test

Ask:  
“Should a reader assign different probabilities to propositions they care about after seeing these results?”

### Output template

- **Novelty bullets:**
  - Novel: …
  - Builds on: …
  - Differs from: …
- **Closest-work map:** paper → overlap → difference → why it matters

### Common failure modes

- Reader can’t tell what’s new
- Claims sound arrogant or undersell
- Missing key citations to closest work

---

## modules/04-readteaming.md

---

_Source: `modules/04-readteaming.md`_

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

---

## modules/05-experiments-design.md

---

_Source: `modules/05-experiments-design.md`_

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

---

## modules/06-avoid-misleading.md

---

_Source: `modules/06-avoid-misleading.md`_

---

title: Avoid Cherry-Picking and Post-Hoc Storytelling
tags: rigor, cherry-picking, post-hoc, qualitative, bias
description: Prevent selection bias and overinterpretation by documenting selection, tracking pre/post-hoc analysis, and testing alternatives.

---

## Avoid Cherry-Picking and Post-Hoc Storytelling

Evidence can look more compelling than it is if selection bias or post-hoc narratives creep in.

### What to do

#### Qualitative examples

- State selection method.
- Prefer random/context examples when possible.
- Exception: existence proof claims (one trustworthy example can suffice).

#### Pre vs post-hoc tracking

- Mark which experiments were planned before the claim vs after.
- Treat post-hoc interpretations as weaker evidence.

#### Alternative explanations

Ask: “Could the evidence be true but the claim false?”  
If yes, add tests to distinguish.

### Checklist

- Are examples cherry-picked?
- Did we clearly label post-hoc analyses?
- Could the same pattern arise from a confound?
- Did we add sanity checks?

### Common failure modes

- “Best examples only” presented as representative
- Post-hoc discoveries written like predictions
- Correct prediction for the wrong reason

---

## modules/07-structure-abstract.md

---

_Source: `modules/07-structure-abstract.md`_

---

title: Write an Abstract That Stands Alone
tags: abstract, structure, narrative, clarity, cold-start
description: Use a sentence-role structure to orient cold-start readers, state claims, evidence, and impact with minimal jargon.

---

## Write an Abstract That Stands Alone

The abstract is the highest-leverage part of the paper. Many readers won’t go further.

### What to do

Use sentence roles:

1. **Context:** what subfield / topic and why it’s real.
2. **Gap/need:** what’s unknown/problematic.
3. **Core contribution/claim:** what you show + why it’s exciting.
4. **Clarifier (optional):** definition or how evidence connects.
   5–N. **Evidence + secondary claims:** 1 sentence per idea; include a concrete metric/result if possible.
   Final 1–2. **Impact:** takeaway, implications, standard of evidence.

### Checklist

- Would a cold-start reader know the “genre” of the paper?
- Are claims explicit (not implied)?
- Is there at least one concrete result/metric (when applicable)?
- Is jargon minimized or defined?

### Common failure modes

- Too technical too early
- No clear claim
- No evidence
- No impact/takeaway

---

## modules/08-structure-introduction.md

---

_Source: `modules/08-structure-introduction.md`_

---

title: Write an Introduction That Summarizes the Whole Paper
tags: introduction, structure, contributions, novelty, motivation
description: Treat the intro as an extended abstract: claims, motivation, novelty, key evidence, and impact, plus contribution bullets.

---

## Write an Introduction That Summarizes the Whole Paper

The introduction should be a self-contained narrative summary. Don’t fear repetition.

### What to do

Suggested flow:

1. **Context + motivating question + why it matters** (cite liberally).
2. **Technical background + why current approaches are inadequate** (cite).
3. **Main claim + nuance + novelty labeling** (novel vs builds-on).
   3.5 **The case:** the most critical evidence in brief.
   (Optional) repeat for claim 2/3.
4. **Impact:** implications, who should care, what changes.
   End with **contribution bullets** (claims + brief evidence pointers).

### Checklist

- Could a reader stop after the intro and still get the narrative?
- Is novelty explicitly labeled?
- Is key evidence summarized (not deferred)?
- Are key terms defined or signposted?

### Common failure modes

- Intro doesn’t say what’s new
- Intro motivates but doesn’t summarize evidence
- Assumes too much reader context

---

## modules/09-figures.md

---

_Source: `modules/09-figures.md`_

---

title: Make Figures Communicate the Takeaway
tags: figures, visualization, captions, results-communication
description: Design figures around a single takeaway and write captions that enable standalone interpretation.

---

## Make Figures Communicate the Takeaway

Figures are a primary channel for communicating results. Put serious effort into them.

### What to do

For each figure:

1. Decide the **takeaway** (one sentence).
2. Choose a visualization that emphasizes the takeaway.
3. Make interpretation easy:
   - readable axes/ticks
   - clear legend
   - annotation/highlighting for key lines/patterns
4. Write a caption that includes:
   - what is shown
   - experimental conditions
   - how to interpret
   - caveats if needed

### Checklist

- If someone only sees the figure + caption, do they get the point?
- Is the plotted quantity tied to a claim?
- Are the conditions and baselines clear?

### Common failure modes

- Figure shows numbers but no message
- Caption lacks setup/conditions
- Visual clutter hides the key effect

---

## modules/10-main-body.md

---

_Source: `modules/10-main-body.md`_

---

title: Layer Technical Detail So Readers Can Verify
tags: main-body, methods, results, definitions, reproducibility
description: Present results at multiple abstraction levels and include enough detail to replicate and interpret correctly.

---

## Layer Technical Detail So Readers Can Verify

The main body is where you justify claims to an engaged skeptical reader.

### What to do

#### Layering principle

- high-level in abstract/intro
- results in figures
- increasing technical detail in main body + appendix

#### Define key terms

Readers have less context than you think. Err toward defining:

- key techniques
- key terms
- setup details that affect interpretation

#### Default structure

- **Background:** context, terminology, crucial techniques
- **Methods:** what you did + why it’s relevant
- **Results:** how methods were applied; what happened; interpretation

### Checklist

- Could someone reproduce the core results from the description?
- Are all crucial choices specified (data, models, metrics, preprocessing)?
- Are definitions placed where readers need them?

### Common failure modes

- Missing details that change interpretation
- Readers can’t replicate
- Sections that don’t support claims

---

## modules/11-related-work.md

---

_Source: `modules/11-related-work.md`_

---

title: Use Related Work to Clarify Differences
tags: related-work, citations, positioning, professionalism
description: Cover only genuinely relevant work and explain overlap vs difference clearly; keep tone professional when critiquing.

---

## Use Related Work to Clarify Differences

Related work exists to help readers understand how your paper fits into the literature.

### What to do

- Focus on the closest work and explain:
  - what they did
  - what you share
  - what you do differently
  - why it matters
- If your work fixes a flaw:
  - state politely
  - specify the flaw and its consequence
  - explain how you resolve it

### Checklist

- Are the closest neighbors covered?
- Is “difference” explicit or implied?
- Does the reader know what to cite you for?

### Common failure modes

- Citation laundry list without clarity
- Defensive or personal critique tone

---

## modules/12-discussion-limitations.md

---

_Source: `modules/12-discussion-limitations.md`_

---

title: State Limitations to Calibrate Belief
tags: limitations, discussion, integrity, calibration, future-work
description: Tie limitations directly to claim strength and evidence scope, and state implications without overclaiming.

---

## State Limitations to Calibrate Belief

Readers must understand limitations to correctly update beliefs.

### What to do

1. List the biggest limitations:
   - evidence scope
   - confounds
   - generalization gaps
2. For each limitation:
   - how it affects claim strength
   - what experiment would reduce it
3. If useful, discuss broader implications and future work.

### Checklist

- Are limitations specific and tied to claims?
- Should any claim be hedged or narrowed given limitations?
- Did we avoid hype and clearly calibrate confidence?

### Common failure modes

- Hiding limitations to sound exciting
- Generic limitations that don’t change interpretation

---

## modules/13-writing-process.md

---

_Source: `modules/13-writing-process.md`_

---

title: Write Iteratively: Compress Then Expand
tags: writing-process, outlining, iteration, feedback
description: Use an iterative pipeline (abstract → bullets → outline → draft → edit) and get feedback early to fight the illusion of transparency.

---

## Write Iteratively: Compress Then Expand

Writing is part of research. It clarifies thinking and exposes gaps.

### What to do

#### Compress

- Explain the work to someone; ask what’s most interesting.
- Plan a talk.
- Have an LLM summarize notes, then critique it.
  Iterate until you have:
- 1–3 claims
- why they matter
- 1–3 key experiments per claim

#### Expand (recommended sequence)

1. Abstract draft
2. Bullet narrative
3. Intro bullet outline
4. Full paper outline
5. Figures draft
6. Prose draft
7. Edit aggressively; repeat

#### Feedback strategy

Get feedback early on narrative/outline (fast to critique), not only on dense prose.

### Checklist

- Did I write the abstract early and iterate?
- Did I outline before drafting prose?
- Did I get feedback at each stage?

### Common failure modes

- Writing treated as an afterthought
- Illusion of transparency (assuming reader context)

---

## modules/14-common-pitfalls.md

---

_Source: `modules/14-common-pitfalls.md`_

---

title: Avoid the Classic Paper-Writing Traps
tags: pitfalls, publishability, clarity, verbosity, tacit-knowledge
description: Don’t optimize for hype, complexity, or conference vibes at the expense of truth, clarity, and useful knowledge transfer.

---

## Avoid the Classic Paper-Writing Traps

### Trap: obsessing over publishability

Peer review rewards shininess and familiarity. Prefer scientific value; wrap for conference norms at the end if needed.

### Trap: unnecessary complexity and verbosity

If readers don’t understand, they ignore it (or assume it’s BS). Use plain language and keep jargon only where it increases precision.

### Trap: not prioritizing writing

Your work only matters if people understand it. Iterate on abstract/intro/figures early.

### Trap: discarding tacit knowledge

Troubleshooting, “what broke,” replication tips, and intuitions are often valuable. Put them in:

- appendix A
- companion blog post

### Checklist

- Did I simplify language without losing precision?
- Did I explicitly calibrate claims and limitations?
- Did I preserve high-value tacit knowledge somewhere?

---

## modules/15-checklists.md

---

_Source: `modules/15-checklists.md`_

---

title: Paper Writing Checklists
tags: checklists, review, narrative, evidence, clarity, integrity
description: Quick checklists for narrative, evidence, clarity, integrity, and process to apply during drafting and review.

---

## Paper Writing Checklists

### Narrative

- Can I state the paper’s narrative in 2–5 sentences?
- Are there 1–3 concrete claims?
- Do claims fit a cohesive theme?

### Evidence

- For each claim: 1–3 key experiments?
- Do experiments discriminate hypotheses?
- Are baselines strong and tuned?
- Are there ablations for multi-part methods?
- Did we red-team bugs/confounds?

### Clarity

- Are key terms defined?
- Does intro summarize claims + evidence + novelty + impact?
- Do figures + captions stand alone?

### Integrity

- Are limitations explicit and tied to claims?
- Am I informing rather than persuading?
- Did I avoid cherry-picking or disclose selection?
- Did I mark post-hoc vs pre-specified?

### Process

- Did I iterate: abstract → outline → draft → edit?
- Did I get feedback early?

---

## Templates

---

The following templates are included in sorted order.

---

## templates/abstract-template.md

---

_Source: `templates/abstract-template.md`_

---

title: Abstract Template
tags: template, abstract, narrative, cold-start
description: Fill-in template for a cold-start abstract that states context, gap, claims, evidence, and impact with minimal jargon.

---

## Abstract Template

Use this to draft an abstract that stands alone for readers who stop after the abstract.

### How to use

- Keep **1 sentence per idea**.
- Prefer **simple language**; define or avoid jargon.
- Include at least **one concrete result/metric** when applicable.

### Fill-in

1. **Context (1 sentence):**  
   _(What area of AI? What’s uncontroversially true / established?)_
   - …

2. **Gap / need (1 sentence):**  
   _(What’s unknown, missing, or problematic?)_
   - …

3. **Core contribution / claim (1 sentence):**  
   _(What do you show? Why is it notable?)_
   - …

4. **Clarifier / definition (optional, 1 sentence):**  
   _(Define key term or clarify claim meaning if needed.)_
   - …

5. **Key evidence (1–3 sentences, 1 idea each):**  
   _(Summarize the strongest experimental evidence; include a metric if possible.)_
   - …
   - …
   - …

6. **Impact / takeaway (1–2 sentences):**  
   _(Why should the reader care? What changes if this is true?)_
   - …
   - …

### “Remember this” (1–2 sentences)

- …

---

## templates/evidence-audit-template.md

---

_Source: `templates/evidence-audit-template.md`_

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

---

## templates/figure-caption-template.md

---

_Source: `templates/figure-caption-template.md`_

---

title: Figure and Caption Template
tags: template, figures, captions, results-communication
description: Fill-in template to design a figure around a single takeaway and write a caption that supports standalone interpretation.

---

## Figure and Caption Template

Use this to ensure every figure has a clear purpose and the caption provides enough context to interpret it without hunting through the paper.

### How to use

- Start with the takeaway sentence.
- Describe what is plotted and the experimental conditions.
- Explain how to interpret the pattern and any caveats.

### Fill-in

## Figure takeaway (1 sentence)

- …

## What is plotted

- X axis:
- Y axis:
- Lines/groups/markers:
- Metric definition (if nonstandard):
- Experimental conditions (model/data/setup):

## What the reader should notice

- Primary pattern:
- Secondary pattern (optional):
- What would contradict the intended interpretation:

## Caption draft

Figure X: …

- What is shown:
- Conditions/setup:
- Interpretation guidance:
- Caveats/limitations:

---

## templates/intro-template.md

---

_Source: `templates/intro-template.md`_

---

title: Introduction Template
tags: template, introduction, contributions, novelty, motivation
description: Fill-in template for an introduction that functions as an extended abstract: claims, novelty, evidence summary, and impact.

---

## Introduction Template

Use this to draft an introduction that communicates the full narrative even if readers stop after the intro.

### How to use

- The intro should answer: **What? Why? So what?**
- Explicitly label **novel vs builds-on**.
- End with **contribution bullets** readers can skim.

### Fill-in

## P1 — Context & motivating question

_(What topic, what question, why it matters? Cite liberally.)_

- Topic:
- Motivating question:
- Why it matters:
- Key citations:

## P2 — Technical background & why current approaches are inadequate

_(What’s known? What’s missing? Why is this hard?)_

- Established facts/approaches:
- What’s inadequate / missing:
- Key citations:

## P3 — Main claim + nuance + novelty labeling

_(State claim clearly. Clarify scope. Mark novelty.)_

- Main claim:
- Scope (models/tasks/regimes):
- Novel vs builds-on:
  - Builds on:
  - Novel contribution:

## P3.5 — The case (evidence summary)

_(Summarize the most critical evidence in brief.)_

- Evidence 1:
- Evidence 2:
- Evidence 3:

## (Optional) P4/P5 — Additional claims + brief evidence

- Claim 2 + evidence:
- Claim 3 + evidence:

## Final — Impact

_(What should the reader take away? Who should care? What changes?)_

- Takeaway:
- Implications:
- Who should update beliefs or behavior:

## Contributions (bullets)

_(Concise, skimmable. Claims + brief evidence pointers.)_

- …
- …
- …

---

## templates/paper-outline-template.md

---

_Source: `templates/paper-outline-template.md`_

---

title: Paper Outline Template
tags: template, outline, structure, methods, results, reproducibility
description: Fill-in template for a tight paper outline where every section supports the narrative and claims.

---

## Paper Outline Template

Use this to plan a paper where each section has a clear role in supporting 1–3 claims.

### How to use

- If you can’t answer “what goes wrong if I cut this?”, cut it.
- Layer detail: high-level → figures → body → appendix.

### Fill-in

## Narrative (top-level)

- Claims (1–3):
  1.
  2.
  3.
- Why should the reader care?
- Key evidence per claim (1–3 items each):

## Abstract

- (use Abstract Template)

## Introduction

- (use Introduction Template)

## Background

- Key terms to define:
- Concepts readers may lack context for:
- Minimal necessary prior work:

## Methods

- Experimental setup:
- Models:
- Data:
- Metrics:
- Baselines:
- Implementation details required for replication:

## Results

### Claim 1 results

- Key figure(s):
- Key quantitative results:
- Key qualitative results (if any):
- Sanity checks:

### Claim 2 results (optional)

- …

### Claim 3 results (optional)

- …

## Discussion / Limitations

- Limitations tied to each claim:
- What evidence would strengthen this?
- Broader implications:
- Future work:

## Related work

- Closest papers:
- Overlap vs difference bullets:

## Appendices

- Extra experiment details:
- Extra plots:
- Reproducibility details:
- Tacit knowledge / replication tips:
