# samsung-one-ui — Claim Traceability Matrix

> Maps every One UI-specific factual statement in `services/samsung-one-ui.md` to its
> claim IDs in [`research/one-ui-claims.md`](./one-ui-claims.md). The production file
> exposes only `[src:N]` citations (repository convention); this matrix carries the
> claim-ID layer so each statement stays independently re-verifiable.
> `[src:N]` in the production doc == frontmatter `sources[N-1]` == the Source URL of the
> mapped claims below (the claim registry records the same URLs).
>
> Statement types used in the production doc:
> **stated** = Samsung-stated (plain prose + `[src:N]`) · **interp** = implementation
> interpretation (marked "카탈로그 해석" / "해석" in the doc, no fabricated citation) ·
> **observed** = observation (marked "(관찰)").

| design.md location | Statement | Type | Claim IDs | [src:N] |
|---|---|---|---|---|
| lead | Cross-device scope (phone/tablet/watch/earbud/PC) | stated | OUI-001 | 1 |
| lead | Numeric tokens trace to 2019 guidelines (One UI 2 era) | stated | OUI-081–084, 042, 089, 145 provenance | 9 |
| Brand & Style | "joyful and comfortable" goal | stated | OUI-001 | 1 |
| Brand & Style | Seamless device connection + simplicity | stated | OUI-002, OUI-003 | 2 |
| Brand & Style | Developer-portal 4 principles | stated | OUI-006 | 1 |
| Brand & Style | Design-portal 4 principles (different names) | stated | OUI-016 | 2 |
| Brand & Style | Watch/Tizen set differs (no canonical list) | stated | OUI-023 | (prose note; detailed in Known Gaps) |
| Brand & Style | Viewing/interaction split | stated | OUI-009, OUI-018 | 1, 2 |
| Brand & Style | Reachability on large devices; one-handed | stated | OUI-010, OUI-017, OUI-043 | 1, 2 |
| Brand & Style | Focus on content; remove the unnecessary; short journeys | stated | OUI-007, OUI-008, OUI-019, OUI-020 | 1, 2 |
| Brand & Style | Responsive adaptation, controls in reach | stated | OUI-014, OUI-015 | 1 |
| Brand & Style | Dark mode/high-contrast keyboard/variable font sizes | stated | OUI-011, OUI-012, OUI-013 | 1 |
| Brand & Style | One UI 7 circle motif (version-labelled) | stated | OUI-004, OUI-005 | 38 |
| Colors (blockquote) | Provenance: role colors from color page + 2019 PDF; One UI 7 unpublished | stated | OUI-078–084, OUI-096 | 7, 9, 38 |
| Colors | Rich solid colors; brightness/saturation ranges (unpublished figures) | stated | OUI-077 | 7 |
| Colors | Role usages (Primary/Primary dark/Color control activated) | stated | OUI-078, OUI-079, OUI-080 | 7 |
| Colors yaml | primary #0381fe | stated | OUI-078 | 7 |
| Colors yaml | primary-dark #0072de / on-dark #3e91ff | stated | OUI-079 | 7 |
| Colors yaml | color-control-activated #3e91ff | stated | OUI-080 | 7 |
| Colors yaml | white #fafafa · black #000000 · black-dark #080808 | stated | OUI-081, OUI-082, OUI-083 | 9 |
| Colors | Shared #3e91ff is published data, not an error | stated | OUI-079, OUI-080 | 7 |
| Colors | Android categorized-palette mechanism ≠ Material rules | stated + interp guard | OUI-084 | 9 |
| Colors | Dark mode backgrounds black/dark gray; test both | stated | OUI-086, OUI-087 | 8 |
| Colors | Bezel-merge rationale for near-black | stated | OUI-088 | 9 |
| Colors | Dark-mode switch at desired/set time recommended | stated | OUI-085 | 9 |
| Typography | No published type scale | stated (absence) | OUI-089 Notes, OUI-091 | Known Gaps |
| Typography | Roboto default (2019) | stated | OUI-089 | 9 |
| Typography | SamsungOne = brand typeface (26/400+/25,000+) | stated | OUI-090 | 10 |
| Typography | Variable font sizes; 200% resize | stated | OUI-013, OUI-146 | 1, 30 |
| Typography yaml | Roboto+Pretendard stack & Google Fonts src | interp (marked) | — (substitution, no Samsung claim) | — |
| Spacing | ≥24dp side margins | stated | OUI-038 | 4, 9 |
| Spacing | Reject/Grip zones (no sizes) | stated | OUI-039, OUI-040 | 4 |
| Spacing | Viewing-area wide margins | stated | OUI-032 | 3 |
| Spacing | Camera cutout avoidance (90°/270°) | stated | OUI-041 | 4 |
| Spacing yaml | 24px value with dp→px note | stated + interp (unit mapping marked) | OUI-038 | 4 |
| Rounded (blockquote) | Provenance: 2019 PDF + button page | stated | OUI-042, OUI-110 | 9, 16 |
| Rounded yaml | thumbnail 26/20/12dp | stated | OUI-042 | 9 |
| Rounded yaml | button 18dp (code-spec strength note) | stated | OUI-110 | 16 |
| Rounded | Standardized rounded corners principle | stated | OUI-022 | 2 |
| Elevation & Depth | blur/dim/shadow roles; no dim+shadow; even dim | stated | OUI-025–028 | 6 |
| Elevation & Depth | No published figures | stated (absence) | OUI-025 Notes | Known Gaps |
| Elevation & Depth | One UI 7 colored glass/gradients (labelled) | stated | OUI-029, OUI-030 | 38 |
| Shapes | Rounded-corner standardization; circle motif | stated | OUI-022, OUI-004 | 2, 38 |
| Shapes | Icon square bg + rounded corners/outlines | stated | OUI-092 | 11 |
| Shapes | Vibrant bg + white symbols | stated | OUI-093 | 12 |
| Shapes | Gradient ≤3 analogous colors | stated | OUI-094 | 12 |
| Shapes | Rounded stroke terminals, sharp corners | stated | OUI-095 | 9 |
| Shapes | One UI 7 icon visuals (AI-simulated imagery) | observed (marked "(관찰)") | OUI-096 | 38 |
| Components/app-bar | Standard+extended forms; ≤3 action buttons | stated | OUI-097, OUI-098 | 13 |
| Components/app-bar-extended | Centered title; scroll condense/expand | stated | OUI-097, OUI-099 | 13 |
| Components/bottom-bar | Max 5; no single button; overflow 4+More; icon+text; scroll hide | stated | OUI-100–103 | 14 |
| Components/bottom-navigation | <4 rec / max 5; text-only; no swiping; title omission | stated | OUI-104–106 | 15 |
| Components/button-flat | Flat in toolbars/dialogs; accent text | stated | OUI-107, OUI-108 partial | 16, 7 |
| Components/button-contained | Gray=moderate, color=high; one style/screen; 18dp | stated | OUI-107–110 | 16, 7 |
| Components/dialog-choice | Bottom placement; persistence | stated | OUI-111, OUI-113 | 17, 1 |
| Components/dialog-info | Center placement; popup limits | stated | OUI-112, OUI-137 | 17, 26 |
| Components/list-item | 31 chars; right toggle; priority order | stated | OUI-114, OUI-115 | 18 |
| Components/search | Auto-complete/predictive; pre-typing suggestions | stated | OUI-116, OUI-117 | 19 |
| Components/toast | ~1 line, ≤3; minor info only; no duration figure | stated | OUI-118, OUI-119 | 20 |
| Motion | Engagement/instant/smooth | stated | OUI-121–123 | 21 |
| Motion | 100–500ms | stated | OUI-124, OUI-125 | 22 |
| Motion | Interpolator [0.22,0.25,0,1]; accelerate-then-slow | stated | OUI-126, OUI-127 | 22 |
| Motion | CSS cubic-bezier mapping | interp (marked) | — | — |
| Motion | Image/text cross-fade rules | stated | OUI-128 | 22 |
| Sound & Haptics | Only-when-necessary; input vs cancel/delete; sine | stated | OUI-129–131 | 23 |
| Sound & Haptics | Crisp haptics; special keys; visual sync | stated | OUI-132–134 | 24 |
| Writing | Purposeful text; action not dead end | stated | OUI-135, OUI-136 | 25 |
| Writing | Popup limits; singular they | stated | OUI-137, OUI-138 | 26 |
| Writing | One question; state solution; no blame | stated | OUI-139–141 | 27 |
| Writing | Korean register unpublished | stated (absence) | — | Known Gaps |
| Accessibility | 4C principles | stated | OUI-142 | 28 |
| Accessibility | 4.5:1 / 3:1 (+18dp/14dp definition) | stated | OUI-143, OUI-144 | 29 |
| Accessibility | 2019 per-size contrast table | stated | OUI-145 | 9 |
| Accessibility | 200% resize | stated | OUI-146 | 30 |
| Accessibility | 5s auto-play stop | stated | OUI-148 | 31 |
| Accessibility | Touch-area sufficiency, NO dp figure | stated (absence guarded) | OUI-147 | 30 |
| Accessibility | Gesture alternatives; consistent locations | stated | OUI-149, OUI-150 | 31 |
| Accessibility | Focus rules; no looping; no decorative focus | stated | OUI-151–153 | 32 |
| Accessibility | No shape/color/location-only refs; audio+visual; no strobing | stated | OUI-154–156 | 33 |
| Accessibility | No color-only info; grayscale check | stated | OUI-157 | 29 |
| Do's | Each Do restates a cited rule above | stated | (per-row mapping above) | 3,4,8,14,16,17,22,29,30,34 |
| Don'ts | No swipe tabs / no dim+shadow / no color-only | stated | OUI-106, OUI-026, OUI-157 | 15, 6, 29 |
| Don'ts | No invented figures | interp (catalog policy) | absence claims (OUI-147 Notes etc.) | — |
| Don'ts | Material ≠ One UI | stated + interp guard | OUI-084 + catalog policy | 9 |
| Don'ts | Domain boundary (system surfaces, cover/main) | stated basis + catalog policy | OUI-024, OUI-066 | 5, 36 |
| Don'ts | Vendor neutrality / not-official | catalog policy (no citation needed) | — | — |
| Responsive/Window classes | 600/840 classes; device mapping; per-class nav | stated | OUI-049–053, OUI-057–059 | 34, 35 |
| Responsive/Large screens | No stretching; 42:58 & 38:62 @960; 4 principles | stated | OUI-054–056, OUI-045 | 34, 35 |
| Responsive/Foldables | 50:50; continuity ×3; cover/main; letterbox; crease; Flex | stated | OUI-060–070, OUI-072 | 34, 36 |
| Responsive/Multi-window | 3 split + 5 popup; drag-drop; multi-instance | stated | OUI-073, OUI-075, OUI-076 | 34, 37 |
| Applied Guidance (all 10 items) | Synthesis of cited rules into directives | interp (section-level marked "카탈로그 해석") | derived from rows above | section intro states this |
| Known Gaps (all bullets) | Absence statements | stated (absence) | OUI-016/023 (sets), OUI-089/090/091, OUI-147, OUI-077, OUI-096 Notes | 1,2,4,6,7,9,10,20,30,38 |

## Coverage check

- Every numeric value in the production doc (hex ×6, 24dp, 26/20/12dp, 18dp, 100–500ms, interpolator, 4.5:1/3:1, 18dp/14dp, 200%, 5s, 600/840/960dp, 42:58/38:62/50:50, 3/5 windows, ≤3/≤5/<4/31자/3줄 counts) maps to an EXPLICIT claim with an exact official source.
- Zero INFERRED claims were promoted to rules. The two OBSERVED claims (OUI-091, OUI-096) appear only as an absence note and a "(관찰)"-marked line.
- Interpretations carry no `[src:N]` of their own and are explicitly marked in the production prose (`카탈로그 해석`, unit-mapping notes, CSS notation mapping).
