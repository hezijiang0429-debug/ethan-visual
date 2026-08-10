---
name: ethan-visual
description: Generate original 1:1 editorial raster illustrations for article and concept topics in a restrained black, white, and warm-gold ink style. Use for new text-oriented illustrations that need the recurring Ethan character, logical scene poses, optional golden-shaded cat, safe canvas margins, and sparse contextual accents.
---

# Ethan Visual

Create a new illustration with the built-in image generation tool. This skill is for generation, not image editing, unless the user explicitly asks to edit an existing image.

## Non-negotiable visual rules

- Use a square 1:1 canvas and a mostly pure-white background.
- Keep every mark, color field, prop, limb, tail, and shadow fully inside the canvas. Preserve at least a 12% blank white safety margin on all four sides; never let artwork touch or get cropped by an edge. If a draft violates this, regenerate or scale the composition down rather than cropping it.
- Use clean, slightly loose black hand-drawn outlines, simple flat fills, and restrained analog/print texture. The core palette is black, white, warm golden yellow, pale cream, and occasional muted gray or blue only when the scene needs it.
- Keep the image adult, calm, and lightly humorous: simple and relaxed, not childish. Avoid photorealism, 3D rendering, gradients, glossy effects, neon/multicolor palettes, exaggerated perspective, chibi proportions, heavy detail, logos, watermarks, or decorative borders.
- Do not place readable text in the image by default. Replace labels, calendar copy, UI text, and code with abstract lines, blocks, icons, or scribbles unless the user explicitly requests exact text.

## Recurring protagonist

The human protagonist appears in every image. Use `assets/ethan-human-reference.png` as the identity/style reference. Keep these traits stable: compact solid-black side-swept hair with one curved forelock, simple oval adult face, small open almond-shaped eyes with tiny pupils, plain white crewneck sweatshirt, solid-black straight trousers, and plain white low-top sneakers. Avoid oversized cartoon eyes or childlike proportions.

The pose must make physical and visual sense for the scene. Turn shoulders, head, eyes, hands, and feet toward the relevant object: face the monitor when coding or designing UI; look at a book when reading; face the audience when presenting; orient toward a calendar when organizing a schedule. Do not show a person typing while looking away from the computer.

## Optional cat

The cat is supporting, not mandatory. If the user explicitly includes or excludes it, follow that instruction. Otherwise include it in roughly 70% of single illustrations and omit it in roughly 30%; for a batch, target about a 7:3 include/omit ratio. Scene fit can override the default when a cat would make the composition confusing.

When present, use `assets/ethan-cat-reference.png`: a simplified golden-shaded British Shorthair with a round face, small rounded upright ears, plush compact body, short sturdy legs, and a thick curled tail. Use pale cream-gold muzzle/chest/belly, honey-gold sides, deeper amber crown/back/tail, restrained dark tips, and sparse directional short-fur strokes. Show visible light/dark plush variation without realistic fur rendering, tabby striping, Persian features, or overly cute exaggeration. When the cat is omitted, do not add another animal.

## Composition and accents

Make the human the clear focal point and keep the cat subordinate. Add scene-appropriate small accents totaling about 10–15% of the canvas: for example a coffee cup, sticky note and check mark, pen, cable, small sparkles, scissors, timeline blocks, or a few UI panels. Use only the few accents that clarify the topic; do not introduce another large subject or clutter. Keep all accents inside the 12% safety margin.

Use the provided references as visual anchors, not as content to copy literally:

- Human identity and screen-facing pose: `assets/ethan-human-reference.png`
- Golden-shaded cat and duo proportions: `assets/ethan-cat-reference.png`
- Open-eye treatment: `assets/ethan-open-eye-reference.png`
- Accent density and safe composition example: `assets/ethan-accent-sample.png`

## Generation workflow

1. Translate the user’s topic into one concrete action and one clear focal object.
2. Decide cat presence using the explicit instruction or the 70/30 default.
3. Write a structured image prompt naming the 1:1 canvas, 12% white safety margin, recurring protagonist, logical gaze/pose, palette, line treatment, optional cat, and 10–15% contextual accents.
4. Generate with the built-in image tool and include the relevant local reference images. Do not ask for text unless requested.
5. Inspect the result for identity, open eyes, scene logic, cat rule, palette, accent density, readable-text leakage, and edge clearance. Regenerate if any invariant fails.
6. Return only the image unless the user asks for a description or multiple variants.

## Prompt skeleton

“Create a 1:1 editorial illustration about [TOPIC]. Always include the recurring adult Ethan character from the attached human reference; he is [ACTION] and his head, eyes, shoulders, hands, and body logically face [FOCAL OBJECT]. Use small open almond-shaped eyes, black side-swept hair, white crewneck, black trousers, and white sneakers. [Include/omit] the optional golden-shaded British Shorthair from the cat reference. Use black hand-drawn outlines, white space, warm golden yellow and pale cream flat fills, restrained print texture, and a calm adult tone. Add only a few scene-specific accents totaling 10–15% of the canvas. No readable text, logos, watermark, gradients, photorealism, 3D, or exaggerated/cartoon proportions. Keep every element fully inside the canvas with at least 12% blank white margin on all sides; do not crop.”

## Final check

Before delivery, confirm: square output; human present and recognizable; open eyes; physically logical pose; optional cat decision obeyed; limited palette; 10–15% accents when useful; no unintended text; and at least 12% blank white margin on every side. If any check fails, regenerate rather than explaining the failure.
