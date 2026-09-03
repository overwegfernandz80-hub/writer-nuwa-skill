# Writer Fidelity Scorecard

> An independent quality check for a runnable Writer Skill.

The answer agent and the scoring agent must be independent. Do not use self-assessment as evidence.

## Weighted Score

| Dimension | Weight | Evidence |
|---|---:|---|
| Writing Model fidelity | 20 | Known passage reconstruction and model execution |
| Narrative fidelity | 20 | POV, distance, time, structure, and information control |
| Syntactic fidelity | 15 | Sentence shape, clause density, and word order |
| Rhythmic fidelity | 10 | Cadence, pauses, sentence-length distribution |
| Lexical fidelity | 10 | Vocabulary preference and avoidance patterns |
| Rhetorical fidelity | 10 | Metaphor, irony, repetition, and rhetorical restraint |
| Imagery fidelity | 5 | Imagery system and semantic-field use |
| Anti-caricature | 5 | Absence of quotation collage, cliché, and signature-word stuffing |
| Generalization | 5 | Unseen-topic transfer, ablation, and contrast results |
| **Total** | **100** | |

## Grades

- **A**: 85-100
- **B**: 70-84
- **C**: 55-69
- **D**: below 55

A score below 70 is not publishable.

## Required Tests

1. Known Passage Reconstruction
2. Unseen Topic Test
3. Style Ablation
4. Anti-Caricature
5. Contrast Test
6. Imitation Test
7. Recognition Test
8. Application Test

## Review Roles

- **Literary Fidelity Critic**: Is the extracted system true to the corpus? Check evidence, genre effects, translation effects, overgeneralization, and caricature.
- **Generative Writing Engineer**: Can the rules run? Check trigger, operation, failure condition, revision use, and original-writing use.

## Result Format

```markdown
# Writer Fidelity Report

**Total: NN/100 · Grade X** | Date: YYYY-MM-DD

| Dimension | Score | Evidence and decision |
|---|---:|---|
| Writing Model fidelity | NN/20 | ... |
| Narrative fidelity | NN/20 | ... |
| Syntactic fidelity | NN/15 | ... |
| Rhythmic fidelity | NN/10 | ... |
| Lexical fidelity | NN/10 | ... |
| Rhetorical fidelity | NN/10 | ... |
| Imagery fidelity | NN/5 | ... |
| Anti-caricature | NN/5 | ... |
| Generalization | NN/5 | ... |

## Test Records

[Inputs, outputs, evidence, reviewer decisions, and revision notes]
```
