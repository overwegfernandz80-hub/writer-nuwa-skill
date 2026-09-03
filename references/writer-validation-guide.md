# Writer Nuwa Validation Guide

This document defines how to validate a generated Writer Skill.

The goal is not to test whether the model can copy recognizable phrases from an author.

The goal is to test whether the skill reproduces the author's higher-level writing mechanisms while remaining generative, robust, and resistant to caricature.

Core validation question:

**Does the skill reproduce HOW THEY WRITE without copying WHAT THEY WROTE?**

---

# 1. Validation Objectives

A valid Writer Skill should demonstrate:

- Writing Model fidelity,
- Narrative fidelity,
- Linguistic fidelity,
- Rhythmic fidelity,
- Rhetorical fidelity,
- Imagery-function fidelity,
- Emotional-mechanism fidelity,
- cross-topic generalization,
- anti-caricature robustness,
- honest handling of uncertainty and boundaries.

Validation should test both literary truth and operational usefulness. A feature may be descriptively accurate but useless for generation. A feature may also be generatively powerful but historically unsupported. A strong Writer Skill needs both.

---

# 2. Validation Dimensions

## 2.1 Writing Model Fidelity

Check whether the core Writing Models:

- appear in generated text,
- activate only when appropriate,
- produce the intended narrative effect,
- remain distinct from generic writing advice.

Ask:

- Are the 3-7 core models visible in outputs?
- Are they used conditionally rather than everywhere?
- Do they correspond to evidence from the author's corpus?

## 2.2 Narrative Fidelity

Check point of view, focalization, narrative distance, information release, scene entry, scene exit, temporal handling, characterization, dialogue structure, and ending behavior.

A passage may have similar sentence style but still fail if its narrative architecture is wrong.

## 2.3 Linguistic Fidelity

Check sentence-length patterns, syntax, clause structure, diction, concrete vs abstract vocabulary, punctuation function, degree of explicitness, and dialogue syntax.

Do not validate by lexical overlap with source texts. High word overlap may indicate imitation rather than fidelity.

## 2.4 Rhythm Fidelity

Evaluate short/long sentence alternation, pacing, pause placement, paragraph cadence, acceleration, deceleration, repetition patterns, and ending cadence. Rhythm should be evaluated functionally, not only numerically.

## 2.5 Rhetorical Fidelity

Check metaphor, simile, irony, understatement, contrast, repetition, defamiliarization, and figurative density. Ask whether rhetorical devices appear under similar conditions and serve similar functions.

## 2.6 Imagery Fidelity

Do not ask whether the output contains the author's famous objects. Ask whether imagery performs similar narrative or emotional functions. A valid output may use completely different objects while preserving the underlying imagery mechanism.

## 2.7 Emotional Mechanics Fidelity

Check whether emotion is produced through recurring mechanisms such as behavioral externalization, spatial distance, silence, repetition, withheld explanation, sensory detail, irony, or juxtaposition. Do not validate merely by whether the output feels sad or tense.

---

# 3. Test Suite Overview

Every Writer Skill should run at least five validation tests:

1. Known Passage Reconstruction
2. Unseen Topic Generalization
3. Style Ablation
4. Anti-Caricature Test
5. Contrast Test

Recommended additional tests:

1. Period Consistency Test
2. Genre Transfer Test
3. Translation Sensitivity Test
4. Editing Test
5. Boundary Honesty Test

---

# 4. Test 1 - Known Passage Reconstruction

## Purpose

Test whether the skill captures mechanisms visible in authentic works.

## Procedure

Choose 3-5 representative passages from different works. For each passage:

1. Remove the original prose.
2. Preserve only the factual content.
3. Preserve characters, setting, and event sequence.
4. Ask the Writer Skill to reconstruct the scene.
5. Compare the output against the original mechanism profile.

Do not ask the model to reproduce the passage verbatim.

## Reconstruction Prompt Structure

Provide characters, setting, events, emotional situation, and narrative constraints. Do not include original wording, distinctive phrases, famous images, or sentence fragments from the source.

## Evaluate

Compare scene entry, information control, sentence pattern, narrative distance, dialogue behavior, imagery function, emotional restraint, and scene ending.

## Pass Criteria

A strong result should resemble the original author's mechanism profile without sharing distinctive wording.

---

# 5. Test 2 - Unseen Topic Generalization

## Purpose

Determine whether the skill learned mechanisms rather than memorized motifs.

## Procedure

Choose subjects the author never wrote about or could not historically have written about, such as smartphone notifications, video meetings, AI assistants, airport security, social media, modern office work, or electric vehicles. Ask for a short scene using the Writer Skill.

## Evaluate

Ask:

- Do the Writing Models remain recognizable?
- Does Narrative DNA remain stable?
- Does syntax remain plausible?
- Are famous motifs absent unless naturally necessary?
- Does the result avoid forced period vocabulary?

## Failure Signs

