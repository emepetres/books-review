# Essay Book Notes Reference

## Banned Meta-Narrative

Do not write formulations like:

- "This introduces..."
- "The chapter explains..."
- "The chapter emphasizes..."
- "This section describes..."
- "Throughout the chapter..."

Every idea must be written as a direct claim about the domain, not as a comment about what the text does.

## Explicit Structure Pattern

Use brief paragraphs for single claims, conclusions, and causal relations. Use lists for categories, causes, effects, symptoms, types, or multi-part concepts.

Preferred pattern:

```md
*Organizational pressure degrades technical quality when it changes everyday incentives.* Its main effects are:

- **Reduced learning**: the team repeats familiar decisions even when the context has changed.
- **Invisible debt**: future costs remain outside immediate metrics.
- **Operational fragility**: systems depend on manual coordination and tacit knowledge.
```

Avoid compressing several categories, symptoms, causes, or effects into one dense paragraph when a list would be clearer.

## Chapter Relationships

Each chapter section ends with `### Relationships With Other Chapters`.

Relationship rules:

- Reference only chapters from the same attached book.
- Use brief factual relations such as `reinforces`, `expands`, `contrasts with`, `depends on`, `anticipates`, or `returns to`.
- Do not introduce new ideas in this block.
- Do not add broad interpretive comparisons.

Example:

```md
### Relationships With Other Chapters

- **Chapter 2**: expands the relationship between organizational incentives and technical quality.
- **Chapter 5**: returns to the dependency between tacit knowledge and operational fragility.
```

## Stability Checklist

Before finalizing, verify:

- The number of summary sections equals the number of extracted chapters.
- Chapter titles and order match the attached book exactly.
- Each section maps to one chapter only.
- Repeated ideas are summarized in every chapter where they appear.
- Examples are included only when clearly present in the chapter.
- The final thematic-note suggestions are separate from the main summary.
