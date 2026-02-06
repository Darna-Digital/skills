---
name: frontend-design-skill
description: Create frontend design specifications for UI components, pages, and layouts with design tokens, responsive breakpoints, and component state documentation. Use when the user wants to design a UI component, create a design spec for a page or feature, define a design system or tokens (colors, typography, spacing), plan responsive layouts, document component states and variants, or translate a design brief into an implementable frontend specification.
---

## Overview

This skill produces structured design specifications that bridge the gap between design intent and frontend implementation. Specs are written as markdown files in this skill's `specs/` folder (locate it next to this SKILL.md).

## Workflow

1. Ask the user for design context:
   - What component, page, or feature needs a design spec?
   - Any existing designs, screenshots, or references?
   - Target framework (React, Next.js, etc.) and styling approach (Tailwind, CSS Modules, styled-components)?
2. Analyze the codebase for existing design patterns:
   - Search for existing components, theme files, CSS variables, Tailwind config, or design tokens
   - Identify the current styling approach and conventions
   - Note existing color palette, typography scale, spacing system, and breakpoints
3. Read `references/design-system.md` for design system guidance and token conventions
4. Determine the spec type:
   **Component spec?** → Document props, variants, states, responsive behavior, and token usage
   **Page/layout spec?** → Document layout grid, section hierarchy, component placement, and responsive breakpoints
   **Design system/tokens?** → Document color palette, typography scale, spacing scale, breakpoints, and shadows
5. Generate the design spec in `specs/` with filename `<feature-or-component-name>.design-spec.md`
6. If the branch includes a task slug, prefix the spec filename with the task number

## Spec Structure

Use this structure, adapting sections as needed:

```markdown
# [Component/Page Name] Design Spec

## Context
[Brief description of purpose and where it appears]

## Design Tokens Used
[Colors, typography, spacing, shadows relevant to this spec]

## Layout
[Grid, flexbox, positioning details with responsive breakpoints]

## Component States
[Default, hover, active, disabled, loading, error, empty states]

## Variants
[Size, color, style variants if applicable]

## Responsive Behavior
[Breakpoint-specific layout changes and adaptations]

## Accessibility
[ARIA roles, keyboard navigation, contrast requirements, focus management]

## Implementation Notes
[Framework-specific guidance, component composition, prop interfaces]
```
