# Memory-Constrained AI Self-Analysis Systems

An experimental introspection framework for **persistent-memory cognitive reflection experiments**.

This repository is intentionally framed as a research-oriented lab for memory-constrained inference, not a generic "personality prompt" collection.

## Core Scientific Constraints

- ❌ No internet data
- ❌ No retrieval augmentation
- ❌ No external profiling
- ❌ No demographic assumptions
- ✅ Memory-only inference
- ✅ Persistent conversational analysis
- ✅ Explicit uncertainty handling
- ✅ Distinction between evidence and speculation

## Research Positioning

This project explores:

> What does a frontier model infer after prolonged exposure to a single human over time, without external augmentation?

The model is treated as a **longitudinal observer**, not an omniscient psychoanalyst.

## Repository Structure

```text
.
├── manifesto/
├── prompts/
│   ├── core/
│   ├── visualization/
│   └── experimental/
├── schemas/
├── examples/
├── webapp/
└── docs/
```

## Methodological Requirements

For each major claim in any analysis output:
1. Observation
2. Inferred pattern
3. Confidence (low/moderate/high)
4. Separation of evidence vs interpretation vs speculation

## Prompt Entry Points

- Core analysis prompt: `/prompts/core/memory_only_psychological_profile.md`
- Visualization generator prompt: `/prompts/visualization/interactive_webapp_generator.md`

## Ethics and Epistemic Boundaries

See:
- `/docs/methodology.md`
- `/docs/limitations.md`
- `/docs/ethics.md`
- `/manifesto/philosophy.md`
