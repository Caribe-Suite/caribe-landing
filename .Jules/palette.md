## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-20 - [Touch Targets & Keyboard Visibility]
**Learning:** Small interactive elements like pagination dots often have poor hit areas on mobile. Elements that are visually hidden until hover (opacity-0) are unreachable/invisible for keyboard users unless they also have visibility triggers on focus.
**Action:** Use `p-2` with `bg-clip-content` to increase hit areas without altering visual size. Ensure hidden elements use `focus:opacity-100` and `focus-visible` rings for accessibility.
