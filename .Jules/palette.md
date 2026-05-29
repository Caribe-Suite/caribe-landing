## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-16 - [Large Hit Areas for Small Elements]
**Learning:** For small interactive elements like gallery dots, using `bg-clip-content` with significant padding allows increasing the hit area (e.g., to 32px) while maintaining a small visual appearance (e.g., 6px). This significantly improves accessibility for touch and pointer users without compromising the minimalist design.
**Action:** Prefer `bg-clip-content` and padding over small `width`/`height` for pagination dots or tiny icon buttons to ensure a minimum 24-32px hit area.
