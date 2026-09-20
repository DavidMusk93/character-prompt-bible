# Scene Records

Store one Markdown file per important generated scene or illustration set.

Recommended metadata:

```yaml
scene_id: toys-cleanup-v1
characters:
  - anzai-v1
  - mom-v1
style: family-anime-v1
agent: <agent-name>
model: <model-version-if-known>
reference_images:
  - <approved-reference>
aspect_ratio: 16:9
seed: <if-supported>
date: YYYY-MM-DD
```

Then record:
- final prompt
- model-specific adapter settings
- selected output
- observed drift
- corrections needed

This history is useful when migrating to a different image agent.
