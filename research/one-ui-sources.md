# Samsung One UI — Official Public Source Evidence Catalog

> Research input for a ko-design-md `samsung-one-ui` entry. **Not a design.md.**
> Every finding below is drawn from a **publicly accessible, official Samsung source**
> (`developer.samsung.com`, `design.samsung.com`). No third-party sources, no internal
> documents, no leaked or unreleased material. Numeric values are recorded ONLY where an
> official page states them explicitly.

## Evidence-type definitions

- **EXPLICIT** — Samsung directly states the rule.
- **OBSERVED** — the behavior/visual treatment is visible in an official Samsung public example but is not stated as a rule.
- **INFERRED** — interpretation is required.

## Rules applied while collecting

- OBSERVED / INFERRED findings are **not** promoted to official rules.
- Every numeric value has a precise official source; numbers not explicitly stated were dropped.
- Exact fetched URLs are recorded. Failed/redirected/404 URLs are noted.
- Version-specific sources are flagged. Current public examples are **not** assumed to represent every One UI version.

## ⚠️ Provenance & version caveats (read before using any number)

1. **Three different official "principle" sets exist.** `developer.samsung.com/one-ui` lists *Focus on the task at hand / Interact naturally / Be visibly comfortable / Make things responsive*. `design.samsung.com/.../one-ui/` lists *One Makes It Natural / One Is Clean and Easy / One Keeps Consistency / One Attracts All Senses*. `developer.samsung.com/one-ui-watch-tizen` lists a **watch-only** set (*Scannable / Easy to Follow / Responsive / Desirable*). Treat them as distinct official statements, not one canonical list. The **durable** cross-cutting ideas (viewing vs interaction area, reachability, cross-device consistency, simplicity) appear in more than one set and are the safest to rely on (satisfies the "prefer durable principles" constraint).
2. **Most concrete hex/dp values come from the 2019 "One UI Design Guidelines" PDF** (`design.samsung.com/.../oneui_design_guide_eng.pdf`, PDF metadata CreationDate **Oct 29 2019**, Samsung Mobile UX Center — the One UI 2 / Android 10 era). These are flagged `Version-specific: YES`. They may **not** represent One UI 7 (2025).
3. **The One UI 7 design page (`design.samsung.com/.../one-ui-7/`) publishes NO numeric tokens** and states some imagery is AI-generated ("simulated for illustrative purposes only"). Anything visual there is OBSERVED marketing, not a token.
4. **System UI font ≠ brand typeface.** The 2019 PDF says One UI's *default system font is Roboto* (the Android system font). *SamsungOne* is Samsung's **brand** typeface (26 writing systems, 400+ languages, 25,000+ glyphs) — a corporate identity face, not stated as the One UI UI-rendering font. Do not conflate them.
5. **Contrast ratios (4.5:1 / 3:1) are WCAG-derived** but are stated on official Samsung accessibility pages, so they are cited as EXPLICIT with that note.
6. **No official touch-target size in dp** was found on any fetched One UI page — accessibility guidance says "large enough… with enough spacing" qualitatively only. Do not invent a 48dp figure.
7. **Two different numeric breakpoint systems coexist** in the large-screen docs: window-size classes use **600 / 840 dp**; multi-pane ratio guidance uses **600 / 960 dp**. Not a transcription error — both are on the official pages.

---

## 1. Design philosophy

---
Claim: One UI's overarching philosophy is to create joyful, comfortable experiences across any Samsung device (phone, tablet, watch, earbud, PC).
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: One UI aims to create "joyful and comfortable experiences on any device, whether it's a phone, tablet, watch, earbud, or PC."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: General cross-device philosophy statement.
---
Claim: On design.samsung.com, One UI's stated purpose is to connect devices for a seamless, simple-to-use experience across the entire on→off usage cycle.
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: "One UI has been designed with the purpose of connecting various devices together to provide a seamless experience, and its simplicity makes it easy to use," covering "every moment… from the moment it is turned on until the moment it is off."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: A separate (design-portal) philosophy statement from the developer-portal one.
---
Claim: One UI 7's visual language centers on the circle as a scalable shape producing soft, curved outlines, aiming for a seamless, balanced design with clear information hierarchy.
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 — Samsung Design
Evidence type: EXPLICIT
Evidence: "Utilizing a circle, a simple shape with high scalability, soft and elegant curved outlines appear as a visual element across the screen," for "a visually seamless, balanced design" clarifying "the hierarchy of information across components and contents."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: Explicitly One UI 7; marketing/design-portal framing. No numbers.
---

## 2. Core design principles

