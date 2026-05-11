---
name: essay-book-notes
description: Generate faithful, structured Obsidian-ready notes in the source book's language from attached nonfiction essay books, especially software development, engineering management, and philosophy. Use when the user attaches a full PDF or EPUB book and asks for book notes, chapter summaries, Obsidian notes, blog source notes, or reusable summaries.
---

# Essay Book Notes

## Quick Start

When a user provides a complete PDF or EPUB nonfiction book, produce one Markdown note in the same language as the source book that mirrors the book's chapter structure exactly. Use only the attached book as the source of truth.

Never rely on prior knowledge of the title, other editions, reviews, summaries, or known canonical structures. If the attached file differs from outside knowledge, the attached file wins.

## Workflow

1. Extract bibliographic metadata from the attached book: full title, author(s), edition if identifiable, and publication year if identifiable.
2. Extract the table of contents exactly as it appears in the attached book: preserve chapter order, chapter numbers, and title text. Treat this table of contents as the only structural source of truth.
3. Before drafting, verify structural alignment: same number of planned sections as extracted chapters, same order, one section per chapter, and no chapters merged, split, skipped, renamed, or reordered.
4. For each chapter, follow the same stable process: identify key concepts, explain each concept explicitly, convert implicit enumerations into explicit lists, draft without personal prioritization, and identify factual links to other chapters in the same book.
5. After the chapter summaries, propose 3 to 6 possible derived thematic notes.

## Markdown Output

Start with one global book reference only:

```md
# [Full Book Title]

**Reference**: [Author(s)]. [Full Book Title]. [Edition, if any]. [Year, if identifiable].
```

Then create exactly one section per chapter, in the original order. Localize fixed headings and labels to the source book's language:

```md
## [Chapter number and exact title]

[Chapter notes]

### [Localized equivalent of "Relationships With Other Chapters"]

- **[Localized chapter label] X**: [brief factual relation: reinforces, expands, contrasts with, depends on, anticipates, returns to].
```

Do not include bibliographic references inside chapter sections.

## Chapter Writing Rules

Write in the same language as the source book, using an impersonal, declarative, timeless style suitable for knowledge-base material. Avoid meta-narrative and comments about the text.

Keep the prose pragmatic, readable, and easy to understand. When the source language is dense, archaic, academic, or philosophically difficult, slightly adapt the wording for clarity while preserving the original meaning, scope, and distinctions.

Do not write formulations like "This introduces...", "The chapter explains...", "The chapter emphasizes...", "This section describes...", or "Throughout the chapter...".

Write direct claims about the domain instead. Use brief paragraphs for single claims, conclusions, and causal relations. Use lists for real enumerations. Mark central ideas in *italics*. For list items, name each element in **bold**, followed by an inline explanation after a colon.

Avoid compressing several categories, symptoms, causes, or effects into one dense paragraph when a list would be clearer.

## Coverage And Length

Summarize all relevant ideas from each chapter with controlled exhaustiveness. Do not select only subjectively representative ideas.

Use proportional length by chapter density: short chapters 120 to 180 words, medium chapters 180 to 250 words, and long or dense chapters 250 to 350 words.

Repeat an idea in every chapter where it appears, according to that chapter's specific treatment. Do not consolidate repeated ideas globally.

## Fidelity Rules

Derive all content exclusively from the attached book. Do not fill gaps with external knowledge. Do not add ideas unless they are clearly present in the corresponding chapter. Do not reorganize concepts globally or add interpretive comparisons between chapters. Use examples only when they clearly appear in the chapter, and keep them brief and abstract.

In case of conflict, prioritize structural fidelity, schematic clarity, and reproducible consistency over creative synthesis or excessive compression.

## Final Thematic Notes

After the complete summary, add a localized equivalent of `## Possible Derived Thematic Notes` with 3 to 6 suggested derivative notes. These are suggestions only, not replacements for the chapter-aligned summary.
