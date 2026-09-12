# Design system specification

Use this reference after the creative direction is selected. Create `DESIGN_SYSTEM.md` as an actionable source of truth another designer or engineer can implement without guessing.

## Contents

1. Product and design principles
2. Required document structure
3. Quality gates

## Product and design principles

- Solve the product problem before choosing decoration.
- Preserve one coherent visual thesis.
- Tie consequential choices to users, tasks, business intent, content, brand, platform, or accessibility.
- Prefer semantic tokens and reusable rules over arbitrary component-local values.
- Account for accessibility, responsiveness, localization, loading, empty, error, permission, offline, and destructive states from the beginning.
- Do not fabricate company claims, inventory, prices, testimonials, awards, ratings, or performance metrics.
- Avoid unjustified generic defaults: purple-blue glow gradients, glass panels, floating blobs, oversized centered slogans, uniform card grids, pill-heavy controls, excessive shadows, generic line icons, and vague marketing copy.
- Do not turn every section into a rounded card. Use spacing, alignment, dividers, typography, or a flat composition when containers add no meaning.
- Use any normally discouraged technique when product or brand evidence justifies it, and record the rationale.

## Required document structure

Adapt subsections to the product. When a required item is irrelevant, mark it `Not applicable` and explain why.

### 1. Document control

- Product and design-system name
- Version, status, and date
- Owners or roles when known
- Supported platforms
- Source-of-truth statement
- Change and review notes

### 2. Product context

- Brief summary and problem
- Primary and secondary users
- Core jobs and critical tasks
- Business goals and experience principles
- Constraints, risks, and out-of-scope items
- Confirmed requirements and explicit assumptions

### 3. Experience and brand direction