---
Claim: The developer portal states four One UI principles: Focus on the task at hand; Interact naturally; Be visibly comfortable; Make things responsive.
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: The overview enumerates "Focus on the task at hand," "Interact naturally," "Be visibly comfortable," "Make things responsive."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: The phone/tablet principle set. Differs from the design-portal set below.
---
Claim: "Focus on the task at hand" — simple, intuitive design keeps users focused on content and shortens user journeys.
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "One UI uses simple, intuitive designs to help users focus on content" and "makes user journeys as short and smooth as possible."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: none
---
Claim: "Interact naturally" — the screen is split into a viewing area (top) and interaction area (bottom), keeping interactive elements within easy reach even on large devices.
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Describes a viewing area at top and interaction area at bottom and "places interactive elements within easy reach, even on large devices."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Core reachability statement at the philosophy level.
---
Claim: "Be visibly comfortable" — covers accessibility affordances such as Dark mode, a high-contrast keyboard, and variable font sizes/styles.
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Cites Dark mode to reduce eye fatigue/glare, a high-contrast keyboard, and "Variable font sizes and styles to make text accessible to anyone."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: none
---
Claim: "Make things responsive" — the One UI layout adapts to any device or screen size while keeping interface elements within reach.
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The layout of One UI adapts so it's easy to use on any device or screen size," with elements remaining within reach.
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: none
---
Claim: The design portal states a differently-named four-principle set: One Makes It Natural; One Is Clean and Easy; One Keeps Consistency; One Attracts All Senses.
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: Named principles "One Makes It Natural," "One Is Clean and Easy," "One Keeps Consistency," "One Attracts All Senses."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: IMPORTANT — differs from the developer-portal set; may reflect earlier One UI branding. Two official portals, two lists.
---
Claim: "One Makes It Natural" emphasizes single-handed operation with clearly distinguished viewing and touching areas.
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: Emphasizes single-handed operation "with areas for viewing and touching clearly distinguished."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: Corroborates the viewing/interaction-area split from a second official source (under a different principle name).
---
Claim: "One Is Clean and Easy" focuses on essence and removes unnecessary elements to guide users to important functions.
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: "One UI focuses on the essence, which gives a clean and concise first impression," removing unnecessary elements.
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: none
---
Claim: "One Keeps Consistency" unifies experiences across devices using standardized elements such as rounded corners.
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: "One UI brings all these smart device experiences together into a uniform, one experience," standardizing appearance with elements like rounded corners.
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: No numeric corner radius stated here.
---
Claim: One UI Watch (Tizen) uses a separate principle set: Scannable, Easy to Follow, Responsive, Desirable.
Source URL: https://developer.samsung.com/one-ui-watch-tizen/principle.html
Source title: One UI Watch (Tizen) — Design principles (Samsung Developer)
Evidence type: EXPLICIT
Evidence: The four principles are "Scannable," "Easy to Follow," "Responsive," "Desirable."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: WATCH/TIZEN-SPECIFIC — does NOT apply to phone One UI. Listed only to disambiguate principle sets.
---

## 3. Structure & visual depth

