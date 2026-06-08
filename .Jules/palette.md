## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-06-08 - [Interactive Hit Areas and Focus Visibility]
**Learning:** Tiny interactive elements like gallery dots (e.g., 6px) have poor hit areas. Additionally, elements that only appear on hover (like navigation arrows) are invisible to keyboard users unless explicitly handled.
**Action:** Use a 32px (w-8 h-8) invisible container for small dots to increase hit area. Ensure hover-only elements use `focus-visible:opacity-100` and clear focus rings for keyboard accessibility.
