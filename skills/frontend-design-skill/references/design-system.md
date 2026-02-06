# Design System Reference

## Design Token Conventions

### Colors

Define colors using a semantic naming scheme:

```
Primary:    --color-primary-{50..950}
Secondary:  --color-secondary-{50..950}
Neutral:    --color-neutral-{50..950}
Success:    --color-success-{base|light|dark}
Warning:    --color-warning-{base|light|dark}
Error:      --color-error-{base|light|dark}
Info:       --color-info-{base|light|dark}
```

When analyzing an existing codebase, extract the actual token names and values from theme files, Tailwind config, or CSS variables rather than inventing new ones.

### Typography Scale

```
text-xs:    12px / 0.75rem
text-sm:    14px / 0.875rem
text-base:  16px / 1rem
text-lg:    18px / 1.125rem
text-xl:    20px / 1.25rem
text-2xl:   24px / 1.5rem
text-3xl:   30px / 1.875rem
text-4xl:   36px / 2.25rem
```

Document font-family, font-weight, line-height, and letter-spacing alongside size.

### Spacing Scale

Use a consistent base unit (typically 4px or 8px):

```
spacing-1:  4px / 0.25rem
spacing-2:  8px / 0.5rem
spacing-3:  12px / 0.75rem
spacing-4:  16px / 1rem
spacing-6:  24px / 1.5rem
spacing-8:  32px / 2rem
spacing-12: 48px / 3rem
spacing-16: 64px / 4rem
```

### Breakpoints

```
sm:   640px   (mobile landscape)
md:   768px   (tablet)
lg:   1024px  (desktop)
xl:   1280px  (wide desktop)
2xl:  1536px  (ultra-wide)
```

Always design mobile-first: start with the smallest viewport and layer on complexity at larger breakpoints.

## Component State Checklist

When specifying a component, consider these states:

- **Default** — resting state
- **Hover** — mouse hover (desktop only)
- **Focus** — keyboard focus with visible focus ring
- **Active/Pressed** — during click or tap
- **Disabled** — non-interactive
- **Loading** — async operation in progress
- **Error** — validation failure or error condition
- **Empty** — no data or content
- **Selected** — toggled or selected state
- **Skeleton** — loading placeholder before data arrives

Not all states apply to every component. Include only the relevant ones.

## Accessibility Baseline

Every spec should address:

1. **Color contrast** — minimum 4.5:1 for normal text, 3:1 for large text (WCAG AA)
2. **Keyboard navigation** — all interactive elements reachable via Tab, activatable via Enter/Space
3. **ARIA attributes** — roles, labels, descriptions, live regions where needed
4. **Focus management** — visible focus indicators, logical focus order, focus trapping in modals
5. **Motion** — respect `prefers-reduced-motion` for animations
6. **Screen readers** — meaningful alt text, semantic headings, landmark regions
