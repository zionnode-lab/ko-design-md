# Samsung One UI — design.md Outline (confirmed)

> Confirmed structural plan for `services/samsung-one-ui.md`. Built from
> [`research/repo-analysis.md`](./repo-analysis.md), [`research/one-ui-sources.md`](./one-ui-sources.md),
> [`research/one-ui-claims.md`](./one-ui-claims.md), and the strongest existing repository entries
> (vapor-ui, seed-design, krds, socar). **Not the final document.**
>
> Optimizes for: (1) usefulness to LLM UI generation, (2) public-source verifiability,
> (3) maintainability across One UI versions, (4) repository consistency, (5) clear
> separation of durable principles vs exact specifications.

---

## 0. Cross-cutting version-isolation strategy (governs the whole doc)

Two layers, always kept visually distinct:

- **Evergreen layer (default body prose):** version-independent One UI principles and behavioral rules — mostly `Version-specific: NO` claims. This is the doc's spine.
- **Version-isolated layer (labelled blocks):** numeric specs (hex/dp) that trace mostly to the **Oct-2019 One UI Design Guidelines PDF (One UI 2 era)**. These are quarantined so they never read as universal One UI rules. Mechanism:
  - A provenance blockquote at the head of the relevant section (repo audit-note form):
    `> **발행값 출처 · One UI 2 세대(2019).** 아래 수치 토큰은 2019 공개 가이드라인 기준이며 One UI 7과 다를 수 있다. [src:N]`
  - A per-token trailing comment stamp (`# One UI 2 (2019)`) so the caveat reaches `tokens.json` `note` and the site Tokens tab.
  - One UI 7-only visual language (circle motif, colored glass, gradients) is labelled `One UI 7` and typed OBSERVED, never a token.

This satisfies goals 3 and 5 and the sourcing rules (no invented specs; durable-first; version-specific material isolated).

---

## 1. Frontmatter plan

```yaml
name: 삼성 One UI
design_system_name: One UI
slug: samsung-one-ui
category: developer          # confirm vs etc in the PR
last_updated: <build date>
created_at: <build date>     # same as last_updated (new entry)
sources: [official URLs only]   # == ## References, in order; [src:N] integer index
related_services: []
lang: ko                     # + services/samsung-one-ui.en.md (lang: both)
logo:                        # unset until Samsung trademark/logo review — Stage 13 TODO
```

