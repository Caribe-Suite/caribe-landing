## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-20 - [Keyboard Focus and Hit Targets]
**Learning:** Programmatically calling `.blur()` on a button when it becomes disabled is an accessibility anti-pattern because it resets focus to the document body, causing a loss of context for keyboard users. Additionally, `bg-clip-content` combined with transparent padding is an elegant way to increase interactive hit areas (e.g., to 32px or 44px) without altering the visual design tokens.
**Action:** Avoid `.blur()` on disabled state transitions; let the browser handle focus or move it to a logical next element. Use `bg-clip-content` for small decorative indicators that need large hit areas.
