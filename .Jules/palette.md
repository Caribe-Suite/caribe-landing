## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-16 - [Micro-UX Accessibility Refinement]
**Learning:** Decorative icons and redundant brand logos are common accessibility noise. Using `aria-hidden="true"` for icons and empty `alt=""` for logos immediately followed by text keeps screen reader announcements focused and efficient.
**Action:** Proactively audit components for icon-only buttons (add `type="button"`) and decorative elements that should be hidden from assistive technology.
