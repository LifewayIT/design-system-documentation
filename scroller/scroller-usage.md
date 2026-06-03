## Placement

The Scroller is always positioned at the edge of its scrollable container — it is never placed in isolation or used as a standalone decorative element.

- **Vertical scroll:** The Scroller appears on the trailing (right) edge of the container, spanning its full height
- **Horizontal scroll:** The Scroller appears on the bottom edge of the container, spanning its full width
- **Both axes:** When a container scrolls on both axes, two Scroller instances are used — one vertical, one horizontal

---

## Hierarchy

The Scroller is a passive UI element — it does not interrupt user tasks or carry elevation above its containing surface. It sits within the bounds of its container and does not overlap other content.

- Do not place the Scroller outside the bounds of its overflow container
- Do not use the Scroller as the primary navigation mechanism for long-form content — ensure page-level navigation patterns remain available

---

## Content Rules

The Scroller carries no text content. There are no copy guidelines for this component.

---

## Responsive Behavior

Scroller size should match the density and touch context of the surrounding UI at the target viewport.

- **Spacing:** Extra Small uses reduced vertical padding (4px) to minimize footprint in compact regions. Small through Large use consistent 8px padding on both axes.
- **Typography:** The Scroller contains no typography.
- **Size:** On mobile viewports, prefer Medium or Large to ensure an adequate touch target for the Thumb. Extra Small and Small are best suited for desktop contexts where pointer precision is available.

---

## Do / Don't

#### Matching Size to Context

Do

Use Extra Small or Small in compact desktop layouts — panels, sidebars, and dense data regions where the scrollbar should have minimal visual weight.

Don't

Don't use Extra Small on mobile or touch surfaces — the 2px Thumb width does not provide an adequate touch target.

#### Container Boundaries

Do

Keep the Scroller within the bounds of its scrollable container so it reinforces the scroll region visually.

Don't

Don't place the Scroller outside its container or overlay it on unrelated UI — it will create false affordances and mislead users about what is scrollable.

#### Correct Use Case

Do

Use the Scroller to allow users to navigate overflow content within a container — modals, panels, drawers, and scrollable regions.

Don't

Don't use the Scroller as a progress or loading indicator — use **Progress Bar** for that purpose.
