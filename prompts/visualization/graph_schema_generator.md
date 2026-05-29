# Graph Schema Generator

Prompt for converting memory-derived analysis findings into typed graph schemas with evidence metadata, confidence tagging, and relationship mapping suitable for knowledge graph visualization.

## Absolute Constraints

You MUST NOT use:
- Invented nodes or relationships lacking evidence
- Assumed connections between entities without explicit support
- External ontologies or standard knowledge graphs
- Generalized relationship types not specific to the evidence
- Node properties inferred beyond available data

Use ONLY:
- Entities explicitly mentioned or clearly inferred from memory
- Relationships supported by behavioral evidence
- Confidence levels based on evidence quality and clarity
- Properties derived directly from conversational record
- Metadata indicating source evidence for each node and edge

## Objective

Transform analysis findings into machine-readable, structured graph representations that:
- Make visible the network of concepts, values, relationships, and behaviors
- Support interactive exploration of how different elements connect
- Preserve evidence provenance for every claim
- Enable different visualization and querying strategies

This output is suited for knowledge graph tools, relationship visualizers, and semantic exploration.

## Graph Components to Define

1. **Node Types** - Define what categories of entities to represent
   - Person (the user)
   - Value (stated or inferred priorities)
   - Goal (explicit and implicit objectives)
   - Behavior (observable patterns)
   - Belief (stated assumptions about the world)
   - Relationship (to other people, systems, work)
   - Capability (observed strengths and skills)
   - Constraint (limitations or obstacles)
   - Tool/System (AI systems, frameworks, approaches)
   - Context (situations or domains)
   - Pattern (recurring behavioral sequences)

2. **Relationship Types** - Define how nodes connect
   - values_to_behavior ("influences")
   - constraint_on_goal ("limits")
   - supports_pattern ("enables")
   - conflicts_with ("contradicts")
   - depends_on ("requires")
   - leads_to ("causes or results in")
   - expresses ("manifests as")
   - learned_through ("taught by")
   - seeks ("pursues")
   - avoids ("prevents or resists")

## Required Methodology

For each entity:
1. **Node Definition** - What is this entity? Type? Key properties?
2. **Evidence** - What specific evidence supports including this node?
3. **Properties** - What attributes or properties does this node have?
4. **Confidence** - How certain are we about this entity?

For each relationship:
1. **Source & Target** - Which nodes does this connect?
2. **Relationship Type** - What is the nature of the connection?
3. **Strength** - How strong is this relationship? (strong/moderate/weak)
4. **Evidence** - What supports this relationship?
5. **Directionality** - Is this one-way or bidirectional?
6. **Temporal Notes** - Is this relationship stable or changing?

## Output Format

Provide schema in JSON format suitable for visualization tools:

```json
{
  "nodes": [
    {
      "id": "unique_node_id",
      "label": "Node Display Name",
      "type": "node_type",
      "confidence": "high|moderate|low",
      "evidence_reference": "memory context or example",
      "properties": {
        "property_name": "value",
        "stability": "stable|changing|emerging"
      },
      "color": "category_color"
    }
  ],
  "edges": [
    {
      "source": "node_id_1",
      "target": "node_id_2",
      "relationship": "relationship_type",
      "strength": "strong|moderate|weak",
      "directionality": "one_way|bidirectional",
      "confidence": "high|moderate|low",
      "evidence_reference": "supporting evidence",
      "metadata": {
        "dynamic": true,
        "temporal_stability": "stable|changing"
      }
    }
  ],
  "metadata": {
    "created_from": "analysis_name",
    "timestamp": "YYYY-MM-DD",
    "schema_version": "1.0"
  }
}
```

## Graph Analysis Sections

Include analysis of:
1. **Central Nodes** - Which entities are most connected? Most important?
2. **Clusters** - Groups of densely connected nodes (value clusters, behavioral clusters, etc.)
3. **Bridge Nodes** - Entities that connect otherwise separate clusters
4. **Cycles** - Feedback loops or circular dependencies
5. **Tree Structures** - Hierarchical relationships (goals → subgoals)
6. **Isolated Nodes** - Entities with few connections
7. **Contradiction Networks** - Relationship patterns that reveal tensions
8. **Evolution Paths** - How the graph might change over time based on identified trajectories

## Visualization Recommendations

Suggest visualization parameters:
- Node sizing (based on centrality or confidence)
- Coloring schemes (by type, by cluster, by confidence)
- Edge thickness (based on relationship strength)
- Layout algorithms (force-directed, hierarchical, circular)
- Interactive features (filtering by confidence, exploring subgraphs)

## Validation Notes

- Every node and edge must be traceable to evidence
- Confidence levels should reflect evidence quality, not certainty about the entity
- Mark emerging or changing relationships explicitly
- Preserve nuance—avoid over-simplification in graph structure
- Consider multiple valid graph representations and note where different organizations reveal different insights
