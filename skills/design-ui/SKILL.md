---
name: design-ui
description: Define, implement, render, and refine distinctive product UI. Use for creative-direction exploration, DESIGN_SYSTEM.md creation or updates, substantial UI design or implementation changes, and rendered visual reviews across web and native interfaces. Includes Pinterest-led reference research and optional GSAP and Motion guidance for purposeful web animation, preferring CSS/native animation for simpler interactions and avoiding unnecessary dependencies or effects.
license: MIT
---

# Design UI

Take UI work from product brief to verified render. Treat direction, design-system definition, implementation, and visual QA as one lifecycle. Keep private comparison and scoring private; share decisions, artifacts, concise audit findings, and evidence.

## Route the request

1. Inspect the brief, repository instructions, existing `DESIGN_SYSTEM.md`, routes, components, assets, product language, target platforms, and references.
2. Maintain a requirement ledger covering users, primary jobs, business goal, explicit requirements, flows, states, viewports, accessibility, content, constraints, and assumptions.
3. Choose the correct entry point:
   - No firm visual system: begin with creative-direction exploration.
   - Existing approved design system: treat it as binding and proceed to implementation or review. Do not force a new exploration unless redesign is requested or the system is materially incomplete.
   - Design-system-only request: complete direction selection and `DESIGN_SYSTEM.md`, then stop.
   - Implementation request with a selected target and direction: proceed through implementation and rendered iteration.
   - Review-only request: inspect the rendered interface and report findings; do not modify files unless the user requests changes.
4. Resolve low-risk ambiguity with a stated assumption. Ask at most three concise questions only when answers would materially change the product direction.

When external references are needed or requested, read [references/reference-research.md](references/reference-research.md) completely before researching. Use Pinterest as the default visual-discovery source, supplement it with original product evidence for flows and states, and preserve the user's supplied references and approved direction. Do not make new research a prerequisite for a small change or a review with sufficient existing evidence.

## Phase 1: Choose a creative direction

Run this phase before creating or substantially revising `DESIGN_SYSTEM.md` unless the user supplied an approved visual system or explicitly delegated a specific direction.

Treat an art-direction cue such as retro, playful, brutalist, futuristic, organic, editorial, minimal, or luxurious as an umbrella, not a finished concept. Interpret it across the full design grammar. When no cue exists, keep the exploration product-led and broad.

### Curate 10 directions

Create exactly 10 viable directions. Read [references/design-divergence.md](references/design-divergence.md) completely before generating the set. Apply its full-exploration constraints, evidence, palette-provenance, scoring, novelty-budget, and fingerprint rules using the compact presentation format below.

Keep the user-facing exploration compact. For each direction provide only:

- A distinctive name
- A two-to-five-word design spirit
- Six labeled swatches with exact hex values: primary, secondary, accent, background, surface, and text
- A three-to-eight-word visual-language cue combining typography, form, composition, or imagery
- A three-to-eight-word product-fit note

Present one comparison table or 10 compact style tiles. Limit each direction to 24 words excluding names, labels, and hex values. Never communicate through color alone. End with only:

- `Recommended:` direction name plus one short sentence
- `Alternative:` direction name plus one brief condition
- One concise prompt to choose by number/name, request a hybrid, correct constraints, or delegate the choice

Stop for the choice unless the user already delegated it. Do not write or outline `DESIGN_SYSTEM.md` during the selection response.

## Phase 2: Define the system

After selection, read [references/design-system-spec.md](references/design-system-spec.md) completely and create or update `DESIGN_SYSTEM.md` at the project root or requested path.

- Preserve the chosen direction's whole grammar, not only its palette.
- Calculate contrast ratios for final text, control, and focus pairs; repair failures before tokenizing them.
- Distinguish confirmed requirements from assumptions.
- Define semantic tokens, components, interaction behavior, responsive transformations, content rules, accessibility, motion, technical mapping, and governance.
- Use realistic domain-specific examples without inventing claims, inventory, prices, testimonials, awards, or metrics as facts.
- Update the design system when implementation exposes a missing rule. Do not create undocumented exceptions.

