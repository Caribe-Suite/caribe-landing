## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-16 - [Large Hit Targets for Small UI Elements]
**Learning:** Pagination dots in galleries are often too small for comfortable interaction (e.g., 6px). Wrapping them in a larger invisible or semi-transparent button (32px+) significantly improves accessibility and usability without sacrificing the minimalist aesthetic.
**Action:** Use a wrapper button (e.g., `w-8 h-8`) with an inner `span` for the visual dot. Ensure the wrapper handles focus states and the inner `span` handles visual active states.
