## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-27 - [Interactive Hit Areas and Focus Visibility]
**Learning:** For small interactive elements like gallery dots, using `bg-clip-content` with significant padding allows increasing the hit area (e.g., to 32px) while keeping the visual indicator small (e.g., 6px). Also, elements hidden by default (like navigation arrows with `opacity-0`) must explicitly use `focus-visible:opacity-100` to be accessible to keyboard users.
**Action:** Implement increased hit areas for all small touch targets and ensure all interactive states are reflected in `focus-visible` styles.
