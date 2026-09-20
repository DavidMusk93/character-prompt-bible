# ChatGPT Image Adapter

Use the approved reference sheet as the primary identity anchor whenever image reference is available.

## Assembly order

1. identify the exact character version
2. attach or reference the approved character sheet
3. include only the immutable anchors needed to reinforce identity
4. apply the shared visual style
5. add scene, action, expression, camera, and lighting
6. include global negative constraints

## Rule

Do not re-invent facial details in the scene prompt. If a generated image drifts, correct it by referring back to the approved reference sheet and immutable anchors rather than adding contradictory prose.

## Prompt skeleton

```text
Preserve the identity of {{character_id}} from the supplied approved reference image.
Do not redesign facial geometry, hairstyle silhouette, age, body proportions, or signature clothing.

Apply {{style_id}}.

Scene: {{scene}}
Action: {{action}}
Expression: {{expression}}
Camera: {{camera}}
Lighting: {{lighting}}

Maintain exact continuity with the character reference.
{{negative_constraints}}
```
