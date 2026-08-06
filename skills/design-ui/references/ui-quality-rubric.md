# UI quality rubric

Use this rubric during visual review. Apply it as a diagnostic aid, not as a recipe or a ban on modern visual patterns.

## 1. Requirement fidelity

- Confirm every visible requirement, action, state, data point, asset, and content constraint against the ledger.
- Confirm the primary task is understandable and executable without relying on decorative context.
- Flag a missing requirement, wrong interaction, broken state, or unsupported viewport as critical or high.

## 2. Product specificity

Ask whether the composition, copy, visual language, and details could be moved unchanged to an unrelated app. If so, find the weakest generic choice and replace it with a decision grounded in the product, audience, or task.

Common template cues need a reason, not automatic removal:

- warm cream with dark brown and orange or amber, paired with editorial serif typography and rounded cards
- purple, indigo, blue, or magenta glow gradients on dark surfaces
- oversized headline plus a generic gradient or abstract blob
- repeated frosted panels, pills, and shadowed cards with no hierarchy
- arbitrary bright accent colors or ornamental gradients
- stock-like imagery, vague slogans, and implausible metrics
- an uninterrupted sequence of same-shaped content blocks
- decoration that competes with the primary task

Favor a clear editorial hierarchy, real content, intentional density, and one or two distinctive details with a purpose.

Check six axes: palette, typography, composition, surface language, imagery, and motion. If three or more reproduce the same recognizable AI-brand or generated-template formula without product evidence, mark the finding high severity and revise at least two structural axes.

## 3. Composition and hierarchy

- Identify the first, second, and third things a viewer sees.
- Check whether the primary action follows naturally from the reading order.
- Check alignment, grouping, whitespace, edge relationships, scanning paths, and visual balance.
- Flag an unclear first action, competing focal points, accidental gaps, or collapsed grouping as high when it impairs use.

## 4. Typography, color, and content

- Establish a legible type scale with purposeful contrast in size, weight, and spacing.
- Use colors with roles: surface, text, muted text, border, action, feedback, and emphasis.
- Confirm the palette has product-specific provenance rather than a model-default hue choice.
- Verify contrast and avoid using color as the only status signal.
- Replace lorem ipsum, generic marketing promises, and fake precision with credible task-specific content.

## 5. Geometry, surfaces, and effects

- Confirm corner radii reinforce the intended character rather than repeating a framework default.
- Confirm every card or container represents a meaningful group; remove boxes that duplicate spacing and alignment.
- Confirm outlines clarify structure without fragmenting the page into a cage of rectangles.
- Confirm shadows communicate elevation or interaction and use a coherent light and depth model.
- Confirm flat areas feel composed through type, spacing, color, and alignment rather than visually unfinished.

## 6. Responsive and state design

- Check the narrow layout as a composition in its own right.
- Test long labels, dense data, empty content, loading, error, selected, hover, focus, and disabled states where relevant.
- Flag clipped touch targets, horizontal overflow, collapsed hierarchy, or inaccessible focus behavior as high or critical.

## 7. Revision order

Repair in this order unless the brief dictates otherwise:

1. broken requirements, flows, or accessibility
2. information architecture, hierarchy, and primary action
3. product-specific visual direction and content
4. responsive composition and state behavior
5. typography, spacing, contrast, and visual mechanics
6. fine detail and animation

Record evidence from the rendered route, viewport, and state for each material finding. A review pass is complete only after the evidence is rechecked.
