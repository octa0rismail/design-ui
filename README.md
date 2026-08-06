# design-ui

[![skills.sh](https://skills.sh/b/octa0rismail/design-ui)](https://skills.sh/octa0rismail/design-ui)

An end-to-end agent skill for defining, implementing, rendering, and refining distinctive product interfaces.

It combines creative-direction exploration and design-system definition with an evidence-based frontend iteration loop. The skill starts at the right phase for the request: greenfield direction, design-system work, implementation, or rendered UI review.

## Install

```bash
npx skills add octa0rismail/design-ui --skill design-ui
```

## Use

Invoke `$design-ui` with a product brief, an optional art-direction cue, an existing `DESIGN_SYSTEM.md`, or a UI implementation/review request.

Examples:

```text
Use $design-ui to design and build a responsive marketplace for independent furniture makers.
```

```text
Use $design-ui with direction: playful retro to define the system, then implement the inventory page in React.
```

```text
Use $design-ui to render and refine the current dashboard at desktop and mobile sizes.
```

## What it enforces

- Product-specific creative direction before styling
- A binding, accessible `DESIGN_SYSTEM.md` when the system is unresolved
- Intentional hierarchy, geometry, surfaces, typography, imagery, and motion
- Responsive and state-complete implementation
- At least one render → review → revise → render cycle
- Evidence-backed handoff with inspected routes, viewports, and states

## Repository layout

The installable skill is at [`skills/design-ui`](skills/design-ui).

## License

[MIT](LICENSE)
