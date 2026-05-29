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

## Quick Start Prompts

### Master Prompts (Primary Entry Points)

Start with **one of these** based on your analysis goal:

| Category | Master Prompt | Purpose |
|----------|--------------|---------|
| **Core Analysis** | [`memory_only_psychological_profile.md`](/prompts/core/memory_only_psychological_profile.md) | Comprehensive system-level analysis across cognition, psychology, behavioral dynamics, and operational patterns |
| **Visualization** | [`interactive_webapp_generator.md`](/prompts/visualization/interactive_webapp_generator.md) | Generate interactive visualizations and web-based data representations |
| **Research & Projection** | [`trajectory_projection.md`](/prompts/experimental/trajectory_projection.md) | Exploratory analysis with future-direction hypotheses and pattern research |

### Specialized Prompts

For deeper exploration of specific aspects, use these after the master prompt:

**Core Analysis Specializations:**
- [`behavioral_risk_analysis.md`](/prompts/core/behavioral_risk_analysis.md) — Risk patterns, burnout susceptibility, over-optimization
- [`cognitive_architecture_analysis.md`](/prompts/core/cognitive_architecture_analysis.md) — Thinking patterns, reasoning frameworks, decision-making style
- [`founder_operator_profile.md`](/prompts/core/founder_operator_profile.md) — Operational dynamics, leadership patterns, management approach
- [`ai_relationship_analysis.md`](/prompts/core/ai_relationship_analysis.md) — Interaction patterns with AI systems, communication preferences

**Visualization Specializations:**
- [`timeline_visualizer.md`](/prompts/visualization/timeline_visualizer.md) — Timeline-specific data visualization
- [`graph_schema_generator.md`](/prompts/visualization/graph_schema_generator.md) — Graph and schema-based visualizations

**Research Specializations:**
- [`latent_identity_analysis.md`](/prompts/experimental/latent_identity_analysis.md) — Identity construction and narrative patterns
- [`contradiction_mapper.md`](/prompts/experimental/contradiction_mapper.md) — Paradoxes and pattern contradictions

### Which Prompt Should I Use?

1. **First time?** → Start with **Master Prompt** for your use case
2. **Need specific insight?** → Use a **Specialized Prompt** after master analysis
3. **Exploring uncertainties?** → Use **Research** category for hypothesis generation
4. **Want visualizations?** → Use **Visualization** master for interactive outputs

For detailed workflows, decision trees, and prompt selection FAQ, see [`/docs/prompt_selection_guide.md`](/docs/prompt_selection_guide.md).

## Ethics and Epistemic Boundaries

See:
- `/docs/methodology.md`
- `/docs/limitations.md`
- `/docs/ethics.md`
- `/manifesto/philosophy.md`
