# Build Notes

## Theme foundation

**Decision:** Used CSS custom properties for global design tokens rather than hardcoding values throughout sections.

**AI assistance:** Discussed architecture and received example implementation. I reviewed and hand-typed the final code.

**What I learned:** How Skeleton loads global styles and where theme-wide tokens should live.

---

## Header

**Decision:** Navigation is merchant-configurable rather than hardcoded.

**AI assistance:** Used AI for implementation guidance and code review.

**What I learned:** How link lists, section settings, and responsive navigation work in Shopify.

---

## Global Design System

**Decision:** Extended Skeleton's existing theme settings instead of creating a separate styling system. Global colors, typography, layout values, and border radii are exposed as CSS custom properties.

**AI assistance:** Used AI to help design the token architecture and choose an initial Tressa palette. I hand-typed and reviewed the implementation.

**What I learned:** `settings_schema.json` defines what the merchant can configure, Liquid exposes those values through the `settings` object, `css-variables.liquid` converts them into CSS custom properties, and component CSS consumes those properties.

**Design direction:** Tressa uses hellowisp.com as visual inspiration without copying it directly—warm consumer-healthcare styling, editorial typography, soft backgrounds, strong accent colors, and generous whitespace.

---

## Git Branch Recovery

**Issue:** I accidentally committed the design-system work to `main` instead of the feature branch.

**Resolution:** Stashed an additional uncommitted change, cherry-picked the relevant commits onto `feature/theme-foundation`, restored the stash, then reset local `main` to `origin/main`.

**What I learned:** Unpushed commits can be moved safely between branches with `cherry-pick`, and `stash` can temporarily preserve working-tree changes while switching branches.