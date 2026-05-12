---
name: highlight-idea-notes
description: Generates small, atomic, Obsidian-ready idea notes from a book's reader-selected highlights, using a separate book context file for accuracy. Use when the user asks to create multiple knowledge-base notes, evergreen notes, ideas, or linked Obsidian notes from book highlights and provides or mentions both highlights and book context/summary paths.
---

# Highlight Idea Notes

## Quick Start

Use this skill to create a set of small Markdown notes from a user's book highlights. Treat the highlights as the primary signal of what mattered to the user, and use the book context only to clarify concepts, relationships, author terminology, and bibliographic reference.

Before writing, verify that the user specified all required inputs:

- Highlights file path.
- Book context or summary file path.
- Output folder path.

If any required input is missing, ask for it before drafting or editing files. Default output language is Spanish from Spain. Keep original-language concepts when they are established terms, book-specific terms, or clearer than a forced translation.

## Workflow

1. Read the highlights file first and identify the strongest recurring ideas, tensions, images, or practical claims.
2. Read the book context file second, using it only to disambiguate and enrich the highlight-driven ideas.
3. Select a set of atomic notes, usually 8 to 16 unless the user asks for another amount.
4. Create the output folder if it does not exist.
5. Write one Markdown file per idea using clear slug filenames in lowercase, preferably without accents.
6. Add internal Obsidian links only when they are useful and point to notes being created or existing nearby notes.
7. Verify every note has a final book reference and does not mention the source files, highlights document, summary document, or task mechanics.

## Source Priority

Prioritize sources in this order:

1. User instructions in the current request.
2. Highlights file: primary evidence of what impacted the user.
3. Book context file: secondary support for conceptual accuracy and bibliography.
4. Existing repository style from nearby notes, if obvious.

Do not turn the output into a general book summary. Ideas that appear only in the context file may be included only when they directly connect highlighted ideas or fill an important conceptual gap.

## Note Shape

Each note should be an evergreen knowledge-base note:

- One idea per file.
- A clear `# Title` that states the concept.
- 2 to 5 short paragraphs, usually 100 to 220 words.
- Direct, pragmatic language.
- Standalone explanation without requiring the reader to know the book structure.
- No quotes unless the exact wording is essential.
- No chapter-by-chapter framing.
- No first-person diary tone.
- A final reference line: `Referencia: [Author], *[Book title]*.`

Use bibliographic details from the context file when reliable. If details are incomplete, include only author and title. Keep references consistent across all generated notes.

## Spanish Style

Write in Spanish from Spain:

- Prefer clear concepts over literary paraphrase.
- Use natural Spanish punctuation and accents in note content.
- Avoid academic padding and generic summaries.
- Avoid phrases like "el autor dice" unless attribution is necessary for precision.
- Preserve terms such as *burnout*, *homo liber*, *animal laborans*, *sharing economy*, *sabbat*, or other original concepts when they carry specific meaning.

## Obsidian Rules

Make the notes easy to link later:

- Use stable, conceptual filenames, for example `autoexplotacion-voluntaria.md`.
- Use internal links sparingly, for example `[[potencia-de-no-hacer]]`.
- Link only to durable concepts, not temporary reading-session labels.
- Do not create index files unless the user asks for one.
- Do not include tags unless the surrounding repository convention clearly uses them or the user requests them.

Avoid formulations like:

- "En los highlights..."
- "El resumen explica..."
- "En el archivo..."
- "Esta nota viene de..."
- "El capítulo X trata..."

## Quality Checklist

Before finishing, verify:

- Required paths were specified or requested from the user.
- The highlights drove the note selection.
- The context file improved accuracy without dominating the output.
- Each file contains one atomic idea.
- Every note is in Spanish from Spain, with original-language concepts preserved when appropriate.
- Every note has the final book reference.
- No note refers directly to highlights, summaries, files, chapters, or the generation task.
- Internal links point to sensible note filenames.
- Files were written to the requested output folder.
