## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-16 - [Mailto UX and Redundant Alt Text]
**Learning:** Using `target="_blank"` on `mailto:` links is a poor UX pattern as it creates unnecessary blank tabs. Also, logo alt text should be empty when it's immediately followed by the brand name in text to avoid redundant screen reader announcements.
**Action:** Always avoid `target="_blank"` for mailto links and audit logo alt text for redundancy with adjacent text.
