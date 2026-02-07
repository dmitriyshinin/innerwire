# Translation Guide / Руководство по переводу

## Source of truth

English (`/en/`) is the source of truth. Russian (`/ru/`) follows. When content is updated in English, Russian should be updated to match.

## Principles

1. **Accuracy over fluency** — don't sacrifice meaning for smooth phrasing
2. **Consistent terminology** — always use terms from `glossary.yml`
3. **Cultural adaptation** — questionnaires may need cultural adaptation, not just literal translation (e.g., examples of stressful situations should be culturally relevant)
4. **Don't translate:** author names, journal titles, book titles, scientific terms that have no established Russian equivalent

## Workflow

1. Content is written in English first
2. Russian translation is created following the same structure
3. Both versions are committed together when possible
4. If only one language is available, commit it and open an issue for translation

## Metadata

Each layer directory should maintain version parity tracked in `translations/status.yml`.

Statuses:
- `synced` — translation matches current source version
- `outdated` — source has been updated, translation needs update
- `missing` — no translation exists yet

## Adding a new language

1. Open an issue proposing the language
2. Create `/xx/` directory (ISO 639-1 code)
3. Mirror the `/en/` structure
4. Translate layer by layer (each layer = separate PR)
5. Add language to `status.yml`
6. Update root README.md with language link

## What NOT to translate

- Scientific citations (keep original language)
- Author names
- Questionnaire scoring numbers
- File names and directory names
- Code examples or technical markup
