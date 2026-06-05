## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-16 - [Invisible Focusable Elements and Hit Areas]
**Learning:** Elements hidden with `opacity-0` but still in the DOM (like gallery arrows) are focusable by keyboard users but remain invisible, creating a broken navigation experience. Additionally, tiny interactive elements (like 6px dots) fail WCAG touch target guidelines.
**Action:** Use `focus-visible:opacity-100` on hidden-by-default controls and use larger transparent wrappers (buttons) around small visual indicators to create adequate hit areas (min 24px-44px) without cluttering the UI.
