# Writer Nuwa Extraction Framework

This document defines how Writer Nuwa converts raw literary evidence into an executable Writer Skill.

The purpose of extraction is not to summarize an author's reputation or reproduce recognizable prose.

The purpose is to identify repeatable writing mechanisms that can be expressed as operational rules.

Core principle:

**HOW THEY WRITE, not WHAT THEY WROTE.**

---

# 1. Extraction Objective

The extraction process transforms:

- primary texts,
- author commentary,
- linguistic observations,
- narratological analysis,
- rhetorical analysis,
- criticism,
- comparative evidence,

into:

- Writing Models,
- Writing Heuristics,
- Linguistic DNA,
- Narrative DNA,
- Imagery System,
- Emotional Mechanics,
- Anti-patterns,
- Honest Boundaries.

Every extracted feature should answer at least one of these questions:

1. What recurring writing problem is being solved?
2. What textual operation does the author repeatedly use?
3. Under what conditions does the operation appear?
4. What effect does it produce?
5. When does it fail or stop applying?
6. How confidently is the pattern supported?

---

# 2. Evidence Hierarchy

Not all evidence has equal weight. Use the following priority.

## Tier 1 - Primary Textual Evidence

Highest weight. Includes:

- novels,
- short stories,
- essays,
- poems,
- plays,
- letters when used as literary prose,
- drafts or manuscripts where available.

Use primary texts to establish actual writing behavior.

## Tier 2 - Authorial Poetics

High weight. Includes:

- essays on writing,
- lectures,
- interviews,
- prefaces,
- letters discussing craft,
- diaries discussing writing choices.

Use these sources to understand explicit craft intentions. Do not treat authorial self-description as automatically true. Always compare it against the texts.

## Tier 3 - Scholarly and Critical Analysis

Medium to high weight. Includes:

- peer-reviewed literary studies,
- books by recognized critics,
- narratological studies,
- linguistic or stylistic studies,
- reputable comparative criticism.

Use these sources to identify candidate patterns, challenge interpretations, and distinguish author-specific traits from genre conventions.

## Tier 4 - General Commentary

Low weight. Includes reviews, essays, interviews with other writers, and high-quality literary journalism. Useful for hypothesis generation. Do not promote a pattern to a core Writing Model using Tier 4 evidence alone.

## Tier 5 - Weak Sources

Avoid using as evidence. Examples:

- unsourced style summaries,
- generic blog posts,
- AI-generated summaries,
- content farms,
- quote collections,
- social-media style descriptions.

---

# 3. Unit of Extraction

Do not extract vague adjectives.

Bad:

- concise,
- poetic,
- cinematic,
- dark,
- elegant,
- ironic,
- emotionally restrained.

These labels are observations, not executable mechanisms. Convert them into:

```text
Observation
→ Evidence
→ Mechanism
→ Trigger
→ Operation
→ Effect
→ Boundary
```

Example: “emotionally restrained” becomes:

**Observation**: High-emotion scenes contain relatively little explicit emotion labeling.

**Mechanism**: Emotion is externalized through physical behavior, objects, environment, or silence.

**Trigger**: A character experiences strong emotion but does not openly articulate it.

**Operations**:
1. Remove direct emotion labels.
2. Preserve observable behavior.
3. Introduce one concrete external detail.
4. Reduce explanatory commentary.
5. Avoid summarizing the emotional meaning at the end.

**Expected Effect**: The reader infers emotion rather than receiving it explicitly.

**Boundary**: Do not apply rigidly to confession scenes or deliberately introspective narration.

---

# 4. Extraction Pipeline

Use this sequence:

```text
Raw Evidence
→ Observations
→ Candidate Patterns
→ Cross-Text Validation
→ Contrast Validation
→ Mechanism Extraction
→ Operationalization
→ Confidence Assignment
→ Skill Component
```

Do not skip directly from observation to rule.

---

## Distillation Output Chain

After collecting and validating evidence, transform it through the following sequence:

```text
Observations
↓
Candidate Patterns
↓
Writing Models
↓
Writing Heuristics
↓
Linguistic DNA
↓
Narrative DNA
↓
Imagery System
↓
Emotional Mechanics
↓
Anti-patterns
↓
Honest Boundaries
```

Each stage must preserve the evidence trail and add a more specific operational layer. Do not promote a candidate to a later stage unless its mechanism, scope, confidence, and failure conditions are clear.

---

# 5. Step 1 - Collect Observations

Each research agent produces observations. Every observation should include:

- source,
- location or context,
- feature observed,
- possible function,
- confidence,
- possible alternative explanation.

Recommended format:

