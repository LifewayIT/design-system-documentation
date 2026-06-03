## WCAG Compliance Target

The Scroller targets **WCAG 2.1 AA** compliance.

---

## Accessibility Compliance

### Design

- Thumb fill (==scroller-thumb== → ==border-neutral-subtle==) must meet 3:1 contrast against the Track background (==scroller-track== → transparent) and the underlying container surface in both light and dark modes (1.4.11)
- The Scroller does not rely on color alone to communicate scroll position — Thumb size relative to Track length conveys proportion of visible content independently of color (1.4.1)
- The Scroller does not carry interactive focus states at the component level — keyboard and focus behavior is delegated to the browser or implementation layer (2.1.1)
- The Scroller does not contain text; no text contrast requirements apply (1.4.3)

### Code

Awaiting documentation from development

---

## WCAG Guidelines

- **[Non-text Contrast (1.4.11)](https://www.w3.org/WAI/WCAG21/Understanding/non-text-contrast.html)** — The Thumb must maintain at least 3:1 contrast against the surface it sits on. Use ==scroller-thumb== (→ ==border-neutral-subtle==) as specified; do not substitute a lighter fill that reduces this ratio below threshold.
- **[Use of Color (1.4.1)](https://www.w3.org/WAI/WCAG21/Understanding/use-of-color.html)** — Scroll position is communicated by Thumb size and position within the Track, not by color change alone. No color-only states are introduced.
- **[Keyboard (2.1.1)](https://www.w3.org/WAI/WCAG21/Understanding/keyboard.html)** — Keyboard scroll behavior must be supported at the container level by the implementation. The Scroller component itself does not manage focus or key events.

---

## Standards Referenced

- WCAG 2.1 — Level AA
- APCA (informational, not required at AA)
