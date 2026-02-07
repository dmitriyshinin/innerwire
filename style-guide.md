# Style Guide / Руководство по стилю

## Tone / Тон

- **Accessible** — understandable without specialized education
- **Respectful** — never condescending, never "let me explain this simply for you"
- **Direct** — say what you mean, avoid hedging and filler
- **Honest** — if evidence is weak, say so; if something is a hypothesis, call it that

## Language / Язык

- English is the source of truth. Russian follows.
- Root-level project files (README.md, CONTRIBUTING.md) are bilingual inline.
- Layer content files are separate per language (`/en/`, `/ru/`).
- Scientific terms: use English terms with Russian translation on first mention, then consistently use glossary terms (see `translations/glossary.yml`).
- Don't translate author names, journal titles, or book titles.

## Structure: description.md

1. **Title** — short, evocative (e.g., "Your nervous system: three modes")
2. **Core idea in one sentence** — the entire layer summarized
3. **Explanation** — what this system is, how it works (2-3 paragraphs)
4. **Manifestations** — how each pattern/axis shows up in daily life (bulleted lists)
5. **"This is not a type" disclaimer** — emphasize spectrums, malleability
6. **Common patterns** — named regions on the spectrum with descriptions
7. **What shapes your pattern** — factors (early experience, stress, environment, practice)
8. **Deep-dive** — collapsible `<details>` section with theory details and criticism

## Structure: questionnaire.md

1. **Framing** — "This is a self-observation tool, not a clinical test"
2. **Instructions** — based on last 2-3 months, honest answers
3. **Parts** — multiple sections measuring different aspects
4. **Interpretation** — guidance on understanding results
5. **Disclaimer** — not a diagnosis, seek professional help if needed

## Structure: practices.md

1. **Principle** — overarching goal (e.g., "expand access, increase flexibility")
2. **Foundational practice** — one practice for everyone
3. **Pattern-specific practices** — grouped by self-observed pattern
4. **Each practice includes:** what to do, why it works (with science), duration/frequency
5. **General recommendations** — start small, consistency over intensity, stop if discomfort
6. **Observation journal template** (optional)

## Structure: sources.md

1. **Key works** — grouped by topic, APA format
2. **Criticism section** — always present
3. **Note on scientific honesty** — our approach to sources
4. **Link to detailed bibliography** in `/research/`

## Formatting conventions

- Use `###` for subsections within a file (not `#` — that's the file title only)
- Use `---` horizontal rules to separate major sections
- Use `> ⚠️` for important warnings
- Use `<details><summary>` for deep-dive / technical content
- Use `- [ ]` checkboxes in questionnaires
- Use bold `**text**` for emphasis, not ALL CAPS
- One blank line between paragraphs, two blank lines before `---` separators
- No trailing whitespace
- Files end with a single newline
