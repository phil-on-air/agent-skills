---
name: space-expanding-generation
description: Generate structurally different creative candidates and preserve valid divergence instead of collapsing to the safest polished default. Use when the user wants multiple non-paraphrase directions for stories, art, visual concepts, essays, design, research, strategy, or other generative work. Do NOT use for direct single-answer tasks, fact lookup, or execution-only workflows where variance adds no value.
---

# Space-Expanding Generation

Use this skill when you want outputs that widen the possibility space instead of converging on the safest polished default. This is a cross-domain skill. It applies to stories, poems, visual concepts, art direction, essays, research hypotheses, strategic options, software designs, and other generative work.

This version is the **general creative / generative adapter** of the method. If the task is mainly about designing a pipeline, evaluator, workflow, or system that prevents convergence over repeated runs, see the related skill **`software-development/anti-convergence`**.

## Why this exists
Most AI workflows collapse toward:
- familiar structure
- safe legibility
- average taste
- polished but interchangeable outputs

This skill counters that by forcing structural spread, preserving promising anomalies, and selecting from a frontier rather than a single top-1 winner.

## Use when
- You want multiple genuinely different directions, not paraphrases
- The task is creative, exploratory, conceptual, or generative
- A polished default answer would likely be bland
- You want to preserve awkward-but-fertile branches
- You need non-obvious angles, forms, compositions, or frames

Examples:
- short stories, fiction scenes, poems
- art concepts, visual directions, installations, worldbuilding
- essays, scripts, manifestos, positioning
- research ideation, hypothesis generation
- product concepts, strategy options, design directions
- software architecture or implementation exploration

## Do not use when
- Task requires a single direct answer with no benefit from variance
- Fact lookup, format conversion, or mechanical transformation
- Execution of an already-decided plan where exploration adds no value
- Safety-critical tasks requiring the most conservative answer only

## Core rule
Do not ask for "the best version" too early.

Instead:
1. Generate structurally different candidates
2. Identify the real constraints
3. Score validity and novelty separately
4. Preserve promising anomalies
5. Choose from a frontier

## Procedure

### 1. Identify the attractor basin
Ask:
- What default shape will the model fall into here?
- What clichés, templates, or stylistic norms dominate this domain?
- What kind of answer would look good immediately but say nothing new?

### 2. Set the mode
Choose deliberately:
- **Execution** — clean, direct, low-variance
- **Exploration** — search inside the current frame
- **Reframing** — change what the task is really about
- **Adversarial** — surface strong alternatives the default version would suppress

### 3. Generate candidate spread
At minimum, generate:
- **Baseline** — competent default
- **Boundary** — push current frame to its limit
- **Cross-domain** — import structure from another field or medium
- **Reframe** — redefine the problem or artistic premise
- **Anomaly** — the strangest candidate that still feels alive

Important: differences must be structural, not cosmetic.

### 4. Define constraints
Separate:
- **Hard constraints** — what must hold
- **Soft constraints** — what improves the work
- **Conventions** — what is merely familiar

Examples:
- fiction: coherence, character integrity, tonal control
- visual work: composition, motif discipline, medium constraints
- essay work: thesis pressure, factual accuracy, sentence control
- code: tests, contracts, clarity, performance

### 5. Score two axes
#### Validity
- coherence
- integrity
- constraint fit
- usefulness or artistic internal logic

#### Novelty
- distance from baseline
- distance from cliché
- frame shift
- new primitive or new organizing principle

### 6. Map failures before deletion
Classify weak candidates as:
- **noise failure**
- **execution failure**
- **constraint failure**
- **frame-edge failure**
- **primitive signal**

A primitive signal is awkward but reveals a stronger underlying move.

### 7. Preserve the anomaly lane
Keep one candidate that is:
- less polished
- more alive
- structurally unusual
- likely to be rejected for unfamiliarity rather than weakness

### 8. Select from a frontier
Return at least:
- safest valid
- strongest alive
- strangest valid

Then explain the tradeoff.

## Story / fiction adapter
For stories, explicitly vary:
- narrative frame
- temporal structure
- distance to character interiority
- sentence pressure
- what is withheld
- governing image or motif

Generate at least:
- conventional scene
- structurally risky scene
- voice-led scene
- premise-redefining scene

Protect candidates that feel slightly wrong in a productive way. Many good stories begin there.

## Art / visual adapter
For art concepts, explicitly vary:
- formal system
- material logic
- symbolic vocabulary
- compositional rules
- emotional temperature
- relationship between image and concept

Generate at least:
- baseline concept
- motif-distortion concept
- medium-shift concept
- structural inversion concept

Reject novelty-by-decoration. Keep novelty with internal necessity.

## Manual operators

For a more systems-oriented version with pipeline thinking, failure mapping for repeated workflows, and architecture/eval framing, see **`software-development/anti-convergence`**.

### Candidate spread
"Generate five structurally different versions: baseline, boundary, cross-domain, reframed, and anomaly. Differences must be conceptual or formal, not just tonal."

### Constraint split
"List hard constraints, soft constraints, and conventions for this task. Then reassess the candidates using that split."

### Anomaly preservation
"Pick the candidate most likely to be wrongly rejected for unfamiliarity. Preserve its distinctive move and repair only what is necessary."

### Frontier output
"Return the safest valid, strongest alive, and strangest valid versions. Explain the tradeoff and what would be lost if only the smoothest one survived."

## Pitfalls
- Mistaking weirdness for originality
- Letting polish override force
- Confusing convention with quality
- Generating paraphrases and calling them alternatives
- Smoothing away the one candidate with real life in it

## Output shape
1. Attractor basin
2. Candidate spread
3. Constraints
4. Validity vs novelty
5. Failure map
6. Frontier
7. Recommended next move

## Example output

**1. Attractor basin**
- polished moodboard imagery with familiar clichés
- generic "cinematic" framing, safe legibility

**2. Candidate spread**
- Baseline: competent default — monumental brutalist ruin, moss, harsh light, film grain
- Boundary: push further — no lush decay, structural terror, inhuman scale
- Cross-domain: import sacred/archaeological frame — reverent stillness, liturgical dust
- Reframed: make subject system failure, not atmosphere — forensic, infrastructural
- Anomaly: overgrowth is more ordered than the architecture — civic afterlife, uncanny calm

**3. Constraints**
- Hard: preserve subject (abandoned brutalism), mood (serious, cinematic), medium (image prompt)
- Soft: tonal severity, composition control, specific material language
- Conventions: "Blade Runner aesthetic", "film grain" — familiar defaults, not requirements

**4. Validity vs novelty**
- Baseline: high validity / low novelty
- Boundary: high validity / medium novelty
- Cross-domain: high validity / high novelty
- Reframed: medium validity (needs care) / high novelty
- Anomaly: medium validity / very high novelty

**5. Failure map**
- Reframed: execution failure risk — idea is strong, articulation needs work
- Anomaly: primitive signal — awkward but reveals a better organizing principle

**6. Frontier**
- Safest valid: Baseline
- Strongest alive: Cross-domain
- Strangest valid: Anomaly

**7. Recommended next move**
Iterate on Anomaly while preserving the formal logic. Repair coherence without normalizing away the distinctive move.

## Short reminder
The point is not to make outputs stranger.
The point is to stop the system from erasing viable difference too early.