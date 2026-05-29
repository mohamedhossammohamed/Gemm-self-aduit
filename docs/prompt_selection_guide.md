# Prompt Selection Guide

This guide helps you navigate the prompt taxonomy and choose the right tool for your analysis goals.

## Overview

The repository provides **3 master prompts** (primary entry points) and **8 specialized prompts** (for deeper exploration). This structure reduces decision fatigue by providing a clear primary choice while maintaining access to specialized tools.

```
Master Prompts (Start Here)
    ├── Core Analysis (comprehensive cognitive/psychological/behavioral system analysis)
    ├── Visualization (interactive web-based outputs)
    └── Research & Projection (exploratory hypothesis generation)

Specialized Prompts (Use After Master)
    ├── Core Specializations (risk, cognition, operations, AI relationships)
    ├── Visualization Specializations (timeline, graph/schema)
    └── Research Specializations (identity, contradictions)
```

## Category Breakdown

### 1. Core Analysis Category

**Purpose:** Comprehensive memory-only analysis of psychological, cognitive, and behavioral systems.

**Master Prompt:** [`memory_only_psychological_profile.md`](/prompts/core/memory_only_psychological_profile.md)
- Systems-level model across cognition, psychology, behavioral dynamics, identity, motivation, strengths/weaknesses, and AI relationships
- **Use when:** You want a comprehensive starting point for understanding patterns
- **Output:** Structured analysis with confidence labels and evidence/interpretation separation

**Specialized Prompts:**

| Prompt | Focus | Use When |
|--------|-------|----------|
| `behavioral_risk_analysis.md` | Over-optimization, burnout, ideation loops | You need to assess vulnerability areas and risk patterns |
| `cognitive_architecture_analysis.md` | Thinking style, reasoning frameworks, decision-making | You want to understand how decisions are made and problems are approached |
| `founder_operator_profile.md` | Operational patterns, leadership, management approach | You need insights into project management and delegation style |
| `ai_relationship_analysis.md` | AI interaction patterns, communication preferences | You want to understand how the subject interacts with AI systems |

**Decision Tree for Core:**
```
Do you want comprehensive analysis?
    ├─ YES → Use memory_only_psychological_profile.md (Master)
    └─ NO → What specific aspect?
        ├─ Risk factors? → behavioral_risk_analysis.md
        ├─ Thinking style? → cognitive_architecture_analysis.md
        ├─ Work style? → founder_operator_profile.md
        └─ AI interaction? → ai_relationship_analysis.md
```

### 2. Visualization Category

**Purpose:** Generate interactive, visual representations of analysis data.

**Master Prompt:** [`interactive_webapp_generator.md`](/prompts/visualization/interactive_webapp_generator.md)
- Generates complete interactive web-based visualizations
- **Use when:** You want visual outputs and interactive data exploration
- **Output:** HTML/interactive webapp specifications or generation code

**Specialized Prompts:**

| Prompt | Focus | Use When |
|--------|-------|----------|
| `timeline_visualizer.md` | Temporal patterns and progression | You need timeline-based visualizations |
| `graph_schema_generator.md` | Relationship graphs and schema structures | You want network/relationship visualizations |

**Decision Tree for Visualization:**
```
Do you want interactive visualizations?
    ├─ YES → Use interactive_webapp_generator.md (Master)
    └─ What specific type?
        ├─ Timeline? → timeline_visualizer.md
        └─ Network/Schema? → graph_schema_generator.md
```

### 3. Research & Experimental Category

**Purpose:** Exploratory, hypothesis-generating analysis with explicit uncertainty handling.

**Master Prompt:** [`trajectory_projection.md`](/prompts/experimental/trajectory_projection.md)
- Future-direction hypotheses with confidence and uncertainty labels
- **Use when:** You want exploratory analysis, future scenarios, or pattern research
- **Output:** Speculative insights with clear confidence and uncertainty boundaries

**Specialized Prompts:**

| Prompt | Focus | Use When |
|--------|-------|----------|
| `latent_identity_analysis.md` | Identity construction, narrative patterns, self-concept | You want to explore underlying identity assumptions |
| `contradiction_mapper.md` | Paradoxes, inconsistencies, competing patterns | You want to map internal contradictions and tensions |

