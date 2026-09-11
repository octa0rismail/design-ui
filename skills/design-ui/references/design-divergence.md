# Design divergence protocol

Use this protocol when the user has not supplied firm brand tokens, a design system, or a specific visual reference. Seek product fit and authorship, not novelty for its own sake.

## Extract design evidence

Derive visual choices from available signals:

- the user's audience, task, emotional goal, and language
- the product's data, objects, workflows, materials, or physical environment
- existing logos, imagery, assets, architecture, and brand history
- relevant geography, culture, era, editorial context, or technical domain

Do not derive the direction from the model's favorite palette or a fashionable reference that the brief did not mention.

## Explore direction candidates

### Full direction exploration

For a new or substantially revised design system, follow the count and presentation format in [Phase 1](../SKILL.md#phase-1-choose-a-creative-direction). The directions should feel as though independent strong studios answered the same brief.

Build a private contrast map across light/dark, warm/cool, muted/vivid, quiet/energetic, geometric/organic, minimal/expressive, editorial/utilitarian, soft/sharp, spacious/dense, and contemporary/heritage-aware.

- Include meaningful range across posture, temperature, chroma, density, typography, geometry, composition, imagery, materiality, and motion unless brand constraints rule it out.
- Include at least three brave but usable directions.
- Apply the dominant-hue limits in [palette provenance](#establish-palette-provenance).
- For an open brief, do not make orange, amber, copper, or rust the primary identity, and do not make a purple, indigo, blue, or magenta gradient the main identity, unless product or brand evidence specifically supports it.
- Make every pair differ on at least five axes among color architecture, typography, geometry, density, composition, imagery, materiality, iconography, and motion.
- Reject sibling directions and hue-only variations before presenting them.
- Do not default to familiar AI-brand aesthetics, generic SaaS layouts, or conservative luxury merely because they are safe.
- Ground every option in the product, audience, task, content, environment, or supplied brand evidence.

### Focused implementation alternatives

For an implementation-only request that legitimately skips Phase 1 and still lacks firm visual tokens, create three concise candidates before implementation. Give each candidate:

- a concept sentence tied to product evidence
- a palette family and the source of each major color role
- a typographic personality
- a composition rule
- a surface, texture, or image language
- one signature interaction or detail

Make the candidates differ across at least four of those six axes. Do not present one layout in different colors. Keep this exploration concise and choose autonomously unless the user asked to select a direction.

## Suppress default model priors

Treat these combinations as unavailable starting points in an open brief:

- warm cream, dark brown, and orange, amber, copper, or rust; high-contrast editorial serif; rounded cards; restrained line illustrations—the recognizable Anthropic or Claude-adjacent formula
- dark navy or black with purple, indigo, blue, or magenta glow gradients; glass panels; neon accents
- pale gradient blobs, pill-heavy navigation, oversized centered slogan, and a uniform SaaS card or bento grid
- generic blue dashboard, white cards, interchangeable metrics, and a single bright accent

Use one only when the user's brand, assets, subject matter, or explicit reference directly supports it. “Tasteful,” “modern,” “premium,” and “safe” do not count as support. If a justified direction uses one default element, alter the other major axes so the result does not reproduce the whole formula.

## Establish palette provenance

Explore at least three different hue architectures before choosing the palette. For every major color role, state a short source such as a product material, existing asset, environmental cue, data meaning, or cultural reference.

For a 10-direction set, count dominant hue families before presenting it. Do not allow one dominant hue family to lead more than two directions unless supplied brand evidence requires that repetition. A different accent on the same warm-neutral architecture does not count as a different hue architecture.

Build roles for background, surface, text, muted text, border, action, focus, and semantic feedback. Check contrast early. Do not use unusual color merely to appear creative; use an uncommon palette only when it reinforces the thesis and remains legible.

## Choose with a design-fit score

Score each candidate from 0–2 on:

- relevance to audience and primary task
- product and content specificity
- hierarchy and usability
- distinctiveness from recognizable templates
- technical and accessibility feasibility

Choose the strongest total with the clearest product rationale. Do not choose the most familiar candidate merely because it is easiest to execute.

## Spend a controlled novelty budget

Make one or two aspects memorable—composition, type treatment, imagery, material language, or interaction—while keeping the primary flow legible and familiar enough to use. Avoid making every axis unconventional at once.

## Run the fingerprint check

Before implementation and again after rendering, ignore the logo and replace the product copy mentally with generic text. Compare the result across palette, typography, composition, surfaces, imagery, and motion.

If the interface still resembles a recognizable AI-company site or generic generated template on three or more axes without product evidence, treat it as a high-severity issue. Change at least two structural axes before continuing; a minor hue adjustment does not pass. For review-only work, report the finding and recommended structural changes without editing the interface.