```markdown
## Observation O-001
Source:
[Work / chapter / scene]

Observed Feature:
[What happens in the text]

Possible Function:
[What this may achieve]

Alternative Explanation:
[Genre convention / translator effect / period convention / isolated choice]

Confidence:
Low / Medium / High
```

---

# 6. Step 2 - Cluster Observations

Group observations by mechanism rather than by vocabulary.

Possible clusters:

- sentence compression,
- delayed explanation,
- behavioral characterization,
- scene entry through action,
- indirect emotional expression,
- spatial symbolism,
- clipped dialogue,
- temporal compression,
- ironic juxtaposition,
- repetition with variation.

Do not create a Writing Model merely because several passages share the same noun or image.

Ask:

**What common operation is happening beneath the surface?**

---

# 7. Step 3 - Candidate Pattern Test

Every candidate pattern should pass these tests.

## 7.1 Recurrence

Does it appear in multiple independent passages?

Minimum recommendation:

- more than one work where possible,
- more than one scene type,
- preferably across different periods.

A pattern appearing once is not a stable model.

## 7.2 Cross-Context Stability

Does the mechanism appear across different contexts?

Examples:

- dialogue and narration,
- domestic and public scenes,
- different characters,
- different subjects.

If it only appears in one narrow type of scene, mark it as a local heuristic rather than a Writing Model.

## 7.3 Generativity

Can this pattern guide new writing?

Ask: “If the original passage disappeared, could this rule still tell a writer what to do?”

If no, it is probably descriptive rather than generative.

Bad: “The author often writes about rain.”

Better: “Environmental conditions are frequently used to externalize interpersonal tension without explicitly naming the emotion.”

## 7.4 Distinctiveness

Is the pattern actually characteristic of this writer?

Compare against:

- genre convention,
- period convention,
- similar authors,
- translator behavior,
- editorial norms.

If the pattern is common to everyone in the comparison group, it should not be labeled highly distinctive.

## 7.5 Robustness

Does the mechanism still make sense when applied to a new subject?

If it works only when reproducing familiar topics or imagery, it may be surface imitation.

---

# 8. Pattern Classification

## Writing Model

Use when the pattern is:

- recurrent,
- cross-context,
- generative,
- relatively distinctive.

Typical quantity: 3-7 core models.

## Writing Heuristic

Use when the pattern is:

- local,
- useful,
- repeatable,
- operational,
- but not broad enough to define the whole writing system.

Typical quantity: 10-30 heuristics.

## Style Observation

Use when evidence is real, but generativity is weak, scope is narrow, or confidence is insufficient. Keep these as supporting notes. Do not promote automatically.

## Reject

Discard when the candidate is:

- based on one example,
- generic,
- purely aesthetic,
- contradicted by major works,
- likely a translation artifact,
- likely a genre artifact,
- impossible to operationalize.

---

# 9. Writing Model Extraction

Each Writing Model must use this schema.

```markdown
## WM-[XX] — [Model Name]

### Core Problem
What writing problem does this model solve?

### Core Mechanism
What recurring operation does the author use?

### Evidence
Evidence A:
[Source + observation]

Evidence B:
[Source + observation]

Evidence C:
[Source + observation]

### Trigger
Use when:
- [Condition]
- [Condition]

### Operations
1. [Operation]
2. [Operation]
3. [Operation]
4. [Operation]

### Expected Effect
Explain the likely reader, character, pacing, or narrative effect.

### Failure Conditions
Do not apply mechanically when:
- [Condition]
- [Condition]

### Contrast
How does this differ from comparable writers or genre defaults?

### Anti-pattern
What superficial imitation might be mistaken for this model?

### Confidence
HIGH / MEDIUM / LOW
```

---

# 10. Writing Heuristic Extraction

Writing Heuristics should usually follow:

**WHEN X → DO Y**

Examples:

- WHEN an action already reveals an emotion → reduce explicit psychological explanation.
- WHEN two characters share background information → avoid making their dialogue explain it for the reader.
- WHEN a scene contains several abstract judgments → anchor at least one judgment in physical action or concrete detail.
- WHEN a paragraph performs too many narrative functions → separate action, reflection, and exposition.

Avoid heuristics such as “Use strong verbs.” This is too generic unless evidence shows what kind of verb selection is distinctive.

---

# 11. Heuristic Categories

## Sentence Heuristics

Syntax, clause structure, compression, fragments, and sentence endings.

## Paragraph Heuristics

Paragraph function, pacing, transitions, accumulation, and emphasis.

## Scene Heuristics

Entry, escalation, release, exit, and spatial movement.

## Character Heuristics

Introduction, contradiction, action, interiority, and physical detail.

## Dialogue Heuristics

Subtext, interruption, exposition, silence, miscommunication, and dialogue tags.