**Decision Tree for Research:**
```
Do you want exploratory/speculative analysis?
    ├─ YES → Use trajectory_projection.md (Master)
    └─ What aspect?
        ├─ Identity/narrative? → latent_identity_analysis.md
        └─ Contradictions/paradoxes? → contradiction_mapper.md
```

## Usage Workflow

### Recommended Sequence

1. **Start with Master Prompt** (5-10 minute analysis)
   - Choose appropriate master based on your goal
   - Get comprehensive overview
   - Identify areas of interest

2. **Optional: Use Specialized Prompts** (5-15 minutes each)
   - Deep dive into specific aspects
   - Build on master prompt insights
   - Create focused analyses

3. **Optional: Visualize Results** (5-20 minutes)
   - Use visualization master for interactive output
   - Use specialized visualizers for specific formats

### Example Workflows

**Workflow A: Quick Comprehensive Check**
```
memory_only_psychological_profile.md (Master)
→ Read summary
→ Done (5 min)
```

**Workflow B: Targeted Deep Dive**
```
behavioral_risk_analysis.md (Specialized)
→ Identify specific risk areas
→ Done (10 min)
```

**Workflow C: Full Exploration**
```
memory_only_psychological_profile.md (Master)
→ behavioral_risk_analysis.md (Specialized - risks)
→ cognitive_architecture_analysis.md (Specialized - thinking)
→ founder_operator_profile.md (Specialized - operations)
→ interactive_webapp_generator.md (Visualization)
→ Complete analysis with visualizations (30-40 min)
```

**Workflow D: Exploratory Research**
```
trajectory_projection.md (Master)
→ latent_identity_analysis.md (Specialized)
→ contradiction_mapper.md (Specialized)
→ timeline_visualizer.md (Visualization - optional)
→ Speculative insights and research findings (25-35 min)
```

## Constraints & Methodology

All prompts operate under the same core constraints:

- **Memory-Only**: Analysis uses ONLY persistent memory and prior conversations (no internet data, no external profiling)
- **Explicit Uncertainty**: All speculative insights must be labeled with confidence levels
- **Evidence Separation**: Clear distinction between observation, inference, and speculation
- **No Stereotyping**: No demographic assumptions, cultural profiling, or statistical generalizations

See `/docs/methodology.md` for complete methodological details.

## Choosing Your Starting Point

| Goal | Start With |
|------|-----------|
| Comprehensive understanding | `memory_only_psychological_profile.md` |
| Understand decision-making | `cognitive_architecture_analysis.md` |
| Assess vulnerabilities | `behavioral_risk_analysis.md` |
| Understand work style | `founder_operator_profile.md` |
| Understand AI interactions | `ai_relationship_analysis.md` |
| Explore future scenarios | `trajectory_projection.md` |
| Explore identity patterns | `latent_identity_analysis.md` |
| Map contradictions | `contradiction_mapper.md` |
| Get visualizations | `interactive_webapp_generator.md` |
| Timeline visualization | `timeline_visualizer.md` |
| Graph/relationship visualization | `graph_schema_generator.md` |

## FAQ

**Q: Should I always use the master prompt first?**
A: Recommended for first-time users, but experienced users can jump directly to specialized prompts if they know what they need.

**Q: Can I use multiple specialized prompts together?**
A: Yes. They're designed to work sequentially or in parallel. Combining outputs often reveals interesting patterns.

**Q: What if I'm uncertain about which prompt to use?**
A: Start with the master prompt for your category. It will give you enough information to decide if you need specialization.

**Q: How do the specialized prompts relate to the master?**
A: Master prompts provide broad analysis; specialized prompts zoom into specific aspects. Think of it as: Master = landscape view, Specialized = magnified focus.

**Q: Can I skip the master and just use specialized prompts?**
A: Yes, but you lose contextual framing. The master provides the broader system understanding that specialized prompts build on.

## Contributing New Prompts

When adding new prompts, consider:
1. Is this a **master prompt** (comprehensive, broad) or **specialized prompt** (focused, narrow)?
2. Which **category** does it belong to? (core, visualization, experimental)
3. How does it **complement** existing prompts?
4. Update this guide with the new prompt hierarchy

See `/docs/methodology.md` for prompt development guidelines.
