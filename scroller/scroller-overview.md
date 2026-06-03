## Purpose

The Scroller is a passive UI element that communicates scroll position and enables direct manipulation of a scrollable container. It represents the native scrollbar pattern styled to match the Cornerstone design language.

The Scroller is used wherever a container has overflow content that the user needs to navigate — panels, drawers, modals, sheets, and scrollable data regions. It is always tied to a scrollable container and never used decoratively or in isolation.

---

## Usage

Use the Scroller when:

- A container has overflow content along one or both axes
- The user benefits from a persistent or hover-revealed position indicator
- Direct manipulation of scroll position (via drag) is desirable

Do not use the Scroller when:

- The container content is fully visible without scrolling — a visible scrollbar on a non-scrolling surface creates a false affordance
- A progress indicator is needed — use **Progress Bar** for communicating task or load progress
- Content is intentionally paginated rather than continuously scrolled — use **Pagination** instead

---

## Related Components

- **Progress Bar** — Communicates task or load progress; not a scroll position indicator
- **Pagination** — Use when content is paginated rather than continuously scrolled
- **Slider** — A control for selecting a value along a range; shares similar visual language but serves a distinct interactive purpose