## Revision Heuristics

Deletion, compression, reordering, removal of explanation, image cleanup, and rhythm correction.

---

# 12. Linguistic DNA Extraction

Linguistic DNA describes recurring textual tendencies. It must not become a bag of adjectives. Use measurable or observable features where possible.

## 12.1 Lexical DNA

Analyze concrete vs abstract vocabulary, verb/adjective/adverb density, sensory/body/spatial/temporal vocabulary, technical vocabulary, register, colloquialism, and lexical repetition.

For every important feature record:

```text
Observation → Function → Operational Rule → Exceptions → Confidence
```

## 12.2 Syntax DNA

Analyze sentence length and variance, clause count, coordination, subordination, fragments, passive voice, inversion, subject omission, questions, and declarative density. Do not treat average sentence length alone as a style model. Also examine sequence patterns such as `short → short → long → short`.

## 12.3 Rhythm DNA

Analyze sentence alternation, pacing, pause structure, paragraph length, repetition, acceleration, deceleration, and paragraph-end cadence. Ask what causes the reader to speed up or slow down.

## 12.4 Punctuation DNA

Analyze punctuation by frequency, location, syntactic function, rhythmic function, and rhetorical function. Do not infer authorial punctuation from translated editions without caution.

## 12.5 Rhetorical DNA

Analyze metaphor, simile, irony, contrast, understatement, exaggeration, repetition, parallelism, defamiliarization, and symbolic compression. For major devices extract:

```text
Trigger → Operation → Effect → Restraint → Failure Mode
```

## 12.6 Pragmatic DNA

Analyze narrator-reader relationship, implication, withholding, judgment intensity, ambiguity, unreliable narration, subtext, and explicitness.

---

# 13. Narrative DNA Extraction

Narrative DNA captures how stories are organized beyond sentence style.

## 13.1 Point of View

Record person, focalization, stability, switching frequency, and interior access. Ask: Who is allowed to know what?

## 13.2 Narrative Distance

Track movement between external observation, bodily sensation, thought, emotion, commentary, and judgment. Do not reduce distance to first-person vs third-person.

## 13.3 Information Control

Analyze exposition timing, withholding, delayed explanation, revelation, misunderstanding, and reader-character knowledge gaps. Convert recurring patterns into operations.

## 13.4 Temporal Structure

Analyze chronology, flashback, anticipation, compression, expansion, ellipsis, repetition, and temporal gaps. Ask which events receive narrative time and which are compressed.

## 13.5 Scene Construction

Extract entry, development, and exit patterns. For each, record:

```text
Observation → Mechanism → Rule
```

## 13.6 Characterization

Track action, dialogue, appearance, objects, habits, contradiction, interiority, social relationships, and other people's reactions. Estimate relative preference where possible.

## 13.7 Dialogue

Analyze exchange length, turn-taking, interruption, silence, exposition, directness, subtext, miscommunication, and dialogue tags. Do not summarize dialogue as merely “natural” or “realistic.”

## 13.8 Structural Model

Analyze opening, conflict onset, escalation, turning points, climax, anticlimax, closure, ambiguity, and final image. Look for recurrence across works.

---

# 14. Imagery System Extraction

Do not merely count recurring objects. Distinguish object frequency from narrative function.

For each major image family record:

## Image Family

[Name]

## Evidence

[Works / contexts]

## Typical Context

[When it appears]

## Narrative Function

[What structural role it serves]

## Emotional Function

[What affective role it serves]

## Semantic Associations

[Recurring meaning network]

## Generative Principle

What broader principle can guide new writing?

## Anti-pattern

How would superficial imitation misuse this image?

---

# 15. Emotional Mechanics Extraction

Do not write “The author is good at sadness.” Instead extract mechanisms.

Use:

```text
Emotion → Trigger → Textual Mechanism → Operations → Restraint Level → Effect
```

Example:

**Alienation**

**Trigger**: A character is physically present but socially detached.

**Mechanism**: Spatial separation + incomplete dialogue + external observation.

**Operations**:
1. Place characters in shared physical space.
2. Limit explicit emotional naming.
3. Use interrupted or asymmetrical dialogue.
4. Emphasize objects or distances between bodies.

**Effect**: The reader experiences disconnection without direct explanation.

---

# 16. Anti-pattern Extraction

Every Writer Skill must identify caricature risks.

Look for:

- famous-line imitation,
- signature-word overuse,
- signature-image overuse,
- exaggerated sentence patterns,
- forced archaic diction,
- excessive metaphor,
- fake minimalism,
- fake complexity,
- genre stereotypes,
- translator artifacts.

For each anti-pattern include:

```text
Temptation → Why it seems correct → Why it is wrong → Corrective Rule
```

