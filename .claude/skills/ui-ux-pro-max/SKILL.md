# UI/UX Pro Max - Design Intelligence

This comprehensive design system provides guidance across 10 technology stacks with 50+ styles, 161 color palettes, 57 font pairings, and 99 UX guidelines prioritized by impact.

## When to Use This Skill

Apply this skill when tasks involve **UI structure, visual design, interaction patterns, or user experience quality**. Must-use scenarios include designing new pages, creating components, selecting color/typography systems, reviewing UI code for accessibility, and implementing navigation or animations.

Skip this skill for pure backend logic, API design, performance optimization unrelated to interfaces, infrastructure work, or non-visual automation.

## Critical Priority Rules (1-3)

**Accessibility** (Priority 1): Maintain 4.5:1 color contrast for body text, ensure keyboard navigation, provide alt text, use aria-labels for icon buttons, and respect reduced-motion preferences.

**Touch & Interaction** (Priority 2): Keep touch targets minimum 44×44pt with 8px+ spacing between them. Avoid hover-only interactions; provide loading feedback and clear error messages near problem fields.

**Performance** (Priority 3): Use WebP/AVIF images with lazy loading, declare image dimensions to prevent layout shift (CLS < 0.1), preload critical fonts, and virtualize lists with 50+ items.

## High-Priority Rules (4-5, 9)

**Style Selection**: Match visual style to product type using consistent SVG icons—not emojis. Define elevation/shadow scales and ensure state clarity across hover/pressed/disabled conditions.

**Layout & Responsive**: Design mobile-first with systematic breakpoints (375/768/1024/1440px). Prevent horizontal scroll, respect safe areas, and use viewport meta tags without disabling zoom.

**Navigation**: Bottom navigation should have maximum 5 items with both icon and text labels. Provide predictable back behavior, deep linking for all key screens, and clear active state indication.

## Medium-Priority Rules (6-8, 10)

**Typography & Color**: Use 16px base body text with 1.5-1.75 line-height and 65-75 character line length. Define semantic color tokens (not raw hex), ensure separate dark-mode testing, and support platform text scaling.

**Animation**: Keep micro-interactions 150-300ms with easing that expresses cause-effect relationships. Use transform/opacity only—avoid animating width/height. Respect reduced-motion and ensure animations are interruptible.

**Forms & Feedback**: Use visible labels (not placeholder-only), show errors below fields with recovery instructions, validate on blur, and provide inline success confirmation. Support auto-fill with semantic input types and allow undo for destructive actions.

**Charts & Data**: Match chart types to data (trend→line, comparison→bar). Use accessible color palettes with pattern/texture supplements, always show legends, and provide table alternatives for screen readers.

## Implementation Workflow

**Step 1**: Analyze product type, audience, style keywords, and target stack.

**Step 2**: Generate design system using `--design-system` flag with multi-dimensional keywords (e.g., "entertainment social vibrant content-dense"). Optionally persist with `--persist` for hierarchical retrieval across sessions.

**Step 3**: Supplement with domain searches (`--domain color`, `--domain ux`, etc.) for detailed guidance on specific dimensions.

**Step 4**: Reference stack-specific guidelines using `--stack react-native` for implementation best practices.

## Pre-Delivery Quality Checklist

- No emoji icons; use vector SVG instead
- All tappable elements ≥44×44pt with visible press feedback
- Primary text contrast ≥4.5:1 in both light and dark mode
- Safe areas respected for headers, tab bars, fixed elements
- Micro-interactions 150-300ms with platform-native easing
- Reduced-motion and dynamic text scaling supported
- Focus order matches visual order with descriptive labels
- No horizontal scroll on mobile; readable line length on large screens

This skill emphasizes accessibility, touch-friendly interaction, and platform-native idioms as non-negotiable foundations for professional, usable interfaces.