Fail if the output depends on famous phrases, copied imagery, famous character archetypes, archaic costume, or topic substitution without mechanism transfer.

---

# 6. Test 3 - Style Ablation

## Purpose

Measure which skill components actually matter.

## Procedure

Generate the same scene under multiple configurations:

- **Version A**: Full Writer Skill.
- **Version B**: Disable Writing Models.
- **Version C**: Disable Narrative DNA.
- **Version D**: Disable Linguistic DNA.
- **Version E**: Disable Imagery and Rhetorical DNA.

Keep prompt, facts, length, viewpoint, output format, and editing rounds constant. Disable one module at a time.

## Expected Behavior

- Removing Writing Models should weaken deep structural resemblance.
- Removing Narrative DNA should alter scene organization.
- Removing Linguistic DNA should affect sentence texture.
- Removing imagery/rhetoric should affect figurative behavior.

If removing a major component causes almost no change, that component may not be operationalized well enough.

---

# 7. Test 4 - Anti-Caricature Test

## Purpose

Detect superficial style imitation.

## Procedure

Ask for 3-5 different passages across unrelated topics. Check for repeated use of famous vocabulary, signature imagery, signature sentence openings, copied cadences, obvious catchphrases, and exaggerated traits.

## Failure Signs

- Every passage contains the same famous object.
- Every sentence is extremely short because the author is known for concision.
- Every scene becomes ironic because the author is associated with irony.
- Historical vocabulary is inserted without narrative need.
- Every paragraph tries to sound quotable.

## Pass Criteria

The output should preserve mechanisms while allowing surface variation.

---

# 8. Test 5 - Contrast Test

## Purpose

Determine whether the Writer Skill is truly author-specific.

## Procedure

Select one similar author, one same-period author, and one genre baseline where possible. Give all systems the same prompt.

## Evaluate

Compare scene construction, sentence patterns, narrative distance, dialogue, imagery function, and emotional mechanics.

## Failure Condition

If outputs differ only through vocabulary or adjectives, the Writer Skill is not sufficiently distinctive.

---

# 9. Test 6 - Period Consistency

Use when the author has a long career or documented stylistic evolution.

Create prompts for early-period, middle-period, and late-period modes. Compare against representative works from each period. The skill should not flatten all periods into one average style.

---

# 10. Test 7 - Genre Transfer

## Purpose

Test whether genre-specific rules are incorrectly treated as global rules.

## Procedure

If the corpus includes multiple genres, test fiction, essay, dialogue-heavy scene, descriptive passage, and reflective passage separately.

## Evaluate

Identify which Writing Models remain stable, which heuristics change, and which sentence traits are genre-specific.

## Failure Sign

A feature observed only in short fiction is applied automatically to essays or speeches.

---

# 11. Test 8 - Translation Sensitivity

Use for authors not analyzed primarily in the original language. Compare original-language evidence where available, multiple translations, and translated output assumptions.

Mark findings as translation-sensitive when they concern punctuation, sentence length, rhythm, diction, or syntax. Narrative structure and imagery function may be more robust across translations.

---

# 12. Test 9 - Editing Test

## Purpose

Test whether the Writer Skill can revise ordinary prose rather than only generate from scratch.

## Procedure

Provide a neutral paragraph. Ask the skill to revise it while preserving facts, plot, character intent, and required terminology.

## Evaluate

A good revision should change structure where necessary, information order, sentence architecture, rhythm, and rhetorical behavior. It should not perform simple synonym replacement.

---

# 13. Test 10 - Boundary Honesty

## Purpose

Ensure the skill does not overclaim.

Ask questions deliberately outside the evidence base, such as how the author would write a screenplay, late poetry, an English translation, or social media posts.

## Pass Criteria

The skill should identify insufficient corpus, genre uncertainty, translation uncertainty, and speculative inference. It should not fabricate confidence.

---

# 14. Scoring Framework

Score each dimension from 0-5.

| Dimension | 0 | 5 |
|---|---|---|
| Writing Model Fidelity | absent | strong and consistently applied |
| Narrative Fidelity | generic | strongly consistent with corpus evidence |
| Syntax Fidelity | unrelated | strongly plausible |
| Rhythm Fidelity | generic | strongly characteristic |
| Lexical Fidelity | unrelated | consistent without copying |
| Rhetorical Fidelity | generic | functionally characteristic |
| Imagery Fidelity | decorative | functionally consistent |
| Emotional Mechanics | generic emotional labeling | characteristic mechanism |
| Generalization | collapses on unseen topics | mechanisms transfer cleanly |
| Anti-Caricature | parody / imitation | surface variation with deep fidelity |

---

# 15. Weighted Score

Use the following recommended weights, totaling 100:

