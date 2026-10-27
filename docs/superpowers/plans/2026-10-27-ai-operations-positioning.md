# AI Operations Positioning Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Update the homepage messaging from sales-only consulting to AI Operations for B2B business processes, keeping sales as a specialization.

**Architecture:** Keep existing static HTML/CSS/JS, no framework, no new form endpoints. Add an AI Operations section before existing product tariffs; use existing `#brief` lead form and approved pricing. Preserve roadmap, KATANA and all existing pages.

**Tech Stack:** HTML, CSS, GitHub PR, Netlify (actual production source requires validation).

**Spec:** Approved positioning in YAKUZA HQ Notion: https://app.notion.com/p/406fe0ef271181338141dbd9b2a36695

## Global Constraints
- Do not change payment/checkout/form JS, legal content or current product prices.
- Do not represent proposed AI Operations packages as already delivered or fixed-price.
- No external scripts, trackers or frameworks.
- Existing brand: charcoal, red, bone; responsive and keyboard accessible.
- Do not claim live publish until the Netlify production source is checked.

## Review Focus
- Mobile header with one extra nav link must not overflow.
- On-page CTA to `#brief` must exist and its form must remain functional.
- HTML/CSS must keep existing tags/forms untouched.
- Version cache for CSS updated because CSS uses immutable caching.
- Existing OG image remains an asset from old sales branding, so flag visual metadata update as a follow-up.

## Tasks

### Task 1: Update core positioning
**Files:** Modify `index.html`.

- [ ] Verify original homepage uses Sales Audit hero, lacks `#ai-operations` section.
- [ ] Update hero, navigation and descriptive metadata with outcome-focused AI Operations.
- [ ] Add three honest service stages before Sales products and link CTA to existing `#brief`.
- [ ] Check the existing prices, forms, sales blocks and links remain unchanged.

### Task 2: Responsive visual system
**Files:** Modify `site.css`; change cache query in `index.html`.

- [ ] Assert original CSS has no `.aiops-grid` rules.
- [ ] Add accessible responsive 3-to-1 card grid with primary CTA.
- [ ] Check CSS brace balance and mobile breakpoint definitions.
- [ ] Version CSS query string because Netlify immutable cache would otherwise serve stale style.

### Task 3: Release QA and handoff
**Files:** No additional production files.

- [ ] Verify semantic HTML balance, single H1, duplicate IDs, internal anchor targets, existing CTA and tariff preservation.
- [ ] Create PR with exact changed file list and explicit production deployment caveat.
- [ ] Check deployment source; do not claim publication unless verified through actual live domain.
