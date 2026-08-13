# samsung-one-ui — Skeptical Reviewer Audit

> Adversarial audit of the contribution (`services/samsung-one-ui.md` + tokens sidecar +
> previews + test edit). Goal: find what a maintainer would reject, not defend the draft.
> Classifications: **VERIFIED** (official Samsung source explicitly states it) ·
> **PARTIAL** (verified core + unverified garnish: coined names, over-broad framing,
> citation covering only part of the sentence) · **INFERRED** (interpretation presented
> without adequate marking) · **UNSOURCED** (no official support).
>
> Audit inputs: line-level reread of the production md, the claim registry
> ([one-ui-claims.md](./one-ui-claims.md)), the numeric audit
> ([numeric-claims.md](./numeric-claims.md)), the repo's validator source
> (`src/lib/draft-validator.ts`), plus two live re-checks performed during this audit
> (`developer.samsung.com/one-ui/one_ui6.html`; official-domain search for "One UI Sans").

---

## 🔴 Findings that could get the PR rejected

### F1 — Audit-note blockquotes are format-invalid and therefore INVISIBLE to the linter (lines 73, 126)

The repo convention pins audit notes to `> **<라벨>(YYYY-MM-DD).**`, and the validator's
recognizer is `AUDIT_NOTE = /^>\s*\*\*[^*]*\(\d{4}-\d{2}-\d{2}\)\s*\.?\s*\*\*/`
(`src/lib/draft-validator.ts:186`) — **the label must end with a parenthesized pure
date**. Both blockquotes in this draft end with `(2026-08-13 대조).**` — the word `대조`
inside the parens breaks the match. Consequence (spelled out in the repo's CLAUDE.md):
the notes are *not counted as audit notes at all*; placement/duplicate checks silently
skip them, and a maintainer reading the conventions doc will classify this as a rule
violation, not a legacy variant ("형태가 어긋난 메모는 잡히는 게 아니라 아예 안 보인다…
규칙 위반이니 고치면 된다").

This is exactly why `validate:catalog` reported zero warns — not because the notes are
fine, but because they were never seen.

**Fix (required):** relabel so the parens hold only the date, e.g.
`> **발행값 대조 — One UI 2 세대 2019-10 발행분(2026-08-13).**` in both `## Colors` and `## Rounded`.

### F2 — Invented rationale attached to a cited rule (line 178) — INFERRED presented as fact

> "스와이프로 탭 간 이동은 지원하지 않는다 [src:15] — **제스처 내비게이션과의 충돌을
> 피하는** One UI 고유 규칙이므로…"

Samsung's bottom-navigation page states the rule but **never states the reason**. "제스처
내비게이션과의 충돌을 피하는" is a fabricated causal explanation sitting inside a cited
sentence — precisely the kind of thing the repo's semantic spot-check ("인용은 존재가
아니라 내용 일치") is designed to catch. Classification: the rule is VERIFIED, the
rationale is **UNSOURCED**.

**Fix (required):** delete the rationale ("One UI 고유 규칙이므로 스와이프 페이저를 붙이지
말 것"만 남기기), or mark it explicitly as 해석.

---

## 🟠 Findings a strict reviewer would probably flag

### F3 — Citation stretched over synthesis (lines 190, 194) — PARTIAL

- Line 190: "선택·확인 다이얼로그는 화면 하단에 나타난다 [src:17] — 손이 닿는 곳에 결정을
  두는 reachability 원칙의 **구체화다 [src:1]**." src:1 states the reachability principle
  in general; it says nothing about dialogs. The linkage ("구체화다") is catalog synthesis
  wearing a citation. Defensible, but a reviewer applying content-match strictly could
  bounce it.
- Line 194: "결정이 필요 없는 정보이므로 **도달성 대신 가시성이 우선이다**" — an unmarked
  interpretive gloss (Samsung states placement, not the visibility-over-reachability
  rationale). UNSOURCED gloss, low stakes but same pattern as F2.

**Fix (recommended):** move the synthesis outside the citation ("…하단에 나타난다
[src:17]. 하단 배치는 뷰잉/인터랙션 원칙과 같은 방향이다(해석)."), delete the 가시성 gloss
or mark 해석.

### F4 — Catalog-coined token names not declared as coined — PARTIAL

`primary-dark-on-dark` and `black-dark` do not exist in any Samsung publication. Samsung
publishes **one role "Primary dark" with two per-theme values** and **one name "Black"
with two per-theme values**; the catalog split them into separate flat tokens because the
sidecar/yaml format needs one value per name. The *values* are VERIFIED; the *names* are
an unmarked modeling act. The prose explains the value-sharing (#3e91ff) but never says
"이 토큰명 두 개는 카탈로그가 부여한 이름이다."

**Fix (recommended):** one sentence under the yaml fence declaring the naming act, e.g.
"토큰명 `primary-dark-on-dark`·`black-dark`는 테마별 값을 1토큰 1값으로 펴기 위해
카탈로그가 부여한 이름이다 — 발행 role명은 'Primary dark'와 'Black'이다."

### F5 — Global absence claims cited to single pages — PARTIAL (overreach in phrasing)

Absence can only be claimed for the surveyed corpus, not the world:

- Line 73: "One UI 7의 시스템 팔레트 수치는 **공개되지 않았으므로** [src:38]" — src:38
  shows *that page* publishes no figures; it cannot prove Samsung published none anywhere.
- Similar assertive-absence phrasings: "코너 radius 수치는 발행되지 않았다" (Shapes),
  "존의 크기 수치는 발행되지 않았다" (Spacing), "표시 시간 수치는 발행되지 않았다" (toast).
- Counter-example done right, already in the draft: "이후 세대의 시스템 폰트 **교체 여부는
  공개 문서에서 확인되지 않는다**" — survey-scoped phrasing (the socar precedent:
  "공개 조사 범위에서 surfaced되지 않았다").

**Fix (recommended):** normalize assertive-absence phrasings to survey-scoped ones
("공개 조사 범위에서 확인되지 않았다"). Low effort, removes an entire attack surface.

### F6 — Version stamp stronger than its source (Colors yaml) — PARTIAL

`primary`/`primary-dark`/`color-control-activated` carry the stamp "One UI 2(2019)
발행값", but their cited source (`color/system.html`) is **undated**; only the
corroborating PDF is 2019. Stamping the developer-page values as 2019-era asserts
provenance the page itself doesn't state. Conservative direction (it under-claims
currency), but a reviewer can point out the stamp exceeds the evidence.

**Fix (optional):** stamp as "2019 가이드라인과 일치 · 페이지 자체는 무버전" for the three
developer-page tokens, keep "One UI 2(2019)" only for the PDF-only values (white/black/black-dark).

### F7 — Relative valuation in body prose (line 162) — style-rule adjacent

"컴포넌트 규칙은 One UI 발행물에서 **가장 durable한** 부분이다" — the repo bans
relative/superlative claims in audit notes because they rot silently; this is body prose,
not an audit note, but the same reviewer instinct applies ("그 자리에서 참거짓을 확인할 수
있는 측정값으로"). Also "durable"/"evergreen" register: English jargon in ko prose.

**Fix (optional):** "아래 규칙 대부분은 세대 표기 없이 developer 포털 현행 문서로
서빙된다" alone carries the point without the superlative.

---

## 🟡 Minor observations (unlikely to block, worth knowing)

- **F8 · One UI Sans risk.** Community posts (Samsung Members — user-generated, NOT
  official) indicate recent One UI ships a new default font ("One UI Sans"). Live
  re-check during this audit: the official `one_ui6.html` page names no font, and no
  official page found names "One UI Sans". The draft's survey-scoped phrasing survives,
  but this is the single most likely spot where the doc is *factually behind reality
  while technically correctly sourced*. If Samsung publishes an official name later, the
  Typography section takes a mandatory update. Known Gaps already covers the shape of
  this risk.
- **F9 · dark-preview hover interpretation.** `dark.html` uses `--primary-dark-on-dark`
  as a hover *background*; Samsung publishes that value as a dark-theme text/button
  color role. Preview-only styling latitude — not a spec claim, and previews aren't
  spec — but a pixel-hunting reviewer could ask.
- **F10 · `.en.md` decision.** Intake chose `both`, but the repo's collection/tokens
  machinery cannot host two files per slug (BY_SLUG collision + permanent `tokens:check`
  failure). The en text was moved to `research/one-ui-design.en.md`. Right call; the PR
  description should state it so the deviation reads as deliberate.
- **F11 · No logo / `related_services: []` / `category: developer`.** All three are
  known open items: logo omitted pending trademark caution (grid card renders without
  logo), related_services empty, and `developer` vs `etc` is genuinely debatable for an
  OS design language. None block CI; all three belong in the PR description as explicit
  asks to the maintainer.
- **F12 · Android/Material adjacency is disclosed, not contaminated** (verified during
  this audit): window size classes (Compact/Medium/Expanded, 600/840dp) and
  navigation-rail/drawer vocabulary are Android conventions **restated on Samsung's own
  pages** → adoption is explicit; WCAG-derived contrast ratios are stated on Samsung's
  accessibility pages and the draft says so; the Android categorized-palette description
  is followed immediately by a guard sentence ("Material 규칙이 One UI 규칙이라는 뜻이
  아니다") and a dedicated Don't. No undisclosed Material import found.

---

## Classification summary (by special-attention area)

| Area | Statements | VERIFIED | PARTIAL | INFERRED | UNSOURCED |
|---|---|---|---|---|---|
| Exact dimensions (24dp, 600/840/960dp, 3/5 windows) | 8 | 8 | — | — | — |
| Spacing (margins, zones, cutout) | 5 | 4 | 1 (dp→px 매핑 — 선언됨) | — | — |
| Radius (26/20/12, 18) | 4 | 3 | 1 (18dp 강도 — 캐비엇 선언됨) | — | — |
| Typography | 6 | 4 | 1 (웹폰트 스택 — 선언됨) | — | 1 (weights — 선언됨, 비주장) |
| Colors | 10 | 7 | 3 (F4 coined names, F6 stamp) | — | — |
| Component behavior | 22 | 20 | 1 (F3 dialog synthesis) | — | 1 (**F2 rationale**) |
| Foldable behavior | 11 | 11 | — | — | — |
| Large-screen behavior | 9 | 9 | — | — | — |
| Version-specific handling | 8 | 6 | 2 (F5 absence phrasing, F6) | — | — |
| Motion / Sound / Writing / A11y | 24 | 24 | — | — | — |
| Do's & Don'ts / Applied Guidance | 19 | 16 cited | — | 3 (섹션 단위로 해석 선언됨) | — |

Reject-realistic items: **F1 (format-invalid audit notes)** and **F2 (invented
rationale)**. F3–F7 are strict-reviewer friction. Numeric layer: clean (see
numeric-claims.md — 0 removals).

## Recommended fix order before PR

1. F1 — relabel both audit-note blockquotes to regex-valid form (+ keep date = lookup date).
2. F2 — delete/mark the gesture-conflict rationale.
3. F3 — de-stretch the two dialog citations.
4. F5 — normalize absence phrasing to survey-scoped.
5. F4 — declare the two coined token names.
6. F6, F7 — optional polish.
7. PR description: state F10/F11 decisions explicitly.

`last_updated` note: all fixes land before the first commit, so `check:last-updated`
sees one consistent date (2026-08-13) — no further bump needed if committed today.

---

## Resolution log (2026-08-13, same session)

All fixes applied to `services/samsung-one-ui.md`; F8–F12 remain informational.

- **F1 fixed** — both blockquotes relabelled `> **발행값 대조 — One UI 2 세대 2019-10 발행분(2026-08-13).**`. Proof the fix works: the linter immediately began *recognizing* the notes and flagged a real `audit-note-placement` warn in `## Rounded` (blockquote was second paragraph) — moved to first paragraph; warn cleared.
- **F2 fixed** — invented gesture-conflict rationale replaced with "이유는 발행되어 있지 않으므로 규칙만 이식한다".
- **F3 fixed** — dialog-choice: citation de-stretched, linkage marked "(연결은 카탈로그 해석)"; dialog-info: 가시성 gloss deleted; Components intro linkage likewise marked.
- **F4 fixed** — coined-name declaration added under the Colors yaml (`primary-dark-on-dark`/`black-dark` = catalog-assigned names).
- **F5 fixed** — 12 assertive-absence phrasings normalized to survey-scoped ("공개 조사 범위에서 확인되지 않았다") across Colors/Typography/Spacing/Elevation/Shapes/toast/Accessibility/Foldables/Applied Guidance/Known Gaps.
- **F6 fixed** — the four developer-page color tokens restamped "무버전 발행 페이지, 2019 가이드라인과 일치"; PDF-dated values keep "One UI 2(2019) 발행값".
- **F7 fixed** — "가장 durable한 부분" superlative removed from the Components intro.

Post-fix gates: `tokens:build` regenerated (notes carry the new stamps) · `validate:draft` ok ·
`validate:catalog` samsung ok 0 warn (audit notes now *visible* to the linter and passing) ·
`tokens:check` 18 in sync · `audit:oklch` 0 mismatch · `validate:sources` ok.
