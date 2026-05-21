## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2026-05-21 - [Interactive Hit Areas and Focus States]
**Learning:** Small interactive elements like pagination dots need a larger hit area than their visual size for better accessibility (especially on mobile). Additionally, buttons hidden with `opacity-0` until hover must use `focus:opacity-100` to remain accessible to keyboard users.
**Action:** Use `bg-clip-content` with padding to increase hit areas without changing visual size. Ensure all buttons have `type="button"` and proper focus visibility.
