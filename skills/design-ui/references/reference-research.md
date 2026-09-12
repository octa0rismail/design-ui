# Pinterest-led reference research

Use this workflow when the task needs external design references. Its output is a small, traceable set of design decisions, not a large collection of attractive screenshots. Keep findings in the existing requirement ledger or working notes; incorporate adopted decisions into `DESIGN_SYSTEM.md` after direction selection.

[Pinterest](https://www.pinterest.com/) is the default visual-discovery source, not proof that a UI ships or that a flow works. Supplement it with original product pages, public demos, official help articles, or user-supplied recordings. No paid library is required. Honor the user's supplied references and choices of other sources.

## Search from the product problem

Start with the audience, primary job, target platform, content density, required states, and brand constraints. Preserve approved tokens; research should resolve a specific gap rather than reopen settled decisions.

Search across the relevant lenses instead of repeating a broad query such as "beautiful app UI":

| Lens | Query shape | Illustrative furniture-marketplace query |
| --- | --- | --- |
| Task and screen | domain + user action + screen + platform | furniture marketplace browse filters mobile UI |
| Components and states | component + state + interaction | product filter drawer no results applied filters |
| Visual language | domain + typography, composition, or material | furniture catalog editorial grid typography |

Use Pinterest's [keyword search and content filters](https://help.pinterest.com/en/article/search-for-ideas-on-pinterest) where available. Boards help discover related work; individual Pins are the evidence records. Use related Pins or [visual search](https://help.pinterest.com/en/article/use-visual-search-features) to expand a promising direction, then deliberately search a contrasting direction so recommendations do not collapse the set into one style. Do not upload private project images for visual search without authorization.

## Inspect and curate

- Open each shortlisted Pin and inspect its image or video at a readable size. A search thumbnail, title, or summary alone is a lead, not an inspected reference.
- Follow the source link when available. Identify the original product or creator and check whether the linked page supports the Pin's attribution. The person who saved a Pin is not necessarily its creator.
- Classify each useful observation as **live product observed**, **documented or recorded behavior**, **concept/mockup**, or **unverified image**. An inaccessible source stays unverified; a polished mockup or AI-generated concept can inspire visual language but cannot establish production behavior.
- Deduplicate reposts and crops of the same design. Favor task fit, readable detail, traceable sources, distinct structure, and applicable platform over popularity or save counts.
- Keep a small shortlist, usually four to eight distinct examples for a substantial brief and fewer for a focused component. Cover contrasting compositions, not just different palettes, and avoid letting one creator or product dominate unless the user asks for that reference.
- Retain a reference only if it answers a named design question. Stop when the key decisions have useful evidence; search again only for a specific remaining gap.

## Recover flow and state context

A single Pinterest image may show a useful composition without explaining the surrounding interaction. Seek screen sequences and behavioral context from accessible original sources without inventing missing screens.

For the primary task, track the entry point, user action, resulting state, and available recovery path. Inspect relevant loading, empty, error, selected, disabled, long-content, and narrow-layout behavior when the source exposes it. Search the actual product's public documentation or demo for missing steps; use permitted read-only interactions, not purchases, submissions, or account changes merely to inspect a flow.

Keep **observed**, **inferred**, and **proposed for our product** separate. A static screenshot does not establish keyboard behavior, accessibility compliance, responsiveness, animation timing, or usability. A recording proves only the sequence shown. If behavior cannot be inspected, record the gap and design/test it locally; do not describe the reconstructed flow as verified source evidence.

## Record and synthesize

For each shortlisted reference, record:

- Pin URL and original source URL when discoverable; product/creator attribution and inspection date
- Target screen, platform, state, and evidence classification; screenshot or recording reference when available and permitted
- The specific visible principle worth adopting, its product fit, and what must change or be rejected
- What remains unobserved, and how it will be validated in our implementation

Keep the user-facing summary compact: **source → observed principle → product-specific adaptation → evidence gap**. Cite direct Pin and original-source links, not only board or search pages. During the compact direction-selection response, attach source links to the relevant direction names; keep detailed notes out of the option cards.

Combine complementary principles into one visual thesis. Use the existing [divergence protocol](design-divergence.md) for direction comparison and default-template checks; do not assemble incompatible pieces from unrelated screens. References inform decisions but do not override the user's brand, accessibility needs, or required flows. Do not treat Pin availability as permission to reuse imagery, fonts, copy, or other assets; use authorized assets in the implementation.

## Handle limited access

Use available browser and search tools; no Pinterest-specific plugin or paid integration is required. If Pinterest requires a session that is unavailable, use public web/image search such as `site:pinterest.com/pin/ furniture marketplace filters UI` to discover accessible Pins and original sources. Do not bypass login gates, access restrictions, or paywalls, and do not claim to have viewed blocked images.

If a direct attempt and a focused fallback do not provide usable evidence, report the access gap and proceed with accessible original sources or the existing brief. Ask for a user-supplied board, Pin, screenshot, or recording only when the missing reference would materially change the result. Creating boards, saving Pins, following accounts, and uploading assets are separate actions; research alone does not authorize them.

## Research acceptance check

- Each adopted reference maps to a real design question and an inspected visual or behavioral observation, with traceable links and honest attribution.
- The shortlist provides meaningful structural range; repeated Pins and a personalized feed are not mistaken for independent evidence.
- Flow/state gaps are explicit and carried into implementation acceptance criteria, not filled with invented observations.
- The chosen principles become coherent, product-specific rules rather than a copy of one product or a collage of styles.
- The rendered implementation is evaluated using the existing [quality rubric](ui-quality-rubric.md), including usability, accessibility, responsive behavior, and realistic states. Inspiration alone does not pass those gates.
