## Anatomy

The Scroller is composed of two elements.

### Track

The outer bounding container of the scrollbar. The Track has a transparent background (`scroller-track`) by default, allowing the surface beneath it to show through. It defines the padding around the Thumb and establishes the overall scrollbar hit area.

### Thumb

The draggable pill element within the Track. The Thumb communicates current scroll position and the proportion of visible content relative to total scrollable content. It uses a pill radius (`scroller-radius`, 999px) and a fixed neutral fill (`scroller-thumb`). Thumb width scales with the Size property.

---

## Variants

The Scroller component has no variants. All configuration is controlled through the Size property.

---

## Sizes

The Scroller ships in four sizes. Size controls the Thumb width and the Track padding.

| Property | Values | Default |
|---|---|---|
| Size | Extra Small \| Small \| Medium \| Large | Extra Small |

| Size | Thumb Width | Padding X | Padding Y |
|---|---|---|---|
| Extra Small | 2px | 8px | 4px |
| Small | 6px | 8px | 8px |
| Medium | 8px | 8px | 8px |
| Large | 12px | 8px | 8px |

**Size guidance:**
- **Extra Small (2px)** — minimal visual presence; appropriate for dense or compact UI regions where scrollbar footprint should be minimal. Best for desktop pointer contexts.
- **Small (6px)** — standard lightweight scrollbar; suits most panel and sidebar contexts.
- **Medium (8px)** — comfortable default for modal and sheet overflow regions.
- **Large (12px)** — suited for touch-friendly surfaces or prominent scrollable regions where a larger interaction target is appropriate.

---

## Options

The Scroller component has no configurable options. Size is the only property and is documented in the Sizes section above.

---

## States

The Scroller component has no documented interactive states. Hover, pressed, and focus behaviors are delegated to the browser or implementation layer and are not represented as visual states on the component itself.

---

## Token Mapping

Scroller styles use design tokens to maintain consistency across themes and platforms. Implementations should reference component tokens rather than raw foundation values.

### Spacing

Currently, Figma component modes are not supported in our documentation platform. Because of this limitation, the **spacing density modes for this component cannot be displayed.**

| Token | Extra Small | Small / Medium / Large |
|---|---|---|
| ==scroller-xs-padding-x== / ==scroller-padding-x== | 8px | 8px |
| ==scroller-xs-padding-y== / ==scroller-padding-y== | 4px | 8px |

### Color

| Token | Value | Role |
|---|---|---|
| ==scroller-track== | Transparent | Track background fill |
| ==scroller-thumb== | `border-neutral-subtle` | Thumb fill |

### Border

#### Radius

| Token | Value |
|---|---|
| ==scroller-radius== | 999px (pill) |

### Size Core — Thumb Width

| Token | Size | Value |
|---|---|---|
| ==scrollbar-thickness-xs== | Extra Small | 2px |
| ==scrollbar-thickness-sm== | Small | 6px |
| ==scrollbar-thickness-md== | Medium | 8px |
| ==scrollbar-thickness-lg== | Large | 12px |