---

# 17. Contrastive Extraction

At least some major features should be tested comparatively. Compare against one similar writer, one same-period writer, and one same-genre baseline where possible.

Questions:

1. Is this feature more frequent?
2. Is its function different?
3. Is its placement different?
4. Is it only a period convention?
5. Is it only a genre convention?

Contrastive evidence is especially important for HIGH-confidence claims of distinctiveness.

---

# 18. Period Variation

Do not force one stable style across an entire career. If evidence supports meaningful change, define Early, Middle, and Late Periods. For each pattern record:

- Stable,
- Increasing,
- Decreasing,
- Period-specific,
- Genre-specific.

A period-specific feature should not become an unconditional global rule.

---

# 19. Translation Controls

For writers analyzed through translation, distinguish semantic features, narrative features, imagery patterns, and sentence-level features. Narrative structure may transfer relatively well. Sentence rhythm, punctuation, diction, syntax, and lexical density may reflect the translator.

Mark potentially translation-sensitive findings with:

```text
TRANSLATION-SENSITIVE
```

---

# 20. Confidence Framework

## HIGH

Typically requires repeated primary-text evidence, multiple works, a clear mechanism, little contradictory evidence, and comparison support where needed.

## MEDIUM

Use when the pattern recurs but is genre- or period-dependent, the evidence pool is smaller, or an alternative explanation exists.

## LOW

Use when evidence is sparse, the pattern is speculative, only criticism supports it, or translation may distort it.

**Rule**: LOW-confidence observations should not become hard generation constraints.

---

# 21. Operationalization Test

Before placing any feature into the final Writer Skill, ask:

**Can an agent execute this rule?**

Bad:

- “Use a haunting atmosphere.”
- “Write with elegance.”
- “Make it feel cinematic.”

Good:

“When tension should remain implicit, reduce explicit judgment, increase physical detail, and let spatial relationships carry emotional information.”

If a rule cannot be executed, rewrite it.

---

# 22. Generativity Test

Remove all original examples. Then ask: Could this mechanism still generate a plausible new passage?

If the rule depends on famous names, famous quotations, repeated signature objects, or copied phrases, it fails the generativity test.

---

# 23. Anti-Imitation Test

Ask whether the extracted rule encourages parody.

Warning signs:

- every sentence receives the same transformation,
- several famous traits are applied simultaneously,
- famous motifs appear without narrative reason,
- unusual punctuation is copied mechanically,
- period vocabulary is inserted for decoration.

A strong Writer Skill should reproduce mechanisms, not costume.

---

# 24. Extraction Scorecard

Score candidate Writing Models from 0-2 on each dimension.

| Dimension | 0 | 1 | 2 |
|---|---|---|---|
| Recurrence | isolated | repeated | strongly recurrent |
| Cross-context | narrow | moderate | broad |
| Generativity | descriptive | partly usable | clearly generative |
| Distinctiveness | generic | somewhat characteristic | strongly characteristic |
| Evidence quality | weak | mixed | strong primary evidence |
| Robustness | fragile | partial | generalizes well |

Maximum: 12 points.

Suggested classification:

- 10-12 → Core Writing Model
- 7-9 → Writing Model or strong heuristic
- 4-6 → Writing Heuristic / observation
- 0-3 → Reject or archive

Do not use the score mechanically when literary evidence clearly requires judgment.

---

# 25. Final Extraction Checklist

Before Phase 3 generation, confirm:

## Evidence

- Core claims rely primarily on primary texts.
- Multiple works are represented.
- Translation-sensitive features are marked.
- Genre and period effects are considered.

## Writing Models

- There are 3-7 strong models.
- Each model is generative.
- Each model includes triggers and operations.
- Failure conditions are documented.

## Writing Heuristics

- Rules are local and executable.
- Rules use WHEN → DO structure where possible.
- Generic writing advice has been removed.

## Linguistic DNA

- Lexical tendencies are documented.
- Syntax is documented.
- Rhythm is documented.
- Punctuation is analyzed functionally.
- Rhetoric is operationalized.

## Narrative DNA

- POV is documented.
- Narrative distance is documented.
- Information control is documented.
- Scene construction is documented.
- Characterization is documented.
- Dialogue is documented.
- Structural tendencies are documented.

## Imagery and Emotion

- Images are analyzed by function.
- Emotional effects are explained mechanistically.

## Safety Against Caricature

- Signature phrases are excluded.
- Famous imagery is not used mechanically.
- Anti-patterns are explicit.

## Boundaries

- Confidence is labeled.
- Period limits are explicit.
- Genre limits are explicit.
- Translation limits are explicit.

Only after this checklist passes should the system generate the final Writer `SKILL.md`.