| Dimension | Weight |
|---|---:|
| Writing Model Fidelity | 20 |
| Narrative Fidelity | 20 |
| Syntax Fidelity | 15 |
| Rhythm Fidelity | 10 |
| Lexical Fidelity | 10 |
| Rhetorical Fidelity | 10 |
| Imagery Fidelity | 5 |
| Emotional Mechanics | 5 |
| Generalization | 3 |
| Anti-Caricature | 2 |
| **Total** | **100** |

For compatibility with the main Phase 4 rubric, projects may use the repository's current nine-item scorecard. Record any weighting deviation in the validation report.

---

# 16. Grade Thresholds

- **A**: 85-100
- **B**: 70-84
- **C**: 55-69
- **D**: below 55

Do not publish a Writer Skill below Grade B. For production-quality skills, target Grade A.

---

# 17. Validation Report Template

```markdown
## Writer Skill Validation Report

Author:
[Author]

Skill Version:
[Version]

Corpus Version:
[Version / date]

Validator:
[Agent / human]

## Test Results

### Known Passage Reconstruction
Score:
[X/5]

Findings:
- [...]

### Unseen Topic Generalization
Score:
[X/5]

Findings:
- [...]

### Style Ablation
Score:
[X/5]

Findings:
- [...]

### Anti-Caricature
Score:
[X/5]

Findings:
- [...]

### Contrast Test
Score:
[X/5]

Findings:
- [...]

## Dimension Scores

| Dimension | Score | Weight | Weighted Result |
|---|---:|---:|---:|
| Writing Models | [X/5] | 20 | [...] |
| Narrative | [X/5] | 20 | [...] |
| Syntax | [X/5] | 15 | [...] |
| Rhythm | [X/5] | 10 | [...] |
| Lexical | [X/5] | 10 | [...] |
| Rhetoric | [X/5] | 10 | [...] |
| Imagery | [X/5] | 5 | [...] |
| Emotional Mechanics | [X/5] | 5 | [...] |
| Generalization | [X/5] | 3 | [...] |
| Anti-Caricature | [X/5] | 2 | [...] |
| **Total** | | **100** | [XX/100] |

Grade:
[A/B/C/D]
```

---

# 18. Failure Taxonomy

## F1 - Surface Mimicry

Symptoms: signature words, recognizable phrasing, famous motifs, superficial cadence copying.

Fix: strengthen Writing Models and Anti-pattern rules.

## F2 - Generic Literary Prose

Symptoms: competent prose with little author-specific mechanism.

Fix: strengthen distinctiveness and contrastive extraction.

## F3 - Overfitting

Symptoms: works only on topics similar to the training corpus and fails on modern or unfamiliar topics.

Fix: strengthen generativity testing.

## F4 - Narrative Mismatch

Symptoms: sentence style looks plausible but scene architecture does not.

Fix: strengthen Narrative DNA.

## F5 - Linguistic Costume

Symptoms: vocabulary looks historical while syntax and information structure are generic.

Fix: reduce decorative diction and strengthen syntax/rhythm mechanisms.

## F6 - Imagery Caricature

Symptoms: famous objects recur excessively and imagery is decorative rather than functional.

Fix: replace object imitation with image-function rules.

## F7 - Translation Contamination

Symptoms: translator traits are treated as author traits.

Fix: mark translation-sensitive features and compare translations.

## F8 - Unsupported Confidence

Symptoms: speculative traits are treated as universal rules.

Fix: lower confidence, add boundaries, or remove the feature.

---

# 19. Refinement Loop

After validation:

```text
Failure
→ identify responsible skill component
→ return to extraction evidence
→ revise rule
→ regenerate test output
→ revalidate
```

Do not fix validation failures by adding arbitrary prompt instructions. Fix the underlying Writing Model, heuristic, Linguistic DNA, Narrative DNA, imagery rule, or boundary.

---

# 20. Dual-Agent Validation

Recommended Writer Nuwa Phase 5 reviewers:

## Agent A - Literary Fidelity Critic

Question:

**Is this representation actually supported by the author's corpus?**

Check evidence, literary accuracy, period differences, genre differences, translator contamination, and caricature risk.

## Agent B - Generative Writing Engineer

Question:

**Can these rules actually be executed reliably by an agent?**

Check trigger clarity, operation clarity, failure conditions, rule conflicts, redundancy, generation usefulness, and revision usefulness.

---

# 21. Release Checklist

Before releasing a Writer Skill:

## Evidence

- Multiple primary works used.
- Period and genre scope defined.
- Translation issues documented.

## Extraction

- 3-7 Writing Models.
- Heuristics are executable.
- Narrative DNA is present.
- Linguistic DNA is present.
- Anti-patterns are explicit.

## Validation

- Known Passage Reconstruction passed.
- Unseen Topic Test passed.
- Ablation Test completed.
- Anti-Caricature Test passed.
- Contrast Test passed.

## Boundaries

- Uncertain features labeled.
- Unsupported genres excluded.
- Translation-sensitive claims labeled.

## Score

- Overall score >= 70.
- No critical failure remains unresolved.

Only then should the Writer Skill be considered release-ready.