---
Claim: One UI's basic structure comprises the Lock screen, Home screen, Recents screen, Quick panel, and Edge panel.
Source URL: https://developer.samsung.com/one-ui/structure/basic.html
Source title: One UI — Basic structure (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Describes Lock screen, Home screen, Recents ("shows scaled-down apps in order of when they were last used"), Quick panel ("check notifications and change settings"), and Edge panels.
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Structural inventory, not measurements.
---
Claim: One UI builds visual hierarchy with blur, dim, and shadow effects to help users focus on important information.
Source URL: https://developer.samsung.com/one-ui/structure/visual-depth.html
Source title: One UI — Visual depth (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "One UI uses blur, dim, and shadow effects to create a hierarchical structure that helps users focus on important information." Blur/dim for unrelated screens; shadow only for closely related screens.
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: none
---
Claim: One UI dictates that the dim effect and shadow effect must not be applied at the same time, and dim should be applied evenly (avoid multiple hierarchy levels on one screen).
Source URL: https://developer.samsung.com/one-ui/structure/visual-depth.html
Source title: One UI — Visual depth (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "A soft shadow effect can be used to show connections between information while maintaining the hierarchy," and "Avoid applying the dim effect and shadow effect at the same time." Dim should be applied evenly.
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: No numeric opacity/blur/shadow values stated.
---
Claim: One UI 7 adds layered blur plus "colored glass" overlays and gradient backgrounds on certain full-screen apps to create depth and texture.
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 — Samsung Design
Evidence type: EXPLICIT
Evidence: A "blur effect" that "creates a sense of depth and delicate texture" combined with "colored glass" overlays; colorful gradients on startup screens and full-background interfaces (Clock, Calendar, Reminder).
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: One UI 7 specific; extends the developer-doc visual-depth concept. No numbers.
---

## 4. Layout

---
Claim: In One UI layout, the top of the screen is the viewing area (titles) and the rest is the interaction area (user actions).
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The top part of the screen is the viewing area where titles appear. The rest of the screen is the interaction area, where user actions occur."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: The most direct viewing-area vs interaction-area statement.
---
Claim: The viewing area uses wide margins, avoids touch-interactive components, and uses center-aligned text for visual stability.
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Viewing area has "wide margins to give the user the impression of open space," "Components that require touch interaction are avoided here," and uses center-aligned text for "greater visual stability."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: "Wide margins" is qualitative here; the 24 dp value is on the grid page.
---
Claim: In the interaction area, actionable components are grouped in logical order; layouts support list, card, 2-column, and 3-column grids, plus focus blocks (card/list/image).
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Actionable components are grouped and placed in a logical order," with list, card, 2-column, and 3-column layouts and focus blocks in card/list/image formats.
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: none
---
Claim: One UI recommends left/right margins of at least 24 dp to avoid conflicts with curved edges/corners.
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "place interactive components with margins of at least 24 dp on both the left and right sides."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Restated in the 2019 PDF ("at minimum 24dp margins on each side"). Phone/tablet grid context; not labeled to a version on the web page.
---
Claim: One UI blocks accidental touches in the margins via a Reject zone (interaction-area touches) and a Grip zone (palm and three-finger touches while holding the phone).
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The Reject zone blocks touches in the interaction area. The Grip zone blocks palm touches and three-finger touches that may occur when the user is holding their phone."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: Zone sizes not stated numerically.
---
Claim: On-screen items should be optimized to avoid the camera cutout, with guidance for 90° and 270° orientations.
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "items displayed on the screen should be optimized to avoid the camera cutout," addressing 90° and 270° orientations.
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: none
---
Claim: One UI recommends focus-block / thumbnail corner radii of 26 dp, 20 dp, or 12 dp depending on the screen grid and target.
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "04. Thumbnail radius… use the following thumbnail radius value according to the screen grid and target." Values: "Radius=26dp", "Radius=20dp", "Radius=12dp".
Confidence: high
Version-specific: YES
Contains numeric value: YES
Notes: 2019 PDF (One UI 2 era). Applies to rounded focus blocks / image thumbnails; may differ in One UI 7.
---

## 5. Viewing area / interaction area  &  6. Reachability

(See §4 for the primary viewing/interaction-area definitions and §2 "Interact naturally".)

---
Claim: One UI's single-handed-reach model places interactive elements toward the bottom so they stay within thumb reach, even on large devices.
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Interaction area at the bottom "places interactive elements within easy reach, even on large devices."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Reachability is a stated One UI rationale, corroborated by the design-portal "single-handed operation" statement (§2).
---
Claim: On large screens, pop-ups should appear near the UI element the user interacted with to reduce finger-travel distance.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "make the pop-up appear near the button or other UI element that the user interacted with… reduces finger travel distance and saves time."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Reachability rule specific to large screens.
---
Claim: One UI's large-screen layout principles include an explicit "Keep things reachable" principle.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Section headings: "Show menus together with content", "Adjust grids for large screens", "Avoid switching context", "Keep things reachable."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: The "keep things reachable" section cites the Camera app placing controls on the right (OBSERVED example, not a numeric rule).
---

## 7. Responsive behavior

---
Claim: One UI is designed to give the best experience across all display sizes, resolutions, and screen ratios — phones, tablets, foldables, DeX monitors, and split-screen.
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "One UI is designed to give the best experience for all display sizes, resolutions, and screen ratios," across phones, tablets, foldables, Samsung DeX external monitors, and split-screen.
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: none
---
Claim: The design portal describes a "Focus Block" that clears content for single-glance viewing and a consistent upward-swipe gesture across screens.
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: A "Focus Block" that "clears content for single-glance viewing," responsive design across mobile/tablet/PC, and an upward swipe that "remains constant across all screens."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: "Focus block" also appears in developer layout docs, corroborating the concept across portals.
---

## 8. Large screens

---
Claim: Use a large-screen layout for any screen 600 dp wide or more.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Use a large screen layout for screens with a width of 600dp or more."
Confidence: high
Version-specific: NO
Contains numeric value: YES
Notes: The fundamental large-screen threshold.
---
Claim: One UI defines three window size classes by width — Compact (< 600 dp), Medium (600 ≤ width < 840 dp), Expanded (840 ≤ width).
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Compact "(Width < 600)"; Medium "(600 ≤ Width < 840)"; Expanded "(840 ≤ Width)".
Confidence: high
Version-specific: NO
Contains numeric value: YES
Notes: Uses 600/840 dp — distinct from the 600/960 dp multi-pane ratio system below.
---
Claim: Window size classes map to device types — Compact = phone portrait; Medium = Z Fold portrait/landscape + small tablet portrait; Expanded = tablet portrait/landscape.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Compact "Phone in portrait"; Medium "Z Fold devices in portrait / landscape; Small tablet in portrait"; Expanded "Tablet in portrait / landscape."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Platform-adaptation mapping tied to specific form factors.
---
Claim: Multi-pane split ratios — 42% / 58% for 600 ≤ width < 960 dp, and 38% / 62% for width ≥ 960 dp.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "600 ≤ Width < 960" → "42%" / "58%"; "960 ≤ Width" → "38%" / "62%".
Confidence: high
Version-specific: NO
Contains numeric value: YES
Notes: Ratio table lives on intro.html and uses a 960 dp breakpoint (not 840 dp).
---
Claim: Avoid stretching phone apps on large screens; use a multi-pane layout to show more information at once.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Stretched-out apps are harder to read and waste the extra space of the large screen. Use a multi-pane layout to show more information at once."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Core large-screen principle.
---
Claim: Large-screen navigation scales by window class — Compact: navigation bar + modal drawer; Medium: navigation rail + modal drawer; Expanded: navigation rail + modal or standard drawer.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Compact "Navigation bar, modal navigation drawer"; Medium "Navigation rail, modal navigation drawer"; Expanded "Navigation rail, modal or standard navigation drawer."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Platform-adaptation guidance.
---

## 9. Foldables

---
Claim: For foldables, a 50% / 50% two-pane split is recommended.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Breakpoint table "Foldable only" row → "50%" for both panes.
Confidence: high
Version-specific: YES
Contains numeric value: YES
Notes: The "50:50" ratio, labeled "Foldable only" (Z Fold class) — a design recommendation, not a hardware split.
---
Claim: App continuity across fold/unfold requires filling the whole screen, preserving scroll position, and keeping text input + keyboard state on screen switches.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "your app should fill the entire screen"; "keep the scroll position the same when switching"; "the text input and keyboard should remain when switching."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Foldable app-continuity requirements.
---
Claim: Foldable responsive checklist — display correctly across sizes/widths/aspect ratios, support landscape, display correctly on both cover and main screens, and fill the screen without letterboxing.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "displays correctly on screens with various sizes, widths, and aspect ratios"; "supports landscape orientation"; "displays correctly on both the cover screen and main screen"; "fills the entire screen without letterboxing."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Mentions aspect ratios as a concept; no specific ratio value given.
---
Claim: In Flex mode (partially folded), show content on top and controls on the bottom, with a visual transition into/out of Flex mode.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Show content on the top and provide controls on the bottom." "Show a visual transition effect when changing into or out of Flex mode."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Flex mode = half-opened posture.
---
Claim: Avoid positioning interactive elements near the crease in the middle of a foldable screen.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Avoid positioning interactive elements near the crease in the middle of the screen."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: No numeric crease keep-out zone stated.
---
Claim: Flex mode is triggered when the phone is partially folded (POSTURE_HALF_OPENED) and apps should be redesigned for that posture.
Source URL: https://developer.samsung.com/galaxy-z/flex-mode.html
Source title: Flex mode (Samsung Developer, Galaxy Z)
Evidence type: EXPLICIT
Evidence: "When your phone is partially folded, it will go into Flex Mode." "the app should be redesigned proper layout when POSTURE_HALF_OPENED state."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: Galaxy Z (Flip/Fold) specific; developer/API page (references Jetpack WindowManager). No fold-angle degrees stated.
---

## 10. Multi-window behavior

---
Claim: Large screens support up to 3 split-screen views and 5 pop-up views open simultaneously.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "allowing users to have up to 3 split screen view and 5 pop-up view open simultaneously."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Stated as a platform capability, not tied to a One UI version number.
---
Claim: It is possible to have 3 or more apps on screen simultaneously (vs. the common 2-app side-by-side).
Source URL: https://developer.samsung.com/galaxy-z/multi-window.html
Source title: Multi-Window (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "While having 2 apps open side by side has become common, it is now possible to have 3 or more apps on the screen at the same time."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Developer page (not a design-token page). References Android multi-window docs for mechanics.
---
Claim: Enable drag-and-drop content sharing between visible windows and support multiple app instances for multitasking.
Source URL: https://developer.samsung.com/galaxy-z/multi-window.html
Source title: Multi-Window (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Guidance to implement drag-and-drop between windows and "enabling multiple instances of your app."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Implementation guidance; defers mechanics to Android documentation.
---

## 11. Platform adaptation

(See §8 device-type→window-class mapping and §1 cross-device philosophy.)

---
Claim: Some foldable screens (e.g., a settings list) may not need a layout change when partially folded.
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Some apps or screens may not need to change their layout when the device is partially folded. For example, a list of settings."
Confidence: high
Version-specific: NO
Contains numeric value: NO
Notes: Adaptation is content-dependent, not mandatory for every screen.
---

## 12. Color

---
Claim: One UI relies on rich, solid colors whose brightness and saturation fall within particular ranges so important information stays identifiable and readable.
Source URL: https://developer.samsung.com/one-ui/color/system.html
Source title: Color system and usage (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "One UI relies on rich, solid colors to create a sleek modern look. The brightness and saturation of these colors all fall within particular ranges (below)…"
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: The specific numeric brightness/saturation ranges did not extract as text; not recorded.
---
Claim: One UI's Primary color is #0381fe, used identically in Light and Dark themes (floating action buttons, sliders, input fields, focused items).
Source URL: https://developer.samsung.com/one-ui/color/system.html
Source title: Color system and usage (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: Lists "Primary #0381fe" for both Light and Dark theme; corroborated by the 2019 PDF ("Primary #0381fe" under both themes).
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Web page states no version; the matching PDF is 2019, so this is an early-generation value and may differ in One UI 7.
---
Claim: The "Primary dark" role is #0072de (Light theme) and #3e91ff (Dark theme).
Source URL: https://developer.samsung.com/one-ui/color/system.html
Source title: Color system and usage (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "Primary dark — Light: #0072de, Dark: #3e91ff." Used for contained-button/app-bar/text-button/dialog-button emphasis. Confirmed in PDF.
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Role deliberately uses different hex per theme.
---
Claim: The "Color control activated" role (checkboxes, radios, switches) is #3e91ff in both themes.
Source URL: https://developer.samsung.com/one-ui/color/system.html
Source title: Color system and usage (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "Color control activated — #3e91ff" for both themes (Checkboxes, On/off toggles). PDF labels it "Color control active #3e91ff."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Same hex both themes.
---
Claim: One UI defines White as #fafafa (both themes) and Black as #000000 (Light) but #080808 (Dark).
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: Palette table: "White #fafafa" (both), "Black #000000" (Light), "Black #080808" (Dark).
Confidence: high
Version-specific: YES
Contains numeric value: YES
Notes: 2019 PDF; dark theme uses near-black #080808 rather than pure black. Not restated on the developer color page.
---
Claim: One UI's palette follows Android Material's categorized-palette model (Primary, Primary dark, Color control activated), where changing one category updates all elements in that category.
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "Android's material theme provides a categorized color palette system. By changing the color value of one category, you can change all of the color value of on-screen element that belongs to the same category at once."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: 2019 PDF (One UI on Android). This is Samsung *describing* its use of the Android theme system — NOT a statement that Material Design rules govern One UI. Do not treat Material rules as One UI rules (see collection rule 9).
---

## 13. Dark mode

---
Claim: One UI provides default (Light) themes plus Dark mode and recommends all apps let the user switch to Dark mode at a desired/set time.
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "One UI provides default themes and a dark mode. It's recommended that you provide a dark mode…" and "allow the user to switch to Dark mode at the desired or set time."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: 2019 PDF.
---
Claim: In Dark mode, backgrounds/menus/UI turn black or dark gray to reduce glare, and apps must be tested in both Light and Dark before release.
Source URL: https://developer.samsung.com/one-ui/color/theme.html
Source title: Theme (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: In Dark mode "backgrounds, menus, and other UI elements turn black or dark gray to reduce glare"; "test apps and features in both Light and Dark modes before release."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: No hex/threshold values on this page.
---
Claim: A black background against a black device bezel merges the bezel/screen boundary to make the screen appear more visually expanded (rationale for the near-black dark theme).
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "if you use a black background… when the device's bezel is also black, the boundary between the bezel and screen becomes merged, making the screen appear more visually expanded."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: 2019 PDF.
---

## 14. Typography

---
Claim: The default font used in One UI (per the 2019 guidelines) is Roboto (the Android system font).
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "The default font used in One UI is Roboto. It's recommended that you apply the following font sizes to components. Font family of Roboto."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: CRITICAL — this 2019 One UI *system UI* default is Roboto, NOT SamsungOne. The accompanying font-size table did not extract as text (rendered as an image), so specific sizes are NOT recorded. Samsung devices also ship "Samsung Sans"/"One UI Sans" as system fonts in later releases, but no fetched official page stated that as a rule with sizes.
---
Claim: SamsungOne is Samsung's universal brand typeface — 26 writing systems, 400+ languages, 25,000+ glyphs.
Source URL: https://design.samsung.com/global/contents/samsungone/
Source title: SamsungOne — the new universal typeface for Samsung
Evidence type: EXPLICIT
Evidence: "SamsungOne is a family of scripts covering 26 writing systems, more than 400 languages, and over 25,000 glyphs."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Brand/corporate-identity typeface, distinct from the One UI system UI font. Page states no weights or One UI version.
---
Claim: A standalone phone-One-UI typography page under developer.samsung.com/one-ui/ was not found; type guidance instead lives under Accessibility (layout-and-typo) and Writing. A separate Typography page exists only for One UI Watch/Tizen (Breeze Sans).
Source URL: https://developer.samsung.com/one-ui/iconography/symbol.html
Source title: Symbol (Samsung Developer, One UI Iconography)
Evidence type: OBSERVED
Evidence: The One UI docs nav exposes Iconography, Color, Accessibility (incl. Layout and typography), and Writing — but no standalone "/one-ui/typography/" page. Watch typography (Breeze Sans) lives at developer.samsung.com/one-ui-watch-tizen/visual/typography.html.
Confidence: medium
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: No phone One UI typography URL appeared in the fetched nav; the Watch typography page is a distinct product.
---

## 15. Iconography

---
Claim: One UI app icons have square backgrounds with smooth rounded corners and outlines to feel softer and more inviting.
Source URL: https://developer.samsung.com/one-ui/iconography/background.html
Source title: Background (Samsung Developer, One UI Iconography)
Evidence type: EXPLICIT
Evidence: "One UI app icons have square backgrounds with smooth rounded corners and outlines," which "make the icons seem softer and more inviting."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: No corner-radius value stated.
---
Claim: One UI app icons use bright, vibrant background colors with white symbols; the background↔white-symbol contrast produces the brand identity.
Source URL: https://developer.samsung.com/one-ui/iconography/color.html
Source title: Icon color (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "We use bright, vibrant background colors to project confidence, and the contrast between the colored backgrounds and white symbols produces an intuitive, distinct brand identity."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: No hex codes for the icon palette.
---
Claim: One UI icon gradients should use 3 or fewer analogous colors.
Source URL: https://developer.samsung.com/one-ui/iconography/color.html
Source title: Icon color (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: Gradients "3 or fewer analogous colors to maintain previous app identities."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: "3 or fewer" is a color count, not a size/hex.
---
Claim: One UI icons should use rounded stroke terminals (matching One UI's rounded corners) while stroke corners stay sharp for contrast.
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "use rounded stroke terminals for icons… The stroke corners, however, should remain sharp to add contrast to the rounded corners and details."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: 2019 PDF.
---
Claim: One UI 7 app icons are built on circular forms with soft curved outlines and visual effects (blur, translucency, colored glass, gradients).
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 (Samsung Design)
Evidence type: OBSERVED
Evidence: Icons "maintain the key elements while maximizing functionality," on circular forms with "soft and elegant curved outlines"; effects include blur, translucency, colored glass, gradient ("pale yellow and blue hues").
Confidence: medium
Version-specific: YES
Contains numeric value: NO
Notes: One UI 7 marketing page; NO hex/numbers. Some imagery is AI-generated ("simulated… for illustrative purposes only"), so treat visuals as OBSERVED, not tokens.
---

## 16. Components

---
Claim: The One UI App bar has a standard (condensed) form and an Extended app bar variant, with the title centered when expanded; no more than three action buttons recommended per page.
Source URL: https://developer.samsung.com/one-ui/comp/app-bar.html
Source title: App bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Extended app bar" variant; title "right in the center of the expanded app bar"; "We recommend no more than three buttons on any page." Extended bar condenses on scroll down, expands on scroll up.
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: "three" is a recommendation.
---
Claim: The bottom bar holds a maximum of 5 action buttons, can't display only one, and overflows extras into a More options menu; buttons should include both icon and text.
Source URL: https://developer.samsung.com/one-ui/comp/bottom-bar.html
Source title: Bottom bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "maximum of 5 action buttons"; "can't display only one action button"; overflow → "the four most-used… and the rest should go in a More options menu."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Buttons may hide on downward scroll.
---
Claim: One UI bottom navigation should display fewer than 4 tabs (max 5), uses text-only tabs, and does not support swiping between tabs.
Source URL: https://developer.samsung.com/one-ui/comp/bottom-navigation.html
Source title: Bottom navigation (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Tabs should be in text only"; "has to display less than 4"; "maximum of 5 can be displayed"; "Users can't move between tabs by swiping in One UI."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Source has typos. When a screen has tabs, the top title may be omitted.
---
Claim: One UI buttons come in Flat and Contained types with Low/Medium/High emphasis; only one button style per screen; button corner radius is 18 dp.
Source URL: https://developer.samsung.com/one-ui/comp/button.html
Source title: Buttons (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "only one button style should be used on any given screen"; contained buttons "gray background for moderate emphasis… colored background for a high level of emphasis"; corner radius "18dp" in the drawable/mask XML.
Confidence: medium
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Correct URL is button.html (singular; buttons.html 404s). The 18 dp appears in code snippets, not narrative prose — treat as an implementation spec on the official page. No touch-target size stated.
---
Claim: One UI dialogs are positioned by type — choice/confirmation at the bottom, information dialogs centered — and decision dialogs persist until the user acts.
Source URL: https://developer.samsung.com/one-ui/comp/dialog.html
Source title: Dialog (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Choice/confirmation dialogs "appear at the bottom of the screen"; information dialogs "in the center"; decision dialogs "won't disappear until the user makes a choice, taps the Back button, or taps… outside."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: Bottom placement of choice dialogs reflects reachability; code uses setGravity(Gravity.Bottom).
---
Claim: One UI list main text should be a noun/short phrase within 31 characters, with a toggle switch placed on the right side of the row.
Source URL: https://developer.samsung.com/one-ui/comp/list.html
Source title: Lists (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "keep them within 31 characters to avoid spilling over to a second line"; "a toggle switch should be provided on the right side of that row"; lists ordered by priority.
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Correct URL is list.html (singular).
---
Claim: All One UI search boxes support auto-complete and predictive text and show recent searches/suggestions before the user types.
Source URL: https://developer.samsung.com/one-ui/comp/search.html
Source title: Search (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "All search boxes in One UI support auto-complete and predictive text"; "Before a user even types… we offer a list of recently searched keywords and other suggestions."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: Defers technical details to Android search guidelines.
---
Claim: Toasts should be about one line and never exceed 3 lines in any language, reserved for minor success/failure info (serious issues use a popup).
Source URL: https://developer.samsung.com/one-ui/comp/toast.html
Source title: Toasts (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Toasts should be about one line, and should never exceed 3 lines in any language"; for "relatively minor information"; serious issues "use a popup."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Correct URL is toast.html. No duration value stated ("a certain amount of time").
---

## 17. Navigation

(See §8 for large-screen navigation scaling: navigation bar → navigation rail → drawer by window class. Bottom navigation is in §16.)

---
Claim: One UI 7 changed the notification/quick-settings gesture — swipe the upper-right corner for Quick Settings, swipe elsewhere for the Notification panel.
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 (Samsung Design)
Evidence type: EXPLICIT
Evidence: "swipe the upper right corner for the Quick Settings panel, or swipe anywhere else on the screen for the Notification panel."
Confidence: high
Version-specific: YES
Contains numeric value: NO
Notes: One UI 7 specific; differs from the single combined Quick panel described on the developer structure page (version drift — good example of why to prefer durable principles).
---

## 18. Motion

---
Claim: One UI uses motion to emotionally engage users and clarify cause-and-effect; motions should feel instant and respond naturally to touch, with smooth uninterrupted transitions.
Source URL: https://developer.samsung.com/one-ui/motion/intro.html
Source title: Motion introduction (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "One UI uses motion to emotionally engage users…"; "motions should happen instantly and respond naturally to the user's touch"; transitions "smooth and uninterrupted."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: none
---
Claim: One UI motion duration should be at least 100 ms (minimum recognizable) and never exceed 500 ms.
Source URL: https://developer.samsung.com/one-ui/motion/basic.html
Source title: Motion basics and usage (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "at least 100 ms, which is the minimum recognizable length"; "should never exceed 500 ms to avoid interfering with subsequent tasks."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Explicit numeric bounds stated as rules.
---
Claim: One UI's basic path interpolator (easing) is [0.22, 0.25, 0.00, 1.00] — accelerate quickly, then slow gradually.
Source URL: https://developer.samsung.com/one-ui/motion/basic.html
Source title: Motion basics and usage (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Basic Path Interpolator "[0.22, 0.25, 0.00, 1.00]"; "Basic motions in One UI accelerate quickly then slow down gradually."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: Page also defines Linear/Ease-In/Ease-Out/Ease-In-Out usage and cross-fade rules (new image fades in before old disappears; text waits until fully gone before fading in).
---

## 19. Sound and haptics

---
Claim: One UI sounds should be used only when necessary, give immediate feedback, differentiate general input from cancel/delete, and use a sine waveform for a soft, clean feel.
Source URL: https://developer.samsung.com/one-ui/sound-and-haptic/sound.html
Source title: Sound (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "sounds should only be used when necessary"; "different sounds for general input and cancel/delete actions"; "The sine waveform is used to provide a soft and clean feel."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: No durations/frequencies stated.
---
Claim: One UI haptics are crisp and refined to avoid overstimulation, differentiate special keys (Delete/Spacebar/Function), and synchronize timing with the accompanying visual movement.
Source URL: https://developer.samsung.com/one-ui/sound-and-haptic/haptic.html
Source title: Haptic (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Crisp and refined haptic feedback helps users avoid overstimulation"; "different feedback for special keys such as Delete, Spacebar, and Function keys"; "the movement's timing and nuance match perfectly with the vibration."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: No numeric durations/frequencies/intensities stated.
---

## 20. Writing

---
Claim: One UI writing keeps every bit of text purposeful — text that doesn't help the user choose, act, or understand is left out; give an action instead of a dead end.
Source URL: https://developer.samsung.com/one-ui/writing/focused-and-purposeful.html
Source title: Focused and purposeful (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "every bit of text helps users make a choice, take an action, or understand what's happening. If text isn't meeting one of these goals, we leave it out."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: none
---
Claim: One UI writing is simple and human — interrupt with popups only for important cases and use inclusive, gender-neutral language (singular "they").
Source URL: https://developer.samsung.com/one-ui/writing/simple-and-human.html
Source title: Simple and human (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Limit popups to "data input, deletion confirmation, personal info consent, or critical information"; use singular "they" — "we always avoid constructions like 'he/she.'"
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: none
---
Claim: One UI writing is empowering — phrase prompts as questions (limit to one), tell users the solution to a problem, and avoid blaming the user.
Source URL: https://developer.samsung.com/one-ui/writing/empowering.html
Source title: Empowering and engaging (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Use rhetorical questions but "limit it to one"; "If there's a solution to a problem, we tell users what it is"; prefer "Remove filter to take burst shots" over a blame framing.
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: The only number is "limit it to one."
---

## 21. Accessibility

---
Claim: One UI accessibility is guided by four principles (4C): Consideration, Comprehensiveness, Coherence, Co-creation.
Source URL: https://developer.samsung.com/one-ui/accessibility/intro.html
Source title: Accessibility introduction (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Consideration… Comprehensiveness… Coherence: Make every device accessible… Co-creation: Collaborate with our users."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: none
---
Claim: One UI requires small text ≥ 4.5:1 contrast and large text (normal ≥ 18 dp, bold ≥ 14 dp) ≥ 3:1.
Source URL: https://developer.samsung.com/one-ui/accessibility/color-contrast.html
Source title: Color and contrast (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "small text should have at least a 4.5:1 contrast"; "For large text (more than 18 dp for normal text or 14 dp for bold text), the contrast should be at least 3:1."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: WCAG-derived (the PDF cites WCAG) but stated on Samsung's official page.
---
Claim: The 2019 PDF's contrast table sets minimum ratios by dp size: ~12–13 dp = 4.5:1 (regular & bold); 14 & 17 dp = 4.5:1 regular / 3:1 bold; 18 dp and 19 dp+ = 3:1 both.
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: Table rows "~12 4.5:1/4.5:1", "13 4.5:1/4.5:1", "14 4.5:1/3:1", "17 4.5:1/3:1", "18 3:1/3:1", "19~ 3:1/3:1" (Regular/Bold).
Confidence: high
Version-specific: YES
Contains numeric value: YES
Notes: 2019 PDF; the per-size basis for the 18 dp normal / 14 dp bold "large text" cutoff.
---
Claim: One UI requires text (except subtitles and text within images) to be resizable up to 200% without loss of content or functionality; touch areas large with enough spacing.
Source URL: https://developer.samsung.com/one-ui/accessibility/layout-and-typo.html
Source title: Layout and typography (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "All text except subtitles and text within images should be resizable up to 200%…"; "Touch areas should be large enough to be touched easily and have enough spacing… to prevent missed touches."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: 200% is the only explicit number; NO touch-target dp size is stated (do not invent 48dp).
---
Claim: One UI requires controls to stop auto-playing content lasting more than 5 seconds, alternatives to complex gestures, and consistent control locations.
Source URL: https://developer.samsung.com/one-ui/accessibility/interaction-and-control.html
Source title: Interaction and control (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "give users controls to stop content lasting more than 5 seconds"; "Provide alternative ways of performing complex actions such as drag and drop or multifinger gestures"; consistent control locations.
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: YES
Notes: 5 seconds is the only explicit number.
---
Claim: One UI focus order flows logically, shows a focus mark when accessibility is active, excludes decorative elements, and does not support looping.
Source URL: https://developer.samsung.com/one-ui/accessibility/focus-order.html
Source title: Focus order (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "a focus mark should be shown"; "the focus flows logically"; "Looping is not supported"; "No need to focus on decorative elements…"
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: Related elements can be grouped as one focus element.
---
Claim: One UI content must not identify controls by shape/color/location alone, must supplement audio with text/visual feedback, and must avoid strobing / rapid brightness changes.
Source URL: https://developer.samsung.com/one-ui/accessibility/content.html
Source title: Content (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "'Tap Start' is effective, but 'Tap the square button below' is not"; provide visual for audio cues; "Avoid strobing effects, sudden and rapid changes in brightness."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: Provide subtitles/scripts/sign language where possible.
---
Claim: One UI color-and-contrast guidance states color alone must not convey information; provide additional visual marks (test by switching UI to grayscale).
Source URL: https://developer.samsung.com/one-ui/accessibility/color-contrast.html
Source title: Color and contrast (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Color alone is insufficient — "Provide additional marks as well"; "switch your UI to grayscale to check whether information is being conveyed clearly without color."
Confidence: high
Version-specific: UNKNOWN
Contains numeric value: NO
Notes: References the third-party Colour Contrast Analyser as an external aid (the tool is not a Samsung source).
---

---

## Source index (all URLs fetched)

**developer.samsung.com — One UI docs (phone/tablet):**
- /one-ui/index.html — Overview & 4 principles
- /one-ui/structure/basic.html — Basic structure
- /one-ui/structure/visual-depth.html — Visual depth (blur/dim/shadow)
- /one-ui/layout/basic.html — Viewing vs interaction area
- /one-ui/layout/grid.html — Grid, 24 dp margins, Reject/Grip zones, camera cutout
- /one-ui/color/system.html — Color roles + hex (#0381fe, #0072de, #3e91ff)
- /one-ui/color/theme.html — Dark mode
- /one-ui/iconography/background.html — Icon background shape
- /one-ui/iconography/symbol.html — Icon symbol
- /one-ui/iconography/color.html — Icon color, 3-or-fewer gradient
- /one-ui/comp/app-bar.html — App bar
- /one-ui/comp/bottom-bar.html — Bottom bar (max 5)
- /one-ui/comp/bottom-navigation.html — Bottom navigation (<4, max 5)
- /one-ui/comp/button.html — Buttons, 18 dp radius (NOTE: buttons.html 404s)
- /one-ui/comp/dialog.html — Dialog placement
- /one-ui/comp/list.html — Lists, 31 chars (NOTE: lists.html → list.html)
- /one-ui/comp/search.html — Search
- /one-ui/comp/toast.html — Toasts, ≤3 lines (NOTE: toasts.html → toast.html)
- /one-ui/motion/intro.html — Motion intro
- /one-ui/motion/basic.html — Motion 100–500 ms, interpolator [0.22,0.25,0,1]
- /one-ui/sound-and-haptic/sound.html — Sound
- /one-ui/sound-and-haptic/haptic.html — Haptic
- /one-ui/writing/focused-and-purposeful.html — Writing
- /one-ui/writing/simple-and-human.html — Writing
- /one-ui/writing/empowering.html — Writing
- /one-ui/accessibility/intro.html — 4C
- /one-ui/accessibility/color-contrast.html — 4.5:1 / 3:1
- /one-ui/accessibility/layout-and-typo.html — 200% resize
- /one-ui/accessibility/interaction-and-control.html — 5 s auto-play
- /one-ui/accessibility/focus-order.html — Focus order
- /one-ui/accessibility/content.html — Content
- /one-ui/largescreen-and-foldable/intro.html — Large-screen ratios (42/58, 38/62, 50:50), 3 split / 5 pop-up
- /one-ui/largescreen-and-foldable/large_screen_layout.html — 600 dp threshold, window classes 600/840
- /one-ui/largescreen-and-foldable/designing_for_foldable.html — Foldable continuity, Flex mode, crease
- /one-ui-watch-tizen/principle.html — Watch principles (NOT phone; disambiguation only)

**developer.samsung.com — Galaxy Z (developer/API, not design tokens):**
- /galaxy-z/multi-window.html — 2 → 3+ apps, drag-and-drop, multi-instance
- /galaxy-z/flex-mode.html — POSTURE_HALF_OPENED

**design.samsung.com:**
- /global/contents/one-ui/ — Design-portal philosophy + 4 differently-named principles + Focus Block
- /global/contents/one-ui-7/index.html — One UI 7 visual language (no numbers; AI-generated imagery)
- /global/contents/samsungone/ — SamsungOne brand typeface
- /global/contents/one-ui/download/oneui_design_guide_eng.pdf — **2019 One UI Design Guidelines PDF** (source of most hex/dp values; One UI 2 / Android 10 era)

**404 / redirected (recorded so they aren't re-tried as evidence):**
- /one-ui/foldable/unfolded.html — 404
- /one-ui/comp/buttons.html, /lists.html, /toasts.html — 404 (use singular forms)
- /one-ui/foldable-and-largescreen/intro.html — resolves to the large-screen intro content
