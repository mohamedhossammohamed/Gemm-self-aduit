# Timeline Visualizer

Prompt for mapping events, decisions, and pattern evolution across conversational history into structured chronological representations with explicit uncertainty intervals.

## Absolute Constraints

You MUST NOT use:
- Timeline templates that imply causality not evidenced
- Assumptions about event significance based on external importance metrics
- Filling gaps with inferred events lacking explicit evidence
- Causal narratives without clear supporting evidence
- Linear narratives that oversimplify actual complexity

Use ONLY:
- Events explicitly mentioned with dates or temporal references
- Events with clear evidence of impact on behavior or thinking
- The actual sequence and relative timing from memory
- Uncertainty markers where exact timing is unclear
- Spatial relationships between events based on conversational record
- Evidence of how the user experienced temporal progression (subjective vs. objective time)

## Objective

Create structural chronological maps of the user's conversational history that make visible:
- Key events and decisions across time
- Temporal clustering of certain types of decisions or realizations
- Evolution of patterns over the conversation timeline
- Gaps or uncertain periods
- Acceleration or deceleration of change at different points

This is NOT narrative creation. It is visualization of the evidence that exists in temporal sequence.

## Timeline Elements to Map

1. **Explicit Events** - Decisions, milestones, significant moments mentioned with dates
2. **Behavioral Shifts** - Changes in pattern visible as conversation progresses
3. **Realization Moments** - Points where stated understanding changed or deepened
4. **Decision Clusters** - Groups of related decisions made in close temporal proximity
5. **Stable Periods** - Extended times of consistent patterns
6. **Transition Zones** - Times when multiple patterns were shifting simultaneously
7. **Crisis or Inflection Points** - Moments with significant impact on subsequent patterns
8. **Cyclical Patterns** - Events or decisions that repeat at temporal intervals
9. **Unresolved Periods** - Times when outcome is still unknown or in progress

## Required Methodology

For each timeline element:
1. **Event Description** - What happened or changed?
2. **Temporal Positioning** - When did this occur? (Specific date, relative timing, or uncertainty range)
3. **Evidence Source** - How do we know about this from memory?
4. **Impact Assessment** - What shifted as a result?
5. **Confidence in Timing** - High/moderate/low certainty about when this occurred
6. **Causal Relationships** - What events preceded and followed? (Avoid assuming causality)

## Output Format

Should include:
1. **Master Timeline** - Chronological list of all mapped events and pattern shifts
2. **Temporal Clusters** - Groups of related events occurring in similar timeframes
3. **Pattern Evolution Arc** - How key behavioral patterns have changed over the timeline
4. **Inflection Point Analysis** - Moments with significant downstream impacts
5. **Cyclical Pattern Map** - Any patterns that repeat on identifiable intervals
6. **Uncertainty Zones** - Periods where timing or sequence is unclear
7. **Narrative Threads** - Major storylines or themes that unfold across the timeline
8. **Velocity Map** - Where change is accelerating, slowing, or steady
9. **Decision Sequence** - How successive decisions relate to each other temporally
10. **Visualization Ready JSON/Schema** - Structured data suitable for graph or timeline visualization

## Visualization Data Structure

Include machine-readable output suitable for visualization tools:
```
{
  "timeline_events": [
    {
      "id": "event_id",
      "description": "...",
      "start_date": "YYYY-MM-DD or null",
      "end_date": "YYYY-MM-DD or null",
      "confidence": "high|moderate|low",
      "event_type": "decision|realization|shift|milestone",
      "impact_level": "high|moderate|low",
      "relationships": ["event_id_1", "event_id_2"]
    }
  ]
}
```

## Critical Notes

- Mark every date-related claim with explicit uncertainty level
- When exact dates are unknown, provide relative positioning ("after X", "before Y", "during Z period")
- Distinguish between "I know this happened" and "I infer this must have happened"
- Avoid narrative smoothing—preserve actual messiness and contradiction
- Flag where timeline reveals patterns that weren't obvious in non-chronological analysis
