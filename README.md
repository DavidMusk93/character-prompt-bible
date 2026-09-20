# Character Prompt Bible

A model-agnostic visual identity system for recurring anime characters and scenes.

## Goal

Keep the same four characters visually recognizable across different image agents and models.

This repository treats prompts as only one layer of identity. The canonical source of truth is:

1. **Reference images**
2. **Structured character specification**
3. **Shared visual-style specification**
4. **Scene constraints**
5. **Model-specific adapter prompts**

The priority order is:

```
reference image > character spec > style spec > scene prompt > model-specific keywords
```

## Core characters

- `anzai` — 安仔
- `xiner` — 心儿
- `mom` — 妈妈
- `grandma` — 奶奶

## Repository layout

```
characters/     Canonical identity definitions
style/          Shared art direction and invariants
prompts/        Model-neutral prompt templates
adapters/       Model / image-agent specific translation rules
references/     Reference-sheet requirements and asset conventions
scenes/         Reusable scene specifications
```

## Stability rule

Do not encode a character's identity primarily in prose such as "cute anime boy".

Each character must have a stable set of immutable visual anchors:

- face geometry
- hair silhouette
- eye geometry
- body proportions
- signature color palette
- signature clothing silhouette
- age appearance
- distinguishing visual feature(s)

Scene prompts may change pose, expression, lighting, camera, environment and props. They should not redefine immutable anchors.

## Versioning

Character identities use explicit versions:

```
anzai-v1
xiner-v1
mom-v1
grandma-v1
```

Any intentional change to an immutable identity field creates a new version. Scene-level changes do not.

## Current status

The system structure is initialized. The four character files intentionally avoid inventing facial details that have not yet been approved. Fill them from canonical reference images before treating v1 as locked.