If the user has not selected an implementation target, stop after validating the document and ask which stack and page or flow should come first. If the user already requested the full lifecycle and selected or delegated the direction and target, continue.

## Phase 3: Build an intentional first pass

Read [references/design-judgment.md](references/design-judgment.md) completely before coding. State a compact visual thesis: audience, primary job, emotional quality, product-specific idea, palette provenance, geometry/elevation rules, and one memorable detail.

- Establish information architecture, hierarchy, credible content, and the primary action before decoration.
- Implement against `DESIGN_SYSTEM.md`; reuse established components and conventions before introducing new ones.
- Give every radius, card, outline, shadow, elevation, gradient, texture, and motion treatment a job. Omit effects without a defensible purpose.
- For web UI, consider [GSAP](https://gsap.com/) and [Motion](https://motion.dev/) when they materially improve an interaction; follow the motion-tool guidance in `references/design-judgment.md`. Neither is a required dependency.
- Differentiate the chosen direction across at least three structural axes beyond color.
- Build responsive compositions deliberately rather than shrinking desktop.
- Cover relevant loading, empty, error, long-content, selection, hover, focus, disabled, permission, and destructive states.
- Preserve semantic structure, keyboard access, focus visibility, contrast, reduced motion, localization, and clear code responsibilities.
- Prefer product-specific copy, data shapes, and components over placeholders and fabricated precision.

If the task skips direction exploration and lacks firm brand tokens or references, read [references/design-divergence.md](references/design-divergence.md) completely. Follow its focused implementation-alternatives path and record the chosen rationale before implementation.

## Phase 4: Render, review, and revise

Treat the first visual implementation as an unaccepted draft. Run relevant checks and inspect the actual interface.

For review-only requests, perform the inspection and audit steps below, then report findings and recommended revisions. The repair steps and implementation exit gate apply only when changes are requested.

1. Render the primary route and relevant states.
2. Inspect at least one desktop viewport and one narrow mobile viewport for responsive work.
3. Compare against supplied references, `DESIGN_SYSTEM.md`, requirements, and any existing baseline.
4. Treat runtime errors, broken interactions, clipping, overflow, illegible content, missing hierarchy, and accessibility failures as blockers.
5. Read [references/ui-quality-rubric.md](references/ui-quality-rubric.md) completely before the first review.
6. Record a concise observable audit: route, viewport, state, finding, severity, and evidence.
7. Rank findings critical, high, medium, or low. Fix the one to three highest-leverage items first.
8. Rerun checks and rerender affected views. Compare with prior evidence.
9. Complete at least one full render → review → revise → render cycle for every non-trivial visual change. Continue while a critical or high issue remains.

When a high-impact choice remains uncertain, implement or mock the strongest alternative, change one system variable, and compare renders. Revise direction before micro-polish when hierarchy, composition, or product specificity is weak. A token tweak is not an iteration.

## Enforce the exit gate

Finish only when all applicable conditions are true:

- Every explicit requirement is implemented or a real blocker is named.
- The primary flow and relevant visual states work without a known critical failure.
- The rendered result visibly follows the selected direction and `DESIGN_SYSTEM.md`.
- Palette provenance, contrast, geometry, surfaces, hierarchy, and responsive rhythm are coherent.
- The interface passes the default-fingerprint check in the divergence protocol and does not rely on an unjustified generic AI-template cue.
- Desktop and mobile evidence has been inspected when the environment permits.
- Accessibility, responsive behavior, realistic content, and code responsibilities remain intact.

If the work remains stuck after four meaningful revision cycles, attempt a materially different composition or direction when feasible, then report the unresolved constraint instead of claiming completion.

## Hand off with evidence

Summarize the selected direction, palette provenance, key design-judgment rules, highest-impact revisions, checks run, routes/viewports/states inspected, and remaining limitations. Deliver the artifact and concise evidence, not a transcript of reasoning.
