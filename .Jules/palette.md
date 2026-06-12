## 2025-05-15 - [Accessibility Baseline in Landing Pages]
**Learning:** Landing pages built with component-based frameworks (like Astro) often miss basic a11y features like "Skip to Content" links and proper ARIA states for interactive elements (ToC, tab-like galleries) because the focus is usually on visual polish.
**Action:** Always check for a skip link in the root layout and ensure JavaScript-driven state changes (like active video cards) are mirrored in ARIA attributes (`aria-current`).

## 2025-05-22 - [Interactive Micro-UX: Hit Areas and Scroll Synchronization]
**Learning:** Small interactive elements like gallery dots (often < 8px) are difficult to target on touch and high-DPI screens. Additionally, programmatic smooth scrolling (e.g., `scrollTo`) can conflict with `scroll` event listeners that update state based on position, leading to jitter or "ping-pong" state updates.
**Action:** Use a 32px-44px invisible button container for small dots to increase hit area without changing visual weight. Implement a transient `isScrolling` flag during programmatic transitions to temporarily disable position-based state listeners.
