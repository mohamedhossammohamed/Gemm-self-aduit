# Interactive Self-Analysis Visualization - Single Artifact HTML Generator Prompt

Generate a modern interactive visualization as a **single standalone HTML file** that visualizes findings from a memory-only AI psychological and behavioral analysis.

## Critical Constraint

Analysis MUST originate exclusively from Gemini persistent memory and saved conversational context.

The system MUST NOT use internet search, external APIs, retrieval augmentation, demographic priors, or generalized personality templates.

## Technical Stack (All Bundled in Single HTML)

- Vanilla JavaScript (ES6+)
- HTML5 Canvas & SVG for graphics
- Tailwind CSS (CDN)
- Framer Motion (CDN)
- D3.js or Chart.js (CDN) for data visualization
- shadcn/ui components (via CDN or inline)
- All dependencies loaded via CDN or embedded inline

## Required Visual Systems

1. **Cognitive Architecture Graph** - Interactive node-link diagram of thought patterns
2. **Behavioral Timeline** - Chronological event visualization with markers
3. **Contradiction Mapper** - Conflict/paradox visualization network
4. **AI Relationship Interface** - Interaction history heatmap
5. **Risk Heatmap** - Concern areas highlight system
6. **Identity Vector Space** - Multi-dimensional projection visualization

## Single HTML Artifact Requirements

Generate:
1. **Complete HTML structure** - All UI in one document
2. **Embedded CSS** - Tailwind via CDN + inline styles
3. **Self-contained JavaScript** - All logic in `<script>` tags
4. **Data Input Section** - Textarea/file input for analysis JSON
5. **Visualization Canvas** - Dedicated render areas for each system
6. **Mock Data Generator** - Function to create sample analysis JSON
7. **Export Functionality** - Download visualization as PNG/SVG
8. **Local-only Architecture** - No API calls, all processing client-side
9. **Privacy-Preserving Design** - Data never leaves browser, optional localStorage only
10. **Responsive Layout** - Mobile/tablet friendly single-page experience

## Deliverable Format

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- All CDN links, inline styles -->
  </head>
  <body>
    <!-- Single page UI -->
    <!-- Input controls -->
    <!-- Visualization containers -->
    <!-- Script with all logic -->
  </body>
</html>
```

The file works completely standalone - no build step, no dependencies to install, no server needed. Open directly in any modern browser.

## Mock Analysis JSON Structure

```json
{
  "timestamp": "2026-05-29T12:00:00Z",
  "cognitive_patterns": {
    "primary_modes": ["analytical", "creative", "relational"],
    "bias_tendencies": [],
    "contradiction_clusters": []
  },
  "behavioral_events": [
    {
      "timestamp": "...",
      "category": "interaction|learning|conflict",
      "intensity": 0.0-1.0,
      "description": ""
    }
  ],
  "relationship_matrix": {},
  "risk_factors": {},
  "identity_vectors": {}
}
```
