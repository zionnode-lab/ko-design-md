# samsung-one-ui — Numeric Value Audit

> Full audit of EVERY design-related numerical value in the production design context
> (`services/samsung-one-ui.md`). Each value gets a `NUM-xxx` ID, cross-referenced to the
> claim registry ([`one-ui-claims.md`](./one-ui-claims.md)) and to the exact official source.
>
> **Verification rules applied:**
> - VERIFIED only when a publicly accessible **official Samsung** source explicitly states the value.
> - Screenshot-only visibility ≠ official spec.
> - Android/Material documentation values are NOT One UI values unless Samsung explicitly adopts them (none in this doc rely on Material docs; the contrast thresholds are WCAG-derived but **stated verbatim on Samsung's own pages**, which qualifies).
> - Third-party One UI clones were never used (none cited anywhere in the pipeline).
>
> **Scope notes:** dates/version numbers (2019-10, One UI 2/7, 2025, Galaxy S25) are provenance metadata, not design values — excluded. The line "48dp 같은 값을 임의로 쓰지 말고" contains 48dp only as a **prohibited example** (a guard against invention), not a claimed value — classified separately at the end.

---

## A. Colors (hex + OKLCH)

### NUM-001
Claim ID: OUI-078
Value: `#0381fe` (as `oklch(0.617 0.208 255.8)`)
Context: `## Colors` yaml — `primary` role (FAB, 슬라이더, 입력 필드, 포커스)
Official source URL: https://developer.samsung.com/one-ui/color/system.html
Exact official support: "Primary #0381fe" listed for both Light and Dark theme; corroborated by the 2019 PDF.
Status: VERIFIED
Note: The OKLCH triplet is the catalog's deterministic sRGB→OKLCH conversion of the verified hex (repo policy: token values OKLCH-only, source hex kept as trailing comment). `audit:oklch` machine-checks the pairing — 0 mismatches.

### NUM-002
Claim ID: OUI-079
Value: `#0072de` (as `oklch(0.561 0.186 255.2)`)
Context: `## Colors` yaml — `primary-dark`, Light-theme value
Official source URL: https://developer.samsung.com/one-ui/color/system.html
Exact official support: "Primary dark — Light: #0072de."
Status: VERIFIED

### NUM-003
Claim ID: OUI-079
Value: `#3e91ff` (as `oklch(0.661 0.182 256.7)`)
Context: `## Colors` yaml — `primary-dark-on-dark` (Primary dark의 Dark 테마 값)
Official source URL: https://developer.samsung.com/one-ui/color/system.html
Exact official support: "Primary dark — Dark: #3e91ff."
Status: VERIFIED

### NUM-004
Claim ID: OUI-080
Value: `#3e91ff` (as `oklch(0.661 0.182 256.7)`)
Context: `## Colors` yaml — `color-control-activated` (체크박스·라디오·토글 활성)
Official source URL: https://developer.samsung.com/one-ui/color/system.html
Exact official support: "Color control activated — #3e91ff" for both themes.
Status: VERIFIED
Note: Duplicate of NUM-003's hex by publication, not transcription — the doc states this explicitly.

### NUM-005
Claim ID: OUI-081
Value: `#fafafa` (as `oklch(0.985 0 0)`)
Context: `## Colors` yaml — `white`, 양 테마 동일
Official source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Exact official support: Palette table "White #fafafa" (Light and Dark).
Status: VERIFIED (version-specific: One UI 2/2019 — stamped in doc)

### NUM-006
Claim ID: OUI-082
Value: `#000000` (as `oklch(0 0 0)`)
Context: `## Colors` yaml — `black`, Light 테마
Official source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Exact official support: "Black #000000" (Light theme).
Status: VERIFIED (version-specific, stamped)

### NUM-007
Claim ID: OUI-083
Value: `#080808` (as `oklch(0.134 0 0)`)
Context: `## Colors` yaml — `black-dark`, Dark 테마 배경(근흑)
Official source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Exact official support: "Black #080808" (Dark theme).
Status: VERIFIED (version-specific, stamped)

## B. Spacing / grid

### NUM-008
Claim ID: OUI-038
Value: 24 dp (yaml로는 `24px` + "공식 표기 24dp" 주석)
Context: `## Spacing` — 좌우 최소 마진 규칙 + `margin-side-min` 토큰
Official source URL: https://developer.samsung.com/one-ui/layout/grid.html
Exact official support: "place interactive components with margins of at least 24 dp on both the left and right sides." (2019 PDF restates "at minimum 24dp margins on each side.")
Status: VERIFIED
Note: The **dp→px 1:1 web mapping** is a catalog interpretation, explicitly declared on the token line ("웹 1dp≈1px 매핑은 카탈로그 해석"). The dp value itself is official; the unit mapping is not a Samsung claim.

### NUM-009
Claim ID: OUI-041
Value: 90° / 270°
Context: `## Spacing` — 카메라 컷아웃 회피 가이드의 회전 방향
Official source URL: https://developer.samsung.com/one-ui/layout/grid.html
Exact official support: Cutout guidance addresses 90° and 270° orientations.
Status: VERIFIED

## C. Radius

### NUM-010
Claim ID: OUI-042
Value: 26 dp (`radius-thumbnail-l: 26px`)
Context: `## Rounded` yaml — 큰 포커스 블록/썸네일
Official source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Exact official support: Thumbnail radius section, "Radius=26dp."
Status: VERIFIED (version-specific: One UI 2/2019 — provenance blockquote + per-line stamp)

### NUM-011
Claim ID: OUI-042
Value: 20 dp (`radius-thumbnail-m: 20px`)
Context: `## Rounded` yaml — 중간 썸네일
Official source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Exact official support: "Radius=20dp."
Status: VERIFIED (version-specific, stamped)

### NUM-012
Claim ID: OUI-042
Value: 12 dp (`radius-thumbnail-s: 12px`)
Context: `## Rounded` yaml — 작은 썸네일
Official source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Exact official support: "Radius=12dp."
Status: VERIFIED (version-specific, stamped)

### NUM-013
Claim ID: OUI-110
Value: 18 dp (`radius-button: 18px`)
Context: `## Rounded` yaml + `### button-contained` — 버튼 코너 radius
Official source URL: https://developer.samsung.com/one-ui/comp/button.html
Exact official support: "18dp" appears in the button mask/background drawable XML shown on the official page.
Status: VERIFIED — with an explicit strength caveat
Note: The value is on an official Samsung page but inside a code sample, not rule prose. The production doc **already discloses this** ("규칙 산문이 아니라 공식 페이지의 구현 스펙(XML) 안에 있는 값이므로, 규칙 강도는 그만큼 낮게 취급한다"). Keep with that caveat intact.

## D. Motion

### NUM-014
Claim ID: OUI-124
Value: 100 ms (최소)
Context: `## Motion` — 지속시간 하한
Official source URL: https://developer.samsung.com/one-ui/motion/basic.html
Exact official support: "at least 100 ms, which is the minimum recognizable length."
Status: VERIFIED

### NUM-015
Claim ID: OUI-125
Value: 500 ms (상한)
Context: `## Motion` — 지속시간 상한
Official source URL: https://developer.samsung.com/one-ui/motion/basic.html
Exact official support: "should never exceed 500 ms."
Status: VERIFIED

### NUM-016
Claim ID: OUI-126
Value: `[0.22, 0.25, 0.00, 1.00]` (CSS 표기 `cubic-bezier(0.22, 0.25, 0, 1)`)
Context: `## Motion` — Basic Path Interpolator
Official source URL: https://developer.samsung.com/one-ui/motion/basic.html
Exact official support: Basic Path Interpolator "[0.22, 0.25, 0.00, 1.00]."
Status: VERIFIED
Note: The CSS `cubic-bezier` rewrite is a notation mapping (same four constants), declared as catalog interpretation in the doc.

## E. Components (counts / limits)

### NUM-017
Claim ID: OUI-098 · Value: ≤ 3 (앱바 액션 버튼/페이지) · Context: `### app-bar`
Official source URL: https://developer.samsung.com/one-ui/comp/app-bar.html
Exact official support: "We recommend no more than three buttons on any page."
Status: VERIFIED

### NUM-018
Claim ID: OUI-100 · Value: 최대 5 (바텀 바 버튼) · Context: `### bottom-bar`
Official source URL: https://developer.samsung.com/one-ui/comp/bottom-bar.html
Exact official support: "maximum of 5 action buttons."
Status: VERIFIED

### NUM-019
Claim ID: OUI-101 · Value: 1개 표시 금지 (바텀 바) · Context: `### bottom-bar`
Official source URL: https://developer.samsung.com/one-ui/comp/bottom-bar.html
Exact official support: "can't display only one action button."
Status: VERIFIED

### NUM-020
Claim ID: OUI-102 · Value: 4 (오버플로우 시 표시 버튼 수) · Context: `### bottom-bar`
Official source URL: https://developer.samsung.com/one-ui/comp/bottom-bar.html
Exact official support: "the four most-used action buttons can be displayed."
Status: VERIFIED

### NUM-021
Claim ID: OUI-104 · Value: < 4 권장, 최대 5 (바텀 내비 탭) · Context: `### bottom-navigation`, Applied Guidance #3
Official source URL: https://developer.samsung.com/one-ui/comp/bottom-navigation.html
Exact official support: "has to display less than 4"; "maximum of 5 can be displayed."
Status: VERIFIED

### NUM-022
Claim ID: OUI-114 · Value: 31자 (리스트 메인 텍스트) · Context: `### list-item`
Official source URL: https://developer.samsung.com/one-ui/comp/list.html
Exact official support: "keep them within 31 characters."
Status: VERIFIED

### NUM-023
Claim ID: OUI-118 · Value: ≤ 3줄 / 약 1줄 (토스트) · Context: `### toast`
Official source URL: https://developer.samsung.com/one-ui/comp/toast.html
Exact official support: "Toasts should be about one line, and should never exceed 3 lines in any language."
Status: VERIFIED

### NUM-024
Claim ID: OUI-139 · Value: 1 (수사적 질문 개수 제한) · Context: `## Writing`
Official source URL: https://developer.samsung.com/one-ui/writing/empowering.html
Exact official support: "limit it to one."
Status: VERIFIED

## F. Accessibility

### NUM-025
Claim ID: OUI-143
Value: 4.5:1 (작은 텍스트 대비)
Context: `## Accessibility`, Do's
Official source URL: https://developer.samsung.com/one-ui/accessibility/color-contrast.html
Exact official support: "small text should have at least a 4.5:1 contrast with the background color."
Status: VERIFIED
Note: WCAG-derived, but stated verbatim on Samsung's official page → Samsung explicitly adopts it (passes the "not Material/Android unless adopted" rule).

### NUM-026
Claim ID: OUI-144
Value: 3:1 + 큰 텍스트 정의(일반 > 18 dp, 볼드 > 14 dp)
Context: `## Accessibility`
Official source URL: https://developer.samsung.com/one-ui/accessibility/color-contrast.html
Exact official support: "For large text (more than 18 dp for normal text or 14 dp for bold text), the contrast should be at least 3:1."
Status: VERIFIED

### NUM-027
Claim ID: OUI-145
Value: 크기 구간별 대비 표 — 12–13 dp → 4.5:1/4.5:1 · 14, 17 dp → 4.5:1/3:1 · 18, 19+ dp → 3:1/3:1
Context: `## Accessibility` (2019 표로 명시 인용)
Official source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Exact official support: Contrast table rows "~12 … 4.5:1/4.5:1", "13 …", "14 … 4.5:1/3:1", "17 …", "18 … 3:1/3:1", "19~ …".
Status: VERIFIED (version-specific: 2019 PDF — labelled in doc)

### NUM-028
Claim ID: OUI-146 · Value: 200% (텍스트 확대) · Context: `## Accessibility`, `## Typography`, Do's
Official source URL: https://developer.samsung.com/one-ui/accessibility/layout-and-typo.html
Exact official support: "resizable up to 200% without affecting content or functionality."
Status: VERIFIED

### NUM-029
Claim ID: OUI-148 · Value: 5초 (자동 재생 중지 컨트롤 기준) · Context: `## Accessibility`
Official source URL: https://developer.samsung.com/one-ui/accessibility/interaction-and-control.html
Exact official support: "give users controls to stop content lasting more than 5 seconds."
Status: VERIFIED

## G. Breakpoints / large screens / foldables / multi-window

### NUM-030
Claim ID: OUI-049 · Value: 600 dp (대형 화면 임계) · Context: `## Responsive Behavior`, Applied Guidance #8
Official source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Exact official support: "Use a large screen layout for screens with a width of 600dp or more."
Status: VERIFIED

### NUM-031
Claim ID: OUI-050 · Value: 윈도우 클래스 경계 600 / 840 dp · Context: Responsive 표
Official source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Exact official support: Compact "(Width < 600)"; Medium "(600 ≤ Width < 840)"; Expanded "(840 ≤ Width)".
Status: VERIFIED

### NUM-032
Claim ID: OUI-054 · Value: 42% : 58% @ 600 ≤ w < 960 dp · Context: Responsive/Large screens
Official source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Exact official support: Breakpoint table "600 ≤ Width < 960" → "42%" / "58%".
Status: VERIFIED
Note: The 960 dp ratio threshold differs from the 840 dp class threshold — both official; the doc states this coexistence explicitly.

### NUM-033
Claim ID: OUI-055 · Value: 38% : 62% @ w ≥ 960 dp · Context: Responsive/Large screens
Official source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Exact official support: "960 ≤ Width" → "38%" / "62%".
Status: VERIFIED

### NUM-034
Claim ID: OUI-060 · Value: 50% : 50% (폴더블 전용) · Context: Responsive/Foldables, Applied Guidance #8
Official source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Exact official support: "Foldable only" row → "50%"/"50%".
Status: VERIFIED (foldable-only labelled in doc)

### NUM-035
Claim ID: OUI-073 · Value: 분할 3개 + 팝업 5개 · Context: Responsive/Multi-window
Official source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Exact official support: "up to 3 split screen view and 5 pop-up view open simultaneously."
Status: VERIFIED

## H. Typeface facts (non-token numerics)

### NUM-036
Claim ID: OUI-090
Value: 26개 문자 체계 · 400+ 언어 · 25,000+ 글리프
Context: `## Typography` — SamsungOne 브랜드 타이페이스 서술 (토큰 아님)
Official source URL: https://design.samsung.com/global/contents/samsungone/
Exact official support: "26 writing systems, more than 400 languages, and over 25,000 glyphs."
Status: VERIFIED

### NUM-037
Claim ID: — (no OUI; declared interpretation)
Value: Roboto 웹폰트 weight 400 / 500 / 700 (`font-sans-src` URL 파라미터 포함)
Context: `## Typography` yaml 스택 + 해석 문단
Official source URL: 없음 (Google Fonts 배포 파라미터)
Exact official support: NONE as a One UI weight policy — and the doc says so verbatim: "weight는 Roboto 배포본의 400/500/700을 사용하되, **One UI가 발행한 weight 정책은 아니다**."
Status: UNSOURCED (as a One UI spec) — but **not presented as one**; explicitly declared a catalog web-substitution parameter
Disposition: see removal list.

## I. Icon rules

### NUM-038
Claim ID: OUI-094 · Value: ≤ 3색 (아이콘 그라디언트 유사색) · Context: `## Shapes`
Official source URL: https://developer.samsung.com/one-ui/iconography/color.html
Exact official support: "3 or fewer analogous colors."
Status: VERIFIED

## J. Guard values (numbers present only as prohibitions)

### NUM-039
Claim ID: OUI-147 (absence claim)
Value: 48 dp — **appears only as a prohibited example**
Context: `## Accessibility` — "공식 터치 타겟 dp 수치는 발행되지 않았다 — 48dp 같은 값을 임의로 쓰지 말고…"
Official source URL: https://developer.samsung.com/one-ui/accessibility/layout-and-typo.html (states NO figure)
Exact official support: N/A — the sentence asserts the absence of an official figure and forbids substituting 48dp (a Material/Android convention).
Status: N/A (guard against invention — this is the enforcement of the audit's own rule, not a claim)

---

## Summary table

| Status | Count | IDs |
|---|---|---|
| VERIFIED | 37 | NUM-001…036, NUM-038 |
| UNSOURCED (declared interpretation, not presented as One UI) | 1 | NUM-037 |
| AMBIGUOUS | 0 | — |
| OBSERVED_ONLY | 0 | — |
| N/A (guard) | 1 | NUM-039 |

Additional cross-cutting interpretation (not a standalone value): the **dp→px 1:1 mapping** used to express dp values as px in the token yaml (NUM-008, 010–013). The dp originals are VERIFIED; the mapping is declared on each affected line and in prose. No hidden conversions exist.

**Preview HTML note:** `public/preview/samsung-one-ui/*.html` additionally contains layout craft values (paddings, demo font sizes, 250ms transitions, neutral surface OKLCHs). None are presented as One UI specs — the files label derived surfaces "카탈로그 해석 (md 토큰 아님)", the 250ms transition sits inside the verified 100–500ms band, and button radius/margins reuse the verified 18px/24px. No preview value leaks into the production design context.

---

## Values that should be REMOVED from the production design context

**None.**

Every numerical value in `services/samsung-one-ui.md` is either (a) VERIFIED against an explicit official Samsung source, (b) a declared, clearly-labelled catalog interpretation that is *not presented as a One UI value* (NUM-037 font weights; the dp→px unit mapping), or (c) a guard value that exists specifically to *prevent* an invented number from entering (NUM-039's 48dp).

Conditional watch-list — keep only while their disclaimers stay intact:

1. **NUM-037 (Roboto 400/500/700)** — keep only together with the sentence "One UI가 발행한 weight 정책은 아니다". If a reviewer objects, the fallback is to drop the three weights from the stack prose and keep only the `font-sans-src` URL (where they are loading parameters, not claims).
2. **dp→px mapping (NUM-008, 010–013)** — keep only with the per-line "공식 표기 Ndp" comments; removing those comments would silently promote px values to false precision.
3. **NUM-013 (18dp button radius)** — keep only with the code-spec strength caveat sentence; without it the value reads as normative rule prose.
