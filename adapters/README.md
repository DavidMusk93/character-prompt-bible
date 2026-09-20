# Agent Adapters

Adapters translate the model-agnostic character bible into image-agent-specific syntax.

Examples:

```text
adapters/chatgpt-image.md
adapters/higgsfield.md
adapters/midjourney.md
adapters/flux.md
```

## Rule

Adapters may change:
- syntax
- ordering
- weighting
- reference-image instructions
- aspect-ratio syntax
- negative-prompt syntax

Adapters may **not** change canonical character identity.

This makes migration between image agents explicit and reviewable.