`sources` / `## References` set (~10, official only): `developer.samsung.com/one-ui` index · layout/basic · layout/grid · structure/visual-depth · color/system · color/theme · motion/basic · accessibility/color-contrast · comp/* · largescreen-and-foldable/* ; `design.samsung.com` one-ui · one-ui-7 · samsungone ; the 2019 PDF. Each reference description notes source nature + version (e.g. "2019 PDF — primary numeric source, One UI 2 generation"; "one-ui-7 page — some imagery AI-generated, visuals are OBSERVED").

---

## 2. Section order (CI-compliant — Stitch 10 standard, exact spelling/order, + allowed non-standard sections between)

```
# 삼성 One UI — design.md
> lead: identity + "not an official Samsung release" notice + version-isolation note

## Brand & Style              [standard·required]  philosophy + core principles + viewing/interaction/reachability principle
## Colors                     [standard·required]  provenance blockquote + role colors (OKLCH + 2019 stamp) + dark-mode rules
## Typography                 [standard·required]  Roboto(system) ≠ SamsungOne(brand); scale = gap line
## Spacing                    [standard·required]  ≥24dp margins + Reject/Grip zones
## Rounded                    [standard·required]  circle-motif principle + thumbnail 26/20/12dp · button 18dp (isolated)
## Elevation & Depth          [standard·required]  blur/dim/shadow hierarchy rules + One UI 7 colored glass (7-labelled)
## Shapes                     [standard·required]  circle/curved visual language + icon (square bg · white symbol · stroke terminals)
## Components                 [standard·required]  ### decomposition incl. navigation (see below)
── non-standard optional sections (between Components and Do's) ──
## Motion                     [optional]  100–500ms, interpolator [0.22,0.25,0,1], cross-fade rules
## Sound & Haptics            [optional]  sine waveform, special-key differentiation, audio↔visual sync
## Writing                    [optional]  purposeful text, popup limits, inclusive language, one-question rule
## Accessibility              [optional]  4C, 4.5:1 / 3:1, 200% resize, 5s auto-play, NO official touch-target dp
## Do's and Don'ts            [standard·required]  4 required Don'ts (below)
## Responsive Behavior        [optional]  subheads: Window classes / Large screens / Foldables / Multi-window
## Applied Guidance for LLMs  [optional]  durable-principle summary + "stamp the version when using numbers" checklist
## Known Gaps                 [optional]  principle-set divergence, version drift, font, touch-target, OBSERVED items
## References                 [standard·required]  mirrors sources, per-source nature/version notes
```

### Section content map (which OUI claims feed each, density, isolation)

| Section | Approach | Density | OUI claims | Version isolation |
|---|---|---|---|---|
| Brand & Style | principle | principle | 001–023, 025 | watch set (023) flagged; One UI 7 circle motif (004–005) labelled "7" |
| Colors | spec (isolated) | spec | 077–084 | **primary isolation point** — every hex stamped One UI 2; dark-mode rules 085–088 |
| Typography | principle + gap | principle | 089–091, 013 | font is version-bound; no scale — honest gap line |
| Spacing | principle + few specs | mixed | 038–041, 046 | 24dp stamped (safe) |
| Rounded | spec (isolated) | spec | 042, 110, 022 | 2019 values stamped |
| Elevation & Depth | principle | principle | 025–028 | minimal (no numbers); One UI 7 colored glass (029) 7-labelled |
| Shapes | principle | principle | 004, 022, 092–096 | One UI 7 icon visuals (096) OBSERVED |
| Components | spec (evergreen behavior) | spec | 097–119 | mostly version-agnostic; only 18dp (110) isolated |
| Motion | principle + specs | mixed | 121–128 | 124–126 numeric, durable |
| Sound & Haptics | principle | principle | 129–134 | — |
| Writing | principle | principle | 135–141 | — |
| Accessibility | principle + specs | mixed | 142–157 | 145 is 2019-PDF table (stamped); 147 notes NO touch-target dp |
| Do's and Don'ts | guidance | guidance | across | — |
| Responsive Behavior | spec (evergreen) | spec | 043–076 | dp thresholds treated evergreen (live in current docs); foldable 50:50 (060) noted foldable-only |
| Applied Guidance for LLMs | synthesis | guidance | across | reiterates the version-stamp rule |
| Known Gaps | honest list | list | — | overall drift ledger |

### Components — `###` decomposition (goal 1: maximal LLM usefulness)
`app-bar` · `app-bar-extended` · `bottom-bar` · `bottom-navigation` · `button-flat` · `button-contained` · `dialog-choice` (bottom placement) · `dialog-info` (center placement) · `list-item` · `search` · `toast`. Each carries `{group.name}` token references + explicit rules (≤3 app-bar buttons, ≤5 bottom-bar, <4 bottom-nav, 31-char list text, ≤3-line toast, single button style per screen, etc.). These behavioral rules are `Version-specific: UNKNOWN` but function as durable conventions.

### Do's and Don'ts — 4 required Don'ts
1. **Domain-boundary Don't** — don't transplant Samsung's OS/device product concepts (foldable-hardware context, etc.) into an unrelated product.
2. **Vendor-neutrality Don't** — `design_system_name: One UI` → don't surface "One UI" / Samsung class prefixes in the consumer's generated UI copy/classes.
3. **Rule-9 Don't** — don't treat Material Design rules as One UI rules (OUI-084 is the seed of this confusion; block it explicitly).
4. **Rule-11 Don't** — don't present this entry as an official Samsung release.

### Known Gaps — honest list
- Three divergent official principle sets (no single canonical list).
- Most hex/dp values are One UI 2 (2019); One UI 7 values unpublished.
- No official typography scale; system font Roboto ≠ brand typeface SamsungOne.
- No official touch-target dp size (do not invent 48dp).
- One UI 7 visuals (colored glass, gradients, circular icons) are OBSERVED, not tokens.

---

## 3. Adopted from the GPT-proposed outline (CI-compliant folding)

- Viewing / interaction / reachability handled as explicit conceptual units → inside **Brand & Style**.
- New optional **`## Applied Guidance for LLMs`** section (strengthens goal 1).
- Large screens & Foldables surfaced as subheads inside **Responsive Behavior**.

Not adoptable as top-level H2 (CI enforces the standard headings/order), folded instead: `Layout` → Brand & Style + tokens; `Iconography` → Shapes; `Navigation` → Components `###`; `Dark mode` → Colors + Elevation & Depth; `Overview` → title lead; `Sources` → `## References`. No content dropped, only relocated.

---

## 4. Two decisions to confirm before drafting

1. **Colors token density** — include the 4–6 published One UI 2 role colors (Primary `#0381fe`, Primary dark, Color control activated, White `#fafafa`, Black `#000000`/`#080808`) as OKLCH + version stamp (fills the token cards), or keep Colors principle-only with minimal token cards. *(Recommendation: include them, each stamped "One UI 2 (2019)".)*
2. **Responsive dp thresholds** — treat 600 / 840 / 960 dp as evergreen (they are live in the current developer docs), or version-isolate them too. *(Recommendation: evergreen, since the current official docs serve them.)*
