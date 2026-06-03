Use the Scroller when:

- A container has overflow content along one or both axes
- The user benefits from a persistent or hover-revealed position indicator
- Direct manipulation of scroll position (via drag) is desirable

Do not use the Scroller when:

- The container content is fully visible without scrolling — a visible scrollbar on a non-scrolling surface creates a false affordance
- A progress indicator is needed — use **Progress Bar** for communicating task or load progress
- Content is intentionally paginated rather than continuously scrolled — use **Pagination** instead