- One-sentence visual thesis
- Three to five brand attributes translated into observable UI behavior
- Emotional goal and trust posture
- Domain conventions retained and intentionally challenged
- Reference qualities without copying a named product
- When external research informed the direction, include the [reference evidence summary](reference-research.md#record-and-synthesize): source links, adopted principles, adaptations, and unverified flow/state gaps
- Anti-goals describing what the product must not feel like
- Selected direction name, spirit, rationale, and approved changes

Translate adjectives into behavior. For example, express `premium` through restrained color, editorial spacing, intentional imagery, and quiet motion rather than leaving it as a mood word.

### 4. Information architecture and page model

- Primary navigation and content hierarchy
- Key entities and relationships
- Required page or screen types
- Reusable page templates
- Primary flows, global actions, and utilities
- Mobile navigation behavior

Define structure, not finished screen layouts.

### 5. Design tokens

Define primitive and semantic tokens with names, values, usage, and accessibility notes.

- Selected palette, thesis, provenance, user changes, verified contrast ratios, and accessibility repairs
- Brand, neutral, surface, text, border, interactive, focus, and status colors
- Typography families, fallbacks, weights, sizes, line heights, letter spacing, and roles
- Spacing and sizing scales
- Grid, containers, columns, gutters, and breakpoints
- Borders, dividers, radii, and stroke widths
- Shadows and elevation
- Opacity, icon sizes, and stroke rules
- Motion durations and easing
- Layer or z-index scale
- Minimum pointer and touch targets
- Light, dark, high-contrast, or branded themes when applicable
- Data-visualization palettes when applicable

Prefer semantic names such as `color.text.primary` over component-specific names unless a component token is necessary.

### 6. Typography and content hierarchy

- Type rationale and fallback stack
- Display, heading, body, label, caption, numeric, and code styles as relevant
- Heading order and responsive scaling
- Line-length, wrapping, and truncation rules
- Numeric alignment and tabular figures when relevant
- Localization and text-expansion behavior

### 7. Layout and responsive behavior

- Container widths, grid behavior, spacing rhythm, and density
- Desktop, tablet, and mobile transformations
- Fixed, fluid, and intrinsic sizing
- Shell, sidebar, panel, and drawer behavior
- Safe areas, reflow, and content priority
- Touch, pointer, and keyboard considerations

Describe how layouts transform, not only breakpoint values.

### 8. Visual language

- Logo placement and clear space when assets exist
- Iconography source and style rules
- Illustration direction
- Photography subject, crop, lighting, and treatment
- Shapes, textures, patterns, and materiality
- Empty-state visuals and data-visualization style
- Asset licensing and provenance expectations

Mark missing brand assets as needed inputs rather than pretending they exist.

### 9. Component system

Cover only relevant components:

- Actions: buttons, icon buttons, links, split buttons, floating actions
- Inputs: fields, text areas, selects, comboboxes, autocomplete, checks, radios, switches, sliders, pickers, uploads, search
- Navigation: headers, sidebars, tabs, breadcrumbs, pagination, steppers, bottom navigation, drawers
- Data display: cards, lists, tables, grids, descriptions, stats, avatars, badges, tags, media, charts
- Feedback: validation, alerts, banners, toasts, progress, loaders, skeletons, empty/error/offline/success states
- Overlays: tooltips, popovers, menus, dialogs, sheets, lightboxes
- Disclosure: accordions and expandable regions
- Domain-specific components

For each relevant component specify purpose, anatomy, variants, sizes, content rules, token dependencies, responsive behavior, accessibility semantics, keyboard behavior, and applicable default, hover, focus-visible, active, selected, disabled, read-only, loading, error, and success states. Explain intentional omissions.

### 10. Interaction patterns and flows

- Form construction and validation
- Search, filtering, sorting, and saved views
- Create, edit, save, cancel, delete, undo, and destructive confirmation
- Authentication, recovery, onboarding, and progressive disclosure when relevant
- Permissions and access control
- Loading, refresh, optimistic updates, retry, and offline recovery
- Import, export, upload, and download
- Selection and bulk actions
- Notifications, preferences, help, and support
- Checkout, booking, or other domain-critical flows

### 11. Content design

- Voice, tone, vocabulary, and naming
- Capitalization and punctuation
- Heading, button, link, hint, and label conventions
- Error, empty, loading, success, and confirmation patterns
- Date, time, number, unit, address, currency, and price formats
- Inclusive language, translation, and text expansion
- Realistic illustrative copy clearly labeled as illustrative

### 12. Accessibility

- Target WCAG 2.2 AA unless another standard is specified
- Contrast requirements and recorded ratios
- Keyboard navigation, focus order, and visible focus
- Screen-reader semantics and landmarks
- Form labels, instructions, and validation announcements
- Alternative text and decorative-image behavior
- Reduced motion, zoom, text resizing, and reflow
- Minimum target sizes
- High contrast and forced colors
- Live regions, captions, transcripts, and audio alternatives when relevant
- Manual and automated test expectations

Never rely on color, position, motion, or an icon alone to communicate meaning.

### 13. Motion and feedback

- Motion principles, durations, and easing
- Enter, exit, transition, and loading behavior
- Gesture and drag-and-drop feedback
- Scroll behavior
- Haptic or audio feedback when appropriate
- Reduced-motion equivalents

Use motion to explain change, preserve context, or confirm action.

When the web implementation stack is known, record the motion tool and why it is needed using [the motion-tool guidance](design-judgment.md#choose-motion-tools-proportionately). CSS/native animation is a valid choice; defer library selection when the target platform is unresolved.

### 14. Technical contract

- Token hierarchy and theme architecture
- Component naming and state/event model
- Platform and browser support
- Responsive implementation expectations
- Performance budgets and asset guidance
- Internationalization requirements
- Testing expectations
- Versioning, deprecation, and migration
- Design-to-code mapping

Remain framework-neutral in the design-system phase.

### 15. Governance and contribution

- Ownership and decision rights
- Contribution and review workflow
- Criteria for adding components or tokens
- Component maturity stages
- Release cadence and documentation requirements
- Adoption measures, deprecation policy, and support path

### 16. Quality-assurance checklist

Include checkboxes for product relevance, coherent thesis, token consistency, component states, interaction coverage, responsiveness, accessibility, localization, content quality, empty/loading/error/permission states, browser/platform behavior, performance, visual regression, interaction testing, fabricated claims, and unjustified AI-design clichés.

### 17. Open questions and implementation handoff

- Decisions requiring user input
- Missing assets or content
- Risks to validate with users
- Recommended usability tests
- Suggested implementation sequence
- Acceptance criteria for the first implementation

## Quality gates

Revise the document until all applicable gates pass:

- The selected direction is recorded without unexplained drift or conservative normalization.
- Final text, control, and focus pairs have calculated role-appropriate contrast ratios.
- The system is specific to this product and domain, not a template with nouns swapped.
- Major visual choices have product, user, brand, or accessibility rationale.
- Tokens form coherent scales and semantic roles.
- Components cover meaningful states, behavior, content, responsiveness, and accessibility.
- Primary flows include failure and recovery.
- Content guidance is realistic and does not fabricate facts.
- Mobile and keyboard use are first-class.
- Accessibility requirements are testable.
- The visual language avoids unjustified clichés and clutter.
- The document is internally consistent and actionable.
