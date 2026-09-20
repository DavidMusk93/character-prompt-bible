# Base Character Prompt Template

Use this template for a single recurring character.

```text
Use the canonical identity of {{character_id}}.

Preserve all immutable identity anchors:
{{immutable_anchors}}

Apply visual style:
{{style_id}}

Do not redesign the character.
Do not reinterpret age, ethnicity, facial geometry, hairstyle silhouette,
body proportions, or signature outfit.

Scene:
{{scene}}

Action:
{{action}}

Expression:
{{expression}}

Camera:
{{camera}}

Lighting:
{{lighting}}

Global negative constraints:
{{negative_constraints}}
```

## Rule

The scene may change pose, expression, lighting, and environment.
It must not silently alter permanent character traits.
