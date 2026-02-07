# CLAUDE.md — Instructions for AI agents

## Project overview

InnerWire is a science-based open-source framework for self-awareness. It provides individual profiles across multiple axes grounded in peer-reviewed neuroscience, physiology, and psychology research. It is an alternative to pseudoscientific typologies (MBTI, Socionics, Human Design).

## Repository structure

```
/
├── en/                    # English content (source of truth)
│   ├── README.md          # English guide
│   └── model/
│       └── layer-N-xxx/   # Each layer: description, questionnaire, practices, sources, README
├── ru/                    # Russian content (translation)
│   ├── README.md
│   └── model/
│       └── layer-N-xxx/
├── research/              # Bibliography and annotated sources
├── templates/             # Layer template for consistent structure
├── translations/          # Translation status, glossary, guide
├── README.md              # Root bilingual README
├── CONTRIBUTING.md        # Contribution guidelines
├── architecture.md        # Model architecture
├── roadmap.md             # Development roadmap
├── style-guide.md         # Content style guide
└── LICENSE                # CC BY-SA 4.0
```

## Five principles (always follow)

1. **Scientific basis** — every claim must reference peer-reviewed research. No opinions, no pop-psychology without citations.
2. **Spectrums, not types** — never assign discrete types. Use continuums, axes, zones.
3. **Layers** — each layer is self-sufficient. Don't require knowledge of other layers.
4. **Dynamic** — profiles change. Never write "you ARE this type." Write "your current pattern tends toward..."
5. **Open** — acknowledge limitations, include criticism of theories used.

## Content rules

- **English is source of truth.** Write EN first, then RU.
- **Bilingual root files** (README.md, CONTRIBUTING.md) use inline bilingual format.
- **Layer files** are separate per language in `/en/` and `/ru/`.
- **Tone:** accessible, respectful, never condescending. No jargon in main text; technical details in collapsible `<details>` blocks.
- **Structure per layer:** README.md → description.md → questionnaire.md → practices.md → sources.md. Follow `templates/layer-template/`.
- **Sources format:** APA-style citations. Include criticism alongside supporting research.
- **Questionnaires** are self-observation tools, NOT clinical tests. Always include disclaimer.

## Terminology

Use consistent terms from `translations/glossary.yml`. Key examples:
- "mode" not "state" or "type" (for autonomic states)
- "pattern" not "type" (for behavioral tendencies)
- "spectrum" or "axis" not "category"

## Commits

- `feat:` — new layer content
- `docs:` — architecture, guides, meta-files
- `fix:` — corrections to existing content
- `refactor:` — restructuring without content change
- `cleanup:` — removing unused files

## What NOT to do

- Don't invent scientific claims. If unsure about research, mark as hypothesis.
- Don't translate scientific author names or journal titles.
- Don't create new layers without research basis.
- Don't use emojis in body text (only in tables for status indicators).
