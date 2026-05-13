## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-22 - [Focus Visibility and Semantic Buttons]
**Learning:** Hidden-by-default interactive elements (like slider arrows) must be forced visible on focus (`focus:opacity-100`) to be accessible to keyboard users. Additionally, all non-submit interactive elements should explicitly define `type="button"` to avoid unintended form behaviors.
**Action:** Always audit `opacity-0` elements for focus states and ensure every `<button>` has a `type` attribute.
