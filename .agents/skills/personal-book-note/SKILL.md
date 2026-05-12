---
name: personal-book-note
description: Creates one concise, personal, Obsidian-ready Markdown note about a book the user has read, driven primarily by reader highlights and supported by a book summary. Use when the user asks for a personal reading note, reminder, reflection, or short article from book highlights plus a Markdown summary, or when no highlights exist but the user specifies the themes to focus on.
---

# Personal Book Note

## Purpose

Create one short Markdown note that helps the user remember what personally mattered most about a book. The note should capture the ideas reflected in the user's highlights, not summarize the whole book.

The note is intended for an Obsidian knowledge base, so it must be readable as a standalone conceptual note. Do not mention the input files, the highlight list, the summary file, or the generation process.

## Required Inputs

Before drafting or editing files, verify that the user provided:

- Output file path for the Markdown note.
- Book summary Markdown file path.
- Highlights Markdown file path, unless the user explicitly says no highlights are available.

If the highlights file is missing and the user did not say highlights are unavailable, ask for it. If no highlights are available, ask the user for the themes, questions, or ideas the note should focus on. If the summary file is missing, ask for it.

Default output language is Spanish from Spain unless the user specifies another language.

## Source Priority

Use sources in this order:

1. Current user instructions, including requested focus, tone, length, title, language, and output path.
2. Highlights: primary evidence of what impacted the user.
3. User-specified themes when no highlights exist.
4. Book summary: context for accuracy, terminology, and source reference.

Do not add major ideas that appear only in the book summary unless they directly clarify, connect, or frame highlighted ideas. The output should be highlight-driven, not summary-driven.

## Workflow

1. Read the highlights first, if available.
2. Identify 2 to 4 central ideas, tensions, or questions that appear strongest in the highlights.
3. Read the book summary only to clarify concepts, relationships, and bibliographic details.
4. Draft one concise note around the selected ideas.
5. Write the note to the exact output path specified by the user.
6. Verify the note does not reference the input files, highlights, summary, chapters, or task mechanics.

## Note Shape

Use this structure unless the user asks otherwise:

```md
# [Conceptual title]

[Brief opening paragraph stating the main idea of the note.]

## [Short section title]

[1-2 short paragraphs.]

## [Short section title]

[1-2 short paragraphs.]

## [Optional short section title]

[1-2 short paragraphs.]

Referencia: [Author], *[Book title]*.
```

Guidelines:

- Usually 250 to 350 words, or shorter if the highlighted idea is narrow.
- Use 1 to 3 sections maximum.
- Prefer short paragraphs and direct claims.
- Use pragmatic, readable language.
- Avoid academic padding, exhaustive coverage, and chapter-by-chapter summaries.
- Avoid diary-like over-personalization unless the user asks for it.
- Do not include quotations unless exact wording is essential.
- Preserve important original terms when they are clearer than translation or are book-specific concepts.

## Style Rules

Write as a personal reading note, not as a review, book report, or full summary.

The note should answer:

- What ideas seem to have mattered most to the reader?
- Why are those ideas important?
- What useful distinction, warning, or question should the reader remember later?

When the source book uses dense, philosophical, academic, or difficult language, simplify the explanation while preserving the original distinctions. The goal is for the note to be easy to reread quickly.

## Obsidian Rules

- Make the note standalone and linkable.
- Use a conceptual title, not necessarily the book title.
- Do not mention source file paths or phrases like "in the highlights", "the summary says", or "this file".
- Do not include tags unless the user requests them or the nearby repository clearly uses them.
- Include exactly one final source reference line using the best bibliographic information available from the summary.

## Quality Checklist

Before finishing, verify:

- The output file was written to the requested path.
- The note is mainly driven by highlights or by user-provided themes when highlights are unavailable.
- The book summary is used as context, not as the main structure.
- The note is brief, clear, and easy to reread.
- The note does not summarize the whole book unless the highlights genuinely require it.
- The note does not mention input files, highlights, summaries, chapters, or task mechanics.
- The note ends with a source reference to the book.
- The language is Spanish from Spain unless another language was requested.
