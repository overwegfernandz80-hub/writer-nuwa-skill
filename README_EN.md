# Writer Nuwa

> Distill how a writer writes, not just what they wrote.

Writer Nuwa is a derivative project based on [NUWA-Skill](https://github.com/alchaincyf/nuwa-skill). It adapts the research and validation method into a writing-system distillation workflow.

## What It Does

Input an author and a scope. Writer Nuwa builds a corpus, extracts evidence-backed writing mechanisms, and assembles a runnable Writer `SKILL.md`.

It produces:

- Writing Models
- Writing Heuristics
- Linguistic DNA
- Narrative DNA
- Imagery System
- Emotional Mechanics
- Anti-patterns
- Honest Boundaries

## How It Works

```text
Author + Scope
      ↓
Corpus Building
      ↓
6 Parallel Writer Research Agents
      ↓
Writing Models
Writing Heuristics
Linguistic DNA
Narrative DNA
Imagery System
      ↓
Writer SKILL.md
      ↓
Fidelity Validation
      ↓
Dual Reviewer Refinement
```

### Phase 1 — Research

Six agents analyze the corpus from different angles:

1. Corpus Analyst
2. Linguistic Analyst
3. Narratology Analyst
4. Rhetoric & Imagery Analyst
5. Poetics & Criticism Analyst
6. Period & Contrast Analyst

### Phase 2 — Distillation

Descriptive labels such as “restrained” or “cinematic” do not enter the skill directly. Each candidate must become:

```text
Observation → Evidence → Mechanism → Trigger → Operation → Failure Condition
```

### Phase 3 — Skill Assembly

The extracted systems are assembled into a Writer `SKILL.md`.

### Phase 4 — Fidelity Validation

The skill is tested with reconstruction, unseen-topic, ablation, anti-caricature, contrast, imitation, recognition, and application tests.

### Phase 5 — Refinement

Two independent reviewers check different questions:

- **Literary Fidelity Critic**: Is this true to the evidence?
- **Generative Writing Engineer**: Can this actually run?

## Usage

Install Writer Nuwa from the repository:

```bash
npx skills add overwegfernandz80-hub/writer-nuwa-skill
```

Then ask your agent:

```text
Distill Lu Xun's writing system

Generate a Hemingway Writer Skill

Analyze the writing mechanisms in Eileen Chang's novels

Create a Chekhov short-fiction Writer Skill
```

## Output

Each distillation typically produces:

```text
writer-author/
├── SKILL.md
├── FIDELITY.md
└── references/
    └── research/
        ├── 01-corpus.md
        ├── 02-linguistic-dna.md
        ├── 03-narrative-dna.md
        ├── 04-rhetoric-imagery.md
        ├── 05-poetics-criticism.md
        └── 06-period-contrast.md
```

## Important Boundaries

Writer Nuwa does not copy specific works or collage recognizable lines. It prioritizes high-level writing mechanisms, narrative structure, linguistic tendencies, rhetorical mechanisms, and editing principles.

For living authors, use it primarily for style analysis, writing education, high-level feature research, and non-high-fidelity creative guidance.

For translated literature, distinguish the author's original-language features from the translator's language features.

## Credits

Writer Nuwa is a derivative project based on [NUWA-Skill](https://github.com/alchaincyf/nuwa-skill).

Original NUWA methodology: Huashu / alchaincyf.

This fork adapts cognitive distillation into writer-system distillation.
