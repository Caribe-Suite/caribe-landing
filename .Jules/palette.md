## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-16 - [Slider Accessibility & Touch Targets]
**Learning:** Carousel/Slider indicators (dots) are often too small for touch devices (e.g., 6px). Using `bg-clip-content` with larger padding (e.g., `p-[13px]`) allows for a 32px interactive hit area while maintaining the small visual size. Additionally, elements hidden with `opacity-0` on hover must also have `focus:opacity-100` to be accessible via keyboard.
**Action:** Apply the `bg-clip-content` + padding pattern for small dots and ensure `focus` visibility for hover-triggered UI elements.
