# CLAUDE.md — Instructions for AI agents

## Project overview

InnerWire is a science-based open-source framework for self-awareness. It provides individual profiles across multiple axes grounded in peer-reviewed neuroscience, physiology, and psychology research. The core idea: your profile is not a fixed label but a starting point — understand how you work, see what influences it, and get concrete tools to change what isn't working.

## Repository structure

```
/
├── en/                    # English content (source of truth)
│   ├── README.md          # English guide
│   ├── quick-profile/     # "Mirror" level — quick profile across all axes
│   └── model/
│       └── layer-N-xxx/   # "Map" level — each layer: description, questionnaire, practices, sources, README
│                          # "Lab" level — deep-dive.md within each layer
├── ru/                    # Russian content (translation)
│   ├── README.md
│   ├── quick-profile/
│   └── model/
│       └── layer-N-xxx/
├── research/              # Bibliography and annotated sources (Lab level)
├── templates/             # Layer template for consistent structure
├── translations/          # Translation status, glossary, guide
├── README.md              # Root bilingual README
├── CONTRIBUTING.md        # Contribution guidelines
├── architecture.md        # Model architecture
├── roadmap.md             # Development roadmap
├── style-guide.md         # Content style guide
└── LICENSE                # CC BY-SA 4.0
```

## Two axes of the model

**Layers (vertical):** five independent aspects — autonomic, interoception, sensory, attachment, allostatic load. Each is self-contained.

**Depth levels (horizontal):** three levels of detail that cut across all layers:
- **Mirror** — quick profile, self-recognition, starter practices (~20 min)
- **Map** — full explanations, questionnaires, detailed practices
- **Lab** — full scientific basis, criticism, primary sources

## Five principles (always follow)

1. **Scientific basis** — every claim must reference peer-reviewed research. No opinions, no pop-psychology without citations.
2. **Spectrums, not types** — never assign discrete types. Use continuums, axes, zones.
3. **Layers** — each layer is self-sufficient. Don't require knowledge of other layers.
4. **Dynamic** — profiles change. Never write "you ARE this type." Write "your current pattern tends toward..."
5. **Open** — acknowledge limitations, include criticism of theories used.
6. **Agency over identity** — the reader is the author. Show where they are, what shaped it, and what they can change. Provide tools, not labels.

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
