# Architecture / Архитектура

## What is a layer / Что такое слой

InnerWire is built as a stack of independent layers. Each layer describes one aspect of how your body and mind work — backed by a specific field of research. Layers don't depend on each other: you can use any single layer and get value. But together they form a richer picture.

InnerWire построен как стек независимых слоёв. Каждый слой описывает один аспект работы тела и психики, опираясь на конкретную область исследований. Слои не зависят друг от друга: любой из них полезен сам по себе. Но вместе они дают более полную картину.

## The five layers / Пять слоёв

| Layer | Name | What it measures | Scientific basis | Status |
|-------|------|------------------|------------------|--------|
| 0 | Autonomic Profile | Three modes of the nervous system (connection, mobilization, freeze) | Polyvagal Theory (Porges), HRV research | 🟡 draft |
| 1 | Interoceptive Profile | How well you sense and interpret body signals | Barrett, Craig, Critchley & Garfinkel | 🟡 draft |
| 2 | Sensory Profile | How you process sensory input from the environment | Dunn's Sensory Processing Framework | 🟡 draft |
| 3 | Attachment Pattern | How you build and maintain closeness with others | Bowlby, Ainsworth, Bartholomew, ECR-R | 🟡 draft |
| 4 | Allostatic Load | Cumulative stress burden on body systems | McEwen, Sterling, Juster | 🟡 draft |

## Layer ordering rationale / Почему такой порядок

The layers are ordered from most physiological (bottom) to most psychological (top), and from least conscious to most conscious:

- **Layer 0** (Autonomic) — operates below awareness, milliseconds
- **Layer 1** (Interoception) — body signals reaching awareness
- **Layer 2** (Sensory) — processing external stimuli
- **Layer 3** (Attachment) — relational patterns, shaped over years
- **Layer 4** (Allostatic Load) — cumulative result of all the above over time

This is not a hierarchy of importance. It's a progression from "what your body does automatically" to "what accumulates over your lifetime."

## How layers interact / Как слои взаимодействуют

Layers are independent but influence each other:

- **0 → 1:** Your autonomic state affects interoceptive accuracy (hard to sense subtle body signals in mobilization mode)
- **1 → 0:** Better interoception helps regulate autonomic states
- **0 → 3:** Autonomic patterns shaped by early attachment experiences
- **2 → 0:** Sensory overload can trigger mobilization or freeze
- **All → 4:** Chronic dysregulation in any layer contributes to allostatic load
- **4 → All:** High allostatic load degrades functioning across all layers

These connections will be documented in cross-reference sections as layers mature.

## File structure per layer / Структура файлов слоя

Each layer contains 5 files (in each language):

```
layer-N-name/
├── README.md          # Quick start: 3 steps, connection to other layers
├── description.md     # Core concepts, daily-life manifestations, patterns, deep-dive
├── questionnaire.md   # Self-observation tool (NOT a clinical test)
├── practices.md       # Actionable exercises for each pattern
└── sources.md         # Key citations + link to research/
```

See `templates/layer-template/` for the canonical structure.

## Design principles / Принципы проектирования

### Spectrums, not types
Every layer uses continuous axes, not discrete categories. When we name "patterns" or "zones," these are convenient labels for regions of a continuous space — not boxes to put people in.

### Self-contained layers
A reader should be able to read one layer, do the questionnaire, try the practices, and get value — without reading anything else.

### Honest about limitations
Every layer's description.md includes a section on criticism and limitations of the underlying theory. We don't hide inconvenient research.

### Practical
Theory is only useful if it leads to action. Every layer includes concrete practices matched to the reader's self-observed pattern.
