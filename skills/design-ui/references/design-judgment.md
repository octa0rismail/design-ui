# Design judgment pass

Perform this pass privately after choosing a direction and before implementation. Deliberate on the high-leverage system choices, not every CSS value. Expose only the chosen rules and concise rationale.

## Decide by purpose

For each relevant design axis, compare at least two plausible options and ask:

- What user task, content, product character, or emotional quality must this choice serve?
- What does each option communicate, and which option reinforces the visual thesis?
- What is the likely failure mode—generic, childish, severe, cluttered, muddy, fragile, or inaccessible?
- Does the choice create useful hierarchy or merely add decoration?
- Can the decision be expressed as one consistent rule and verified in a render?

If an effect has no defensible job, omit it.

## Geometry and corners

Choose among sharp, subtly rounded, and strongly rounded geometry based on product character, density, content, and interaction—not habit.

- Ask whether rounded corners make the product feel appropriately friendly or merely generic and soft.
- Ask whether sharp corners convey precision and confidence or make the interface feel hostile and unfinished.
- Establish a small radius system. Do not apply the same large radius to every button, panel, input, image, and dialog.
- Use exceptions only when they communicate a distinct object or interaction.

## Surfaces, outlines, and elevation

Choose a dominant surface model: flat, outlined, elevated, layered, or a deliberate hybrid.

- Use flat composition when type, spacing, color, and alignment can establish hierarchy without containers.
- Use outlines when they clarify grouping, boundaries, data structure, or affordance. Remove them when they fragment the page into boxes or create a cage-like appearance.
- Use shadows when objects genuinely sit above others or need interaction emphasis. Keep the light logic and elevation scale consistent; avoid hazy shadows used only to make cards feel “designed.”
- Avoid combining fill, border, large radius, and shadow on every surface. Let one treatment dominate and another support it.
- Ask whether a card is necessary. If whitespace and alignment already group the content, do not add a card.

## Density, spacing, and layout

Choose compact, comfortable, or spacious density from task frequency, reading length, device context, and audience.

- Ask whether spaciousness creates focus or wastes space and weakens information relationships.
- Ask whether density communicates capability or overwhelms the primary task.
- Choose a composition rule—strict grid, editorial asymmetry, modular rhythm, layered field, or another product-specific structure—and apply it deliberately.

## Typography, imagery, and controls

- Choose type roles for voice, hierarchy, and readability rather than pairing fonts by trend.
- Decide whether imagery, illustration, iconography, data visualization, or type alone best carries the concept.
- Make control styling reflect importance and behavior. Do not turn every action into the same pill or filled button.
- Check whether labels, icons, and decorative marks feel authored for the product or imported from a generic component library.

## Motion and creative risk

- Use motion to explain change, continuity, causality, or spatial relationship; omit it when it is merely ornamental.
- If every decision is the safest familiar option, increase creative risk on one high-leverage axis that supports the product.
- If more than two axes compete for attention, reduce novelty and strengthen the hierarchy.
- Prefer one memorable systemic idea over many unrelated flourishes.

## Judge the rendered whole

After rendering, ask:

- Do the geometry, surfaces, type, spacing, color, and motion feel like one design system?
- Would removing half the borders, cards, shadows, or radii improve clarity?
- Do outlined elements structure the composition or make it visibly busier and uglier?
- Does the selected surface model make important elements obvious without explanation?
- Does the interface need one braver choice, or has it already spent its novelty budget?

When uncertain about a major choice, produce a focused alternative that changes one system variable—such as sharp versus rounded geometry or outlined versus flat surfaces—and compare the rendered results in context. Choose by the whole composition, not by an isolated component.
