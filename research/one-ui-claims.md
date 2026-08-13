# Samsung One UI — Claim Registry

> Atomic claim registry derived from [`research/one-ui-sources.md`](./one-ui-sources.md).
> Each entry is ONE independently verifiable assertion with a stable `OUI-NNN` ID.
> Compound source findings were split into multiple IDs. Every claim traces to a
> publicly accessible official Samsung source. No third-party, internal, leaked, or
> unreleased material. Numeric values recorded only where an official page states them.

**Categories:** principle · layout · color · typography · iconography · component · interaction · navigation · motion · accessibility · large-screen · foldable · writing · sound-haptic · dark-mode · other

**Cross-cutting caveats (see one-ui-sources.md):** (1) three different official principle sets exist (developer portal / design portal / watch-Tizen); (2) most hex/dp values come from the **Oct-2019 One UI Design Guidelines PDF** (One UI 2 era) and are flagged `Version-specific: YES`; (3) One UI's 2019 system font is **Roboto**, distinct from the **SamsungOne** brand typeface; (4) no official touch-target dp size was found.

---

## OUI-001

Claim: One UI's overarching goal is to create joyful, comfortable experiences across any Samsung device (phone, tablet, watch, earbud, PC).
Category: principle
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "joyful and comfortable experiences on any device, whether it's a phone, tablet, watch, earbud, or PC."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Cross-device philosophy statement.

## OUI-002

Claim: One UI is designed to connect various devices together to provide a seamless experience.
Category: principle
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: "designed with the purpose of connecting various devices together to provide a seamless experience."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Design-portal statement (distinct from the developer-portal one).

## OUI-003

Claim: One UI's simplicity is intended to make it easy to use.
Category: principle
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: "its simplicity makes it easy to use."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Split from the same sentence as OUI-002.

## OUI-004

Claim: One UI 7 uses the circle — a highly scalable shape — to produce soft, curved outlines as a visual element across the screen.
Category: other
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 — Samsung Design
Evidence type: EXPLICIT
Evidence: "Utilizing a circle, a simple shape with high scalability, soft and elegant curved outlines appear as a visual element across the screen."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: One UI 7 visual language; no numbers.

## OUI-005

Claim: One UI 7 aims for a visually seamless, balanced design that clarifies the hierarchy of information across components and content.
Category: other
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 — Samsung Design
Evidence type: EXPLICIT
Evidence: "a visually seamless, balanced design" clarifying "the hierarchy of information across components and contents."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: One UI 7 marketing/design-portal framing.

## OUI-006

Claim: The developer portal defines four One UI principles: Focus on the task at hand; Interact naturally; Be visibly comfortable; Make things responsive.
Category: principle
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Lists the four named principles.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Differs from the design-portal set (OUI-016).

## OUI-007

Claim: The "Focus on the task at hand" principle uses simple, intuitive design to keep users focused on content.
Category: principle
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "One UI uses simple, intuitive designs to help users focus on content."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-008

Claim: The "Focus on the task at hand" principle makes user journeys as short and smooth as possible.
Category: principle
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "makes user journeys as short and smooth as possible."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Split from OUI-007.

## OUI-009

Claim: Under "Interact naturally," One UI divides the screen into a viewing area at the top and an interaction area at the bottom.
Category: layout
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Describes a viewing area at top and interaction area at bottom.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Corroborated by layout/basic.html (OUI-031).

## OUI-010

Claim: One UI places interactive elements within easy reach even on large devices.
Category: interaction
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "places interactive elements within easy reach, even on large devices."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Core reachability rationale.

## OUI-011

Claim: The "Be visibly comfortable" principle cites Dark mode to reduce eye fatigue and glare.
Category: dark-mode
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Cites Dark mode to reduce eye fatigue/glare.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-012

Claim: The "Be visibly comfortable" principle cites a high-contrast keyboard as an accessibility affordance.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Cites a high-contrast keyboard.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-013

Claim: The "Be visibly comfortable" principle cites variable font sizes and styles to make text accessible.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Variable font sizes and styles to make text accessible to anyone."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-014

Claim: The "Make things responsive" principle means the One UI layout adapts so it is easy to use on any device or screen size.
Category: principle
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The layout of One UI adapts so it's easy to use on any device or screen size."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-015

Claim: Under "Make things responsive," interface elements remain within reach across screen sizes.
Category: interaction
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Elements described as remaining within reach across screen sizes.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Split from OUI-014.

## OUI-016

Claim: The design portal states four differently-named One UI principles: One Makes It Natural; One Is Clean and Easy; One Keeps Consistency; One Attracts All Senses.
Category: principle
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: Names the four principles.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Distinct from the developer-portal set; may reflect earlier branding.

## OUI-017

Claim: "One Makes It Natural" emphasizes single-handed operation.
Category: interaction
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: Emphasizes single-handed operation.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-018

Claim: "One Makes It Natural" keeps areas for viewing and touching clearly distinguished.
Category: layout
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: "with areas for viewing and touching clearly distinguished."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Second-source corroboration of the viewing/interaction split.

## OUI-019

Claim: "One Is Clean and Easy" focuses on the essence to give a clean, concise first impression.
Category: principle
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: "focuses on the essence, which gives a clean and concise first impression."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-020

Claim: "One Is Clean and Easy" removes unnecessary elements to guide users to important functions.
Category: principle
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: Unnecessary elements removed to guide users toward important functions.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Split from OUI-019.

## OUI-021

Claim: "One Keeps Consistency" unifies smart-device experiences into one uniform experience.
Category: principle
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: "brings all these smart device experiences together into a uniform, one experience."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-022

Claim: "One Keeps Consistency" standardizes appearance using elements such as rounded corners.
Category: other
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: Standardizes appearance with elements like rounded corners.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: No numeric corner radius stated.

## OUI-023

Claim: One UI Watch (Tizen) uses a separate principle set — Scannable, Easy to Follow, Responsive, Desirable.
Category: principle
Source URL: https://developer.samsung.com/one-ui-watch-tizen/principle.html
Source title: One UI Watch (Tizen) — Design principles (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Lists the four watch principles.
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: WATCH/TIZEN ONLY — does not apply to phone One UI.

## OUI-024

Claim: One UI's basic structure comprises the Lock screen, Home screen, Recents screen, Quick panel, and Edge panel.
Category: other
Source URL: https://developer.samsung.com/one-ui/structure/basic.html
Source title: One UI — Basic structure (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Describes these five system surfaces.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Structural inventory of system screens.

## OUI-025

Claim: One UI uses blur, dim, and shadow effects to create a hierarchical structure that helps users focus on important information.
Category: other
Source URL: https://developer.samsung.com/one-ui/structure/visual-depth.html
Source title: One UI — Visual depth (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "uses blur, dim, and shadow effects to create a hierarchical structure."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: No numeric opacity/blur/shadow values.

## OUI-026

Claim: The dim effect and shadow effect must not be applied at the same time.
Category: other
Source URL: https://developer.samsung.com/one-ui/structure/visual-depth.html
Source title: One UI — Visual depth (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Avoid applying the dim effect and shadow effect at the same time."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-027

Claim: The dim effect should be applied evenly, avoiding exposing multiple hierarchy levels on a single screen.
Category: other
Source URL: https://developer.samsung.com/one-ui/structure/visual-depth.html
Source title: One UI — Visual depth (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Apply dim evenly; caution against multiple hierarchical levels on one screen.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-028

Claim: A soft shadow effect is used to show connections between related information while maintaining hierarchy.
Category: other
Source URL: https://developer.samsung.com/one-ui/structure/visual-depth.html
Source title: One UI — Visual depth (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "A soft shadow effect can be used to show connections between information while maintaining the hierarchy."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Shadow only for closely related screens.

## OUI-029

Claim: One UI 7 uses a layered blur effect combined with "colored glass" overlays to create depth and texture.
Category: other
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 — Samsung Design
Evidence type: EXPLICIT
Evidence: A "blur effect" that "creates a sense of depth and delicate texture" combined with "colored glass" overlays.
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: One UI 7 specific.

## OUI-030

Claim: One UI 7 applies colorful gradient backgrounds to certain full-screen apps (e.g. Clock, Calendar, Reminder).
Category: other
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 — Samsung Design
Evidence type: EXPLICIT
Evidence: Colorful gradients on startup screens and full-background interfaces (Clock, Calendar, Reminder).
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: One UI 7 specific.

## OUI-031

Claim: In One UI layout, the top of the screen is the viewing area where titles appear.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The top part of the screen is the viewing area where titles appear."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-032

Claim: The viewing area uses wide margins to give the impression of open space.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "wide margins to give the user the impression of open space."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Qualitative; dp value is on the grid page (OUI-038).

## OUI-033

Claim: Components that require touch interaction are avoided in the viewing area.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Components that require touch interaction are avoided here."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-034

Claim: The viewing area uses center-aligned text for greater visual stability.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Uses center-aligned text for "greater visual stability."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-035

Claim: In the interaction area, actionable components are grouped and placed in a logical order.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Actionable components are grouped and placed in a logical order."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-036

Claim: One UI interaction-area layouts support list, card, 2-column, and 3-column arrangements.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Supports list, card, 2-column, and 3-column layouts.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Column counts are layout-type names, not measurements.

## OUI-037

Claim: One UI supports focus blocks in card, list, and image formats.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/basic.html
Source title: One UI — Basic layout (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Focus blocks in card, list, and image formats.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-038

Claim: One UI recommends interactive components be placed with margins of at least 24 dp on both left and right sides.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "place interactive components with margins of at least 24 dp on both the left and right sides."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Restated in the 2019 PDF; avoids conflicts with curved edges/corners.

## OUI-039

Claim: One UI's Reject zone blocks accidental touches in the interaction area.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The Reject zone blocks touches in the interaction area."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Zone size not stated numerically.

## OUI-040

Claim: One UI's Grip zone blocks palm and three-finger touches that occur while holding the phone.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The Grip zone blocks palm touches and three-finger touches that may occur when the user is holding their phone."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Zone size not stated numerically.

## OUI-041

Claim: On-screen items should be optimized to avoid the camera cutout, with distinct guidance for 90° and 270° orientations.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Items "should be optimized to avoid the camera cutout," addressing 90° and 270° orientations.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Orientations, not measurements.

## OUI-042

Claim: One UI recommends thumbnail/focus-block corner radii of 26 dp, 20 dp, or 12 dp depending on the screen grid and target.
Category: layout
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "Radius=26dp", "Radius=20dp", "Radius=12dp" under the Thumbnail radius section.
Contains numeric value: YES
Version-specific: YES
Confidence: high
Notes: 2019 PDF (One UI 2 era); may differ in One UI 7.

## OUI-043

Claim: One UI places interactive elements toward the bottom so they remain within thumb reach even on large devices.
Category: interaction
Source URL: https://developer.samsung.com/one-ui/index.html
Source title: One UI — Overview (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Interaction area at the bottom "places interactive elements within easy reach, even on large devices."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Reachability rationale (relates to OUI-010).

## OUI-044

Claim: On large screens, pop-ups should appear near the UI element the user interacted with to reduce finger-travel distance.
Category: interaction
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "make the pop-up appear near the button or other UI element that the user interacted with… reduces finger travel distance."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Large-screen reachability rule.

## OUI-045

Claim: "Keep things reachable" is one of One UI's four stated large-screen layout principles.
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Section headings include "Show menus together with content", "Adjust grids for large screens", "Avoid switching context", "Keep things reachable."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-046

Claim: One UI is designed to give the best experience across all display sizes, resolutions, and screen ratios, including phones, tablets, foldables, DeX monitors, and split-screen.
Category: layout
Source URL: https://developer.samsung.com/one-ui/layout/grid.html
Source title: One UI — Grid system (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "the best experience for all display sizes, resolutions, and screen ratios," across those form factors.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-047

Claim: One UI's "Focus Block" clears content for single-glance viewing.
Category: layout
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: A "Focus Block" that "clears content for single-glance viewing."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Concept also appears in developer layout docs.

## OUI-048

Claim: One UI keeps an upward-swipe interaction constant across all screens.
Category: interaction
Source URL: https://design.samsung.com/global/contents/one-ui/
Source title: One UI — Samsung Design (design.samsung.com)
Evidence type: EXPLICIT
Evidence: An upward swipe that "remains constant across all screens."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-049

Claim: One UI directs developers to use a large-screen layout for any screen 600 dp wide or more.
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Use a large screen layout for screens with a width of 600dp or more."
Contains numeric value: YES
Version-specific: NO
Confidence: high
Notes: Fundamental large-screen threshold.

## OUI-050

Claim: One UI defines three window size classes by width — Compact (< 600 dp), Medium (600 ≤ width < 840 dp), Expanded (840 dp ≤ width).
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Compact "(Width < 600)"; Medium "(600 ≤ Width < 840)"; Expanded "(840 ≤ Width)".
Contains numeric value: YES
Version-specific: NO
Confidence: high
Notes: 600/840 dp classes — distinct from the 600/960 dp ratio system.

## OUI-051

Claim: One UI maps the Compact window class to a phone in portrait.
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Compact = "Phone in portrait."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-052

Claim: One UI maps the Medium window class to Z Fold devices (portrait/landscape) and small tablets in portrait.
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Medium = "Z Fold devices in portrait / landscape; Small tablet in portrait."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Device examples tied to specific form factors.

## OUI-053

Claim: One UI maps the Expanded window class to tablets in portrait and landscape.
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
Source title: Layout design for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Expanded = "Tablet in portrait / landscape."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-054

Claim: For a width of 600 ≤ width < 960 dp, One UI recommends a two-pane split of 42% (first pane) / 58% (second pane).
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "600 ≤ Width < 960" → "42%" / "58%".
Contains numeric value: YES
Version-specific: NO
Confidence: high
Notes: Ratio table uses a 960 dp breakpoint.

## OUI-055

Claim: For a width of 960 dp or more, One UI recommends a two-pane split of 38% (first pane) / 62% (second pane).
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "960 ≤ Width" → "38%" / "62%".
Contains numeric value: YES
Version-specific: NO
Confidence: high
Notes: none

## OUI-056

Claim: One UI advises against stretched-out apps on large screens and recommends multi-pane layouts to show more information at once.
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Stretched-out apps are harder to read and waste the extra space… Use a multi-pane layout."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-057

Claim: For the Compact window class, One UI recommends a navigation bar and a modal navigation drawer.
Category: navigation
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Compact → "Navigation bar, modal navigation drawer."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-058

Claim: For the Medium window class, One UI recommends a navigation rail and a modal navigation drawer.
Category: navigation
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Medium → "Navigation rail, modal navigation drawer."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-059

Claim: For the Expanded window class, One UI recommends a navigation rail with a modal or standard navigation drawer.
Category: navigation
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Expanded → "Navigation rail, modal or standard navigation drawer."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-060

Claim: For foldables specifically, One UI recommends a 50% / 50% two-pane split.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Foldable only" row → "50%" for both panes.
Contains numeric value: YES
Version-specific: YES
Confidence: high
Notes: Design recommendation (Z Fold class), not a hardware split.

## OUI-061

Claim: For app continuity across screen switches, a foldable app should fill the entire screen.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "your app should fill the entire screen."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-062

Claim: For app continuity, a foldable app should keep the scroll position the same when switching screens.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "keep the scroll position the same when switching to a different screen."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-063

Claim: For app continuity, text input and keyboard state should remain when switching screens.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "the text input and keyboard should remain when switching to a different screen."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-064

Claim: A foldable app should display correctly on screens with various sizes, widths, and aspect ratios.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "displays correctly on screens with various sizes, widths, and aspect ratios."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: No specific ratio value stated.

## OUI-065

Claim: A foldable app should support landscape orientation.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "supports landscape orientation."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-066

Claim: A foldable app should display correctly on both the cover screen and the main screen.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "displays correctly on both the cover screen and main screen."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-067

Claim: A foldable app should fill the entire screen without letterboxing.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "fills the entire screen without letterboxing."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-068

Claim: In Flex mode, One UI's basic rule is to show content on the top and provide controls on the bottom.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Show content on the top and provide controls on the bottom."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Flex mode = half-opened posture.

## OUI-069

Claim: One UI advises showing a visual transition effect when changing into or out of Flex mode.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Show a visual transition effect when changing into or out of Flex mode."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: none

## OUI-070

Claim: One UI advises avoiding interactive elements near the crease in the middle of a foldable screen.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Avoid positioning interactive elements near the crease in the middle of the screen."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: No numeric keep-out zone stated.

## OUI-071

Claim: Flex mode is entered when a Galaxy Z phone is partially folded (POSTURE_HALF_OPENED), and apps should redesign their layout for that posture.
Category: foldable
Source URL: https://developer.samsung.com/galaxy-z/flex-mode.html
Source title: Flex mode (Samsung Developer, Galaxy Z)
Evidence type: EXPLICIT
Evidence: "When your phone is partially folded, it will go into Flex Mode." / "redesigned proper layout when POSTURE_HALF_OPENED state."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: Galaxy Z developer/API page; no fold-angle degrees stated.

## OUI-072

Claim: Some foldable screens (e.g. a list of settings) may not need a layout change when the device is partially folded.
Category: foldable
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
Source title: Designing for foldables (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Some apps or screens may not need to change their layout when the device is partially folded. For example, a list of settings."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Adaptation is content-dependent.

## OUI-073

Claim: One UI large screens support up to 3 split-screen views and 5 pop-up views open simultaneously.
Category: large-screen
Source URL: https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
Source title: Designing for large screens (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "up to 3 split screen view and 5 pop-up view open simultaneously."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Stated as a platform capability.

## OUI-074

Claim: On Galaxy Z / large screens it is possible to have 3 or more apps on screen at the same time (beyond the common 2-app side-by-side).
Category: large-screen
Source URL: https://developer.samsung.com/galaxy-z/multi-window.html
Source title: Multi-Window (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "it is now possible to have 3 or more apps on the screen at the same time."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Developer page, not a design-token page.

## OUI-075

Claim: One UI recommends enabling drag-and-drop content sharing between visible windows.
Category: interaction
Source URL: https://developer.samsung.com/galaxy-z/multi-window.html
Source title: Multi-Window (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Guidance to implement drag-and-drop between windows.
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Implementation guidance.

## OUI-076

Claim: One UI recommends supporting multiple instances of an app for multitasking.
Category: other
Source URL: https://developer.samsung.com/galaxy-z/multi-window.html
Source title: Multi-Window (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "enabling multiple instances of your app."
Contains numeric value: NO
Version-specific: NO
Confidence: high
Notes: Defers mechanics to Android docs.

## OUI-077

Claim: One UI relies on rich, solid colors whose brightness and saturation fall within particular ranges to keep important information identifiable and readable.
Category: color
Source URL: https://developer.samsung.com/one-ui/color/system.html
Source title: Color system and usage (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "relies on rich, solid colors… brightness and saturation… all fall within particular ranges."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: The specific numeric ranges did not extract as text; not recorded.

## OUI-078

Claim: One UI's Primary color is #0381fe, used identically in both Light and Dark themes.
Category: color
Source URL: https://developer.samsung.com/one-ui/color/system.html
Source title: Color system and usage (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "Primary #0381fe" for both Light and Dark theme.
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Corroborated by the 2019 PDF; likely an early-generation value that may differ in One UI 7.

## OUI-079

Claim: One UI's "Primary dark" role is #0072de in the Light theme and #3e91ff in the Dark theme.
Category: color
Source URL: https://developer.samsung.com/one-ui/color/system.html
Source title: Color system and usage (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "Primary dark — Light: #0072de, Dark: #3e91ff."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Different hex per theme; confirmed in PDF.

## OUI-080

Claim: One UI's "Color control activated" role (checkboxes, radios, switches) is #3e91ff in both themes.
Category: color
Source URL: https://developer.samsung.com/one-ui/color/system.html
Source title: Color system and usage (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "Color control activated — #3e91ff" for both themes.
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: PDF labels it "Color control active."

## OUI-081

Claim: One UI defines White as #fafafa in both themes.
Category: color
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "White #fafafa" for Light and Dark.
Contains numeric value: YES
Version-specific: YES
Confidence: high
Notes: 2019 PDF.

## OUI-082

Claim: One UI defines Black as #000000 in the Light theme.
Category: color
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "Black #000000" (Light theme).
Contains numeric value: YES
Version-specific: YES
Confidence: high
Notes: 2019 PDF.

## OUI-083

Claim: One UI defines Black as #080808 in the Dark theme.
Category: color
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "Black #080808" (Dark theme).
Contains numeric value: YES
Version-specific: YES
Confidence: high
Notes: 2019 PDF; near-black rather than pure black.

## OUI-084

Claim: One UI's palette uses Android's Material categorized-palette model, where changing one category's value updates all elements in that category.
Category: color
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "Android's material theme provides a categorized color palette system. By changing the color value of one category, you can change all of the color value… at once."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: Samsung describing its use of the Android theme system — NOT a statement that Material rules govern One UI.

## OUI-085

Claim: One UI provides default (Light) themes plus a Dark mode and recommends all apps allow switching to Dark mode at a desired/set time.
Category: dark-mode
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "provides default themes and a dark mode… recommended that you provide a dark mode… switch to Dark mode at the desired or set time."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: 2019 PDF.

## OUI-086

Claim: In Dark mode, backgrounds, menus, and other UI elements turn black or dark gray to reduce glare.
Category: dark-mode
Source URL: https://developer.samsung.com/one-ui/color/theme.html
Source title: Theme (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: In Dark mode "backgrounds, menus, and other UI elements turn black or dark gray to reduce glare."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: No hex values on this page.

## OUI-087

Claim: One UI requires apps and features to be tested in both Light and Dark modes before release.
Category: dark-mode
Source URL: https://developer.samsung.com/one-ui/color/theme.html
Source title: Theme (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "test apps and features in both Light and Dark modes before release."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-088

Claim: One UI notes that a black background against a black device bezel merges the bezel/screen boundary, making the screen appear more visually expanded.
Category: dark-mode
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "the boundary between the bezel and screen becomes merged, making the screen appear more visually expanded."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: 2019 PDF; rationale for the near-black dark theme.

## OUI-089

Claim: The default font used in One UI (per the 2019 guidelines) is Roboto.
Category: typography
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "The default font used in One UI is Roboto."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: CRITICAL — Roboto (Android system font), NOT SamsungOne. Font-size table did not extract; sizes not recorded.

## OUI-090

Claim: SamsungOne is Samsung's universal brand typeface covering 26 writing systems, 400+ languages, and 25,000+ glyphs.
Category: typography
Source URL: https://design.samsung.com/global/contents/samsungone/
Source title: SamsungOne — the new universal typeface for Samsung
Evidence type: EXPLICIT
Evidence: "a family of scripts covering 26 writing systems, more than 400 languages, and over 25,000 glyphs."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Brand/corporate-identity typeface, distinct from the One UI system UI font (do not conflate with OUI-089).

## OUI-091

Claim: No standalone phone-One-UI typography page exists on developer.samsung.com/one-ui; type guidance lives under Accessibility and Writing (a dedicated Typography page exists only for One UI Watch/Tizen, using Breeze Sans).
Category: typography
Source URL: https://developer.samsung.com/one-ui/iconography/symbol.html
Source title: Symbol (Samsung Developer, One UI Iconography)
Evidence type: OBSERVED
Evidence: The One UI docs nav exposes Iconography, Color, Accessibility (incl. Layout and typography), and Writing — but no "/one-ui/typography/" page.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: medium
Notes: Inference from site navigation; the Watch typography page is a distinct product.

## OUI-092

Claim: One UI app icons have square backgrounds with smooth rounded corners and outlines.
Category: iconography
Source URL: https://developer.samsung.com/one-ui/iconography/background.html
Source title: Background (Samsung Developer, One UI Iconography)
Evidence type: EXPLICIT
Evidence: "One UI app icons have square backgrounds with smooth rounded corners and outlines."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: No corner-radius value stated.

## OUI-093

Claim: One UI app icons use bright, vibrant background colors with white symbols, whose contrast produces the brand identity.
Category: iconography
Source URL: https://developer.samsung.com/one-ui/iconography/color.html
Source title: Icon color (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: "bright, vibrant background colors… the contrast between the colored backgrounds and white symbols produces an intuitive, distinct brand identity."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: No hex codes given.

## OUI-094

Claim: One UI icon gradients should use 3 or fewer analogous colors.
Category: iconography
Source URL: https://developer.samsung.com/one-ui/iconography/color.html
Source title: Icon color (Samsung Developer, One UI)
Evidence type: EXPLICIT
Evidence: Gradients "3 or fewer analogous colors."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: A color count.

## OUI-095

Claim: One UI icons should use rounded stroke terminals while keeping stroke corners sharp for contrast.
Category: iconography
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: "use rounded stroke terminals… The stroke corners, however, should remain sharp."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: 2019 PDF.

## OUI-096

Claim: One UI 7 app icons are built on circular forms with soft curved outlines and visual effects (blur, translucency, colored glass, gradient).
Category: iconography
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 (Samsung Design)
Evidence type: OBSERVED
Evidence: Circular forms with "soft and elegant curved outlines"; effects include blur, translucency, colored glass, gradient.
Contains numeric value: NO
Version-specific: YES
Confidence: medium
Notes: One UI 7 marketing page; some imagery AI-generated ("simulated… for illustrative purposes only"). No numbers.

## OUI-097

Claim: The One UI App bar has a standard form and an Extended app bar variant, with the title centered in the expanded state.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/app-bar.html
Source title: App bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Extended app bar" variant; title "right in the center of the expanded app bar."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-098

Claim: One UI recommends no more than three action buttons on any page in the app bar.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/app-bar.html
Source title: App bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "We recommend no more than three buttons on any page."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Recommendation, not a hard limit.

## OUI-099

Claim: The One UI extended app bar condenses to standard height on scroll down and expands on scroll up.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/app-bar.html
Source title: App bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Extended bar condenses on scroll down, expands on scroll up.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-100

Claim: The One UI bottom bar can hold a maximum of 5 action buttons.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/bottom-bar.html
Source title: Bottom bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "maximum of 5 action buttons."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-101

Claim: The One UI bottom bar cannot display only one action button.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/bottom-bar.html
Source title: Bottom bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The bottom toolbar can't display only one action button."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-102

Claim: When the bottom bar overflows, the four most-used buttons are shown and the rest go into a More options menu on the far right.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/bottom-bar.html
Source title: Bottom bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "the four most-used action buttons can be displayed and the rest should go in a More options menu."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-103

Claim: One UI bottom-bar buttons should include both icons and text.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/bottom-bar.html
Source title: Bottom bar (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Buttons "should include both icons and text."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-104

Claim: One UI bottom navigation should display fewer than 4 tabs, up to a maximum of 5.
Category: navigation
Source URL: https://developer.samsung.com/one-ui/comp/bottom-navigation.html
Source title: Bottom navigation (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "has to display less than 4"; "maximum of 5 can be displayed."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Source has typos.

## OUI-105

Claim: One UI bottom-navigation tabs should be text only.
Category: navigation
Source URL: https://developer.samsung.com/one-ui/comp/bottom-navigation.html
Source title: Bottom navigation (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Tabs should be in text only."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-106

Claim: One UI does not let users move between bottom-navigation tabs by swiping.
Category: navigation
Source URL: https://developer.samsung.com/one-ui/comp/bottom-navigation.html
Source title: Bottom navigation (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Users can't move between tabs by swiping in One UI."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-107

Claim: One UI buttons come in Flat and Contained types, each with Low, Medium, and High emphasis levels.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/button.html
Source title: Buttons (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Flat and Contained types with Low/Medium/High emphasis.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Correct URL is button.html (singular).

## OUI-108

Claim: Only one button style should be used on any given One UI screen.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/button.html
Source title: Buttons (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "only one button style should be used on any given screen."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-109

Claim: For contained buttons, a gray background indicates moderate emphasis and a colored background indicates high emphasis.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/button.html
Source title: Buttons (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "gray background for moderate emphasis, and… a colored background for a high level of emphasis."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-110

Claim: One UI buttons use a corner radius of 18 dp.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/button.html
Source title: Buttons (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Corner radius "18dp" in the button mask/background drawable XML.
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: medium
Notes: Appears in a code snippet, not narrative prose.

## OUI-111

Claim: One UI choice/confirmation dialogs appear at the bottom of the screen.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/dialog.html
Source title: Dialog (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Choice/confirmation dialogs "appear at the bottom of the screen."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Reflects reachability (setGravity(Gravity.Bottom)).

## OUI-112

Claim: One UI information dialogs appear in the center of the screen.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/dialog.html
Source title: Dialog (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Information dialogs "appear in the center of the screen."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-113

Claim: One UI dialogs requiring a decision persist until the user makes a choice, taps Back, or taps outside the dialog.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/dialog.html
Source title: Dialog (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "won't disappear until the user makes a choice, taps the Back button, or taps another location outside."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-114

Claim: One UI list main text should be a noun or short verbal phrase kept within 31 characters.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/list.html
Source title: Lists (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "keep them within 31 characters to avoid spilling over to a second line."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Correct URL is list.html (singular).

## OUI-115

Claim: In One UI lists, a toggle switch should be placed on the right side of the row.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/list.html
Source title: Lists (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "a toggle switch should be provided on the right side of that row."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-116

Claim: All One UI search boxes support auto-complete and predictive text.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/search.html
Source title: Search (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "All search boxes in One UI support auto-complete and predictive text."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-117

Claim: One UI search shows recently searched keywords and suggestions before the user types.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/search.html
Source title: Search (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Before a user even types… we offer a list of recently searched keywords and other suggestions."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-118

Claim: One UI toasts should be about one line and never exceed 3 lines in any language.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/toast.html
Source title: Toasts (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Toasts should be about one line, and should never exceed 3 lines in any language."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Correct URL is toast.html.

## OUI-119

Claim: One UI toasts are for relatively minor success/failure information, while serious issues should use a popup.
Category: component
Source URL: https://developer.samsung.com/one-ui/comp/toast.html
Source title: Toasts (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Toasts for "relatively minor information"; serious issues "use a popup."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: No duration value stated.

## OUI-120

Claim: In One UI 7, swiping the upper-right corner opens Quick Settings while swiping elsewhere opens the Notification panel.
Category: navigation
Source URL: https://design.samsung.com/global/contents/one-ui-7/index.html
Source title: One UI 7 (Samsung Design)
Evidence type: EXPLICIT
Evidence: "swipe the upper right corner for the Quick Settings panel, or swipe anywhere else… for the Notification panel."
Contains numeric value: NO
Version-specific: YES
Confidence: high
Notes: One UI 7 specific; differs from the single combined Quick panel on the developer structure page (version drift).

## OUI-121

Claim: One UI uses motion to emotionally engage users and help them understand functions and processes.
Category: motion
Source URL: https://developer.samsung.com/one-ui/motion/intro.html
Source title: Motion introduction (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "uses motion to emotionally engage users and help them understand functions and processes."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-122

Claim: One UI motions should happen instantly and respond naturally to the user's touch.
Category: motion
Source URL: https://developer.samsung.com/one-ui/motion/intro.html
Source title: Motion introduction (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "motions should happen instantly and respond naturally to the user's touch."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-123

Claim: One UI transitions should be smooth and uninterrupted.
Category: motion
Source URL: https://developer.samsung.com/one-ui/motion/intro.html
Source title: Motion introduction (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Transitions "should be smooth and uninterrupted."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-124

Claim: One UI motion duration should be at least 100 ms (the minimum recognizable length).
Category: motion
Source URL: https://developer.samsung.com/one-ui/motion/basic.html
Source title: Motion basics and usage (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "at least 100 ms, which is the minimum recognizable length."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-125

Claim: One UI motion duration should never exceed 500 ms.
Category: motion
Source URL: https://developer.samsung.com/one-ui/motion/basic.html
Source title: Motion basics and usage (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "should never exceed 500 ms to avoid interfering with subsequent tasks."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-126

Claim: One UI's basic path interpolator (easing curve) is [0.22, 0.25, 0.00, 1.00].
Category: motion
Source URL: https://developer.samsung.com/one-ui/motion/basic.html
Source title: Motion basics and usage (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Basic Path Interpolator "[0.22, 0.25, 0.00, 1.00]".
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-127

Claim: One UI basic motions accelerate quickly then slow down gradually.
Category: motion
Source URL: https://developer.samsung.com/one-ui/motion/basic.html
Source title: Motion basics and usage (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Basic motions in One UI accelerate quickly then slow down gradually."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-128

Claim: For One UI image cross-fades the new image fades in before the old fully disappears, while for text the new text waits until the old is fully gone before fading in.
Category: motion
Source URL: https://developer.samsung.com/one-ui/motion/basic.html
Source title: Motion basics and usage (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Cross-fade guidance for images vs text.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: medium
Notes: none

## OUI-129

Claim: One UI sounds should only be used when necessary to avoid irritating users.
Category: sound-haptic
Source URL: https://developer.samsung.com/one-ui/sound-and-haptic/sound.html
Source title: Sound (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "sounds should only be used when necessary."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-130

Claim: One UI provides different sounds for general input versus cancel/delete actions.
Category: sound-haptic
Source URL: https://developer.samsung.com/one-ui/sound-and-haptic/sound.html
Source title: Sound (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "different sounds for general input and cancel/delete actions."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-131

Claim: One UI uses a sine waveform to provide a soft and clean feel for sound.
Category: sound-haptic
Source URL: https://developer.samsung.com/one-ui/sound-and-haptic/sound.html
Source title: Sound (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "The sine waveform is used to provide a soft and clean feel."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: No frequency stated.

## OUI-132

Claim: One UI haptic feedback is designed to be crisp and refined to help users avoid overstimulation.
Category: sound-haptic
Source URL: https://developer.samsung.com/one-ui/sound-and-haptic/haptic.html
Source title: Haptic (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Crisp and refined haptic feedback helps users avoid overstimulation."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-133

Claim: One UI keyboard haptics provide different feedback for special keys such as Delete, Spacebar, and Function keys.
Category: sound-haptic
Source URL: https://developer.samsung.com/one-ui/sound-and-haptic/haptic.html
Source title: Haptic (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "different feedback for special keys such as Delete, Spacebar, and Function keys."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-134

Claim: One UI synchronizes haptic timing and nuance with the accompanying visual movement.
Category: sound-haptic
Source URL: https://developer.samsung.com/one-ui/sound-and-haptic/haptic.html
Source title: Haptic (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "the movement's timing and nuance match perfectly with the vibration."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-135

Claim: One UI writing keeps every bit of text purposeful and omits text that does not help users choose, act, or understand.
Category: writing
Source URL: https://developer.samsung.com/one-ui/writing/focused-and-purposeful.html
Source title: Focused and purposeful (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "If text isn't meeting one of these goals, we leave it out."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-136

Claim: One UI writing gives users an action instead of a dead end.
Category: writing
Source URL: https://developer.samsung.com/one-ui/writing/focused-and-purposeful.html
Source title: Focused and purposeful (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Give users "an action instead of a dead end."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-137

Claim: One UI limits popups to important cases such as data input, deletion confirmation, personal-info consent, or critical information.
Category: writing
Source URL: https://developer.samsung.com/one-ui/writing/simple-and-human.html
Source title: Simple and human (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Limit popups to "data input, deletion confirmation, personal info consent, or critical information."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-138

Claim: One UI writing uses inclusive gender-neutral language, preferring singular "they" and avoiding constructions like "he/she."
Category: writing
Source URL: https://developer.samsung.com/one-ui/writing/simple-and-human.html
Source title: Simple and human (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Use singular "they" — "we always avoid constructions like 'he/she.'"
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-139

Claim: One UI writing limits rhetorical questions to one.
Category: writing
Source URL: https://developer.samsung.com/one-ui/writing/empowering.html
Source title: Empowering and engaging (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Use rhetorical questions but "limit it to one."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-140

Claim: One UI writing tells users the solution to a problem when there is one.
Category: writing
Source URL: https://developer.samsung.com/one-ui/writing/empowering.html
Source title: Empowering and engaging (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "If there's a solution to a problem, we tell users what it is."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: e.g. "Remove filter to take burst shots" over a blame framing.

## OUI-141

Claim: One UI writing avoids blaming the user.
Category: writing
Source URL: https://developer.samsung.com/one-ui/writing/empowering.html
Source title: Empowering and engaging (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Prefers a solution framing over "Can't take burst shots while filter applied."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-142

Claim: One UI accessibility is guided by four principles (4C): Consideration, Comprehensiveness, Coherence, and Co-creation.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/intro.html
Source title: Accessibility introduction (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Lists the four 4C principles.
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-143

Claim: One UI requires small text to have a contrast ratio of at least 4.5:1 with the background.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/color-contrast.html
Source title: Color and contrast (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "small text should have at least a 4.5:1 contrast with the background color."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: WCAG-derived but stated on Samsung's page.

## OUI-144

Claim: One UI requires large text (more than 18 dp normal, or 14 dp bold) to have a contrast ratio of at least 3:1.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/color-contrast.html
Source title: Color and contrast (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "For large text (more than 18 dp for normal text or 14 dp for bold text), the contrast should be at least 3:1."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: Defines "large text" thresholds.

## OUI-145

Claim: The 2019 One UI guidelines specify per-size minimum contrast ratios: ~12–13 dp = 4.5:1 (regular and bold); 14 & 17 dp = 4.5:1 regular / 3:1 bold; 18 dp and 19 dp+ = 3:1 for both.
Category: accessibility
Source URL: https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
Source title: One UI Design Guidelines (PDF)
Evidence type: EXPLICIT
Evidence: Contrast table rows by dp size (Regular/Bold).
Contains numeric value: YES
Version-specific: YES
Confidence: high
Notes: 2019 PDF; the per-size basis behind OUI-143/144.

## OUI-146

Claim: One UI requires all text (except subtitles and text within images) to be resizable up to 200% without loss of content or functionality.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/layout-and-typo.html
Source title: Layout and typography (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "resizable up to 200% without affecting content or functionality."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-147

Claim: One UI requires touch areas to be large enough to touch easily and have enough spacing to prevent missed touches.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/layout-and-typo.html
Source title: Layout and typography (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Touch areas should be large enough… have enough spacing… to prevent missed touches."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: No touch-target dp size stated (do not invent 48dp).

## OUI-148

Claim: One UI requires controls to stop content that plays automatically for more than 5 seconds.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/interaction-and-control.html
Source title: Interaction and control (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "give users controls to stop content lasting more than 5 seconds."
Contains numeric value: YES
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-149

Claim: One UI requires alternative ways to perform complex actions such as drag-and-drop or multi-finger gestures.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/interaction-and-control.html
Source title: Interaction and control (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Provide alternative ways of performing complex actions such as drag and drop or multifinger gestures."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-150

Claim: One UI requires button/controller locations to be designed consistently.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/interaction-and-control.html
Source title: Interaction and control (Samsung Developer)
Evidence type: EXPLICIT
Evidence: Control locations "should be designed in a consistent way."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-151

Claim: One UI requires focus to flow logically and a focus mark to be shown when the accessibility device is active.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/focus-order.html
Source title: Focus order (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "the focus flows logically"; "a focus mark should be shown."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-152

Claim: One UI focus order does not support looping.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/focus-order.html
Source title: Focus order (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Looping is not supported."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-153

Claim: One UI does not focus decorative elements, auxiliary images, or empty spaces.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/focus-order.html
Source title: Focus order (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "There's no need to focus on decorative elements, auxiliary images, or empty spaces."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-154

Claim: One UI content must not identify controls solely by shape, color, or location (e.g. "Tap Start" is effective, "Tap the square button below" is not).
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/content.html
Source title: Content (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "'Tap Start' is effective, but 'Tap the square button below' is not."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-155

Claim: One UI requires audio cues to be supplemented with visual/text representation.
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/content.html
Source title: Content (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "if you instruct users to 'Start after the beep', make sure you provide visual representation."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: Also provide subtitles/scripts/sign language where possible.

## OUI-156

Claim: One UI requires avoiding strobing effects and sudden, rapid changes in brightness (and warning users if such events occur).
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/content.html
Source title: Content (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Avoid strobing effects, sudden and rapid changes in brightness. Warn users if such events will occur."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: none

## OUI-157

Claim: One UI requires that color alone must not convey information; additional visual marks should be provided (test by switching the UI to grayscale).
Category: accessibility
Source URL: https://developer.samsung.com/one-ui/accessibility/color-contrast.html
Source title: Color and contrast (Samsung Developer)
Evidence type: EXPLICIT
Evidence: "Provide additional marks as well"; "switch your UI to grayscale to check whether information is being conveyed clearly without color."
Contains numeric value: NO
Version-specific: UNKNOWN
Confidence: high
Notes: References the third-party Colour Contrast Analyser (not a Samsung source).

---

## Registry summary

- **Total claims:** 157 (OUI-001 … OUI-157)
- **By category:** principle 14 · layout 15 · large-screen 12 · foldable 13 · color 8 · dark-mode 4 · typography 3 · iconography 5 · component 17 · navigation 8 · interaction 8 · motion 8 · sound-haptic 6 · writing 7 · accessibility 16 · other 13
- **Evidence type:** EXPLICIT 154 · OBSERVED 3 (OUI-091, OUI-096, and the One UI 7 icon visuals) · INFERRED 0
- **Numeric claims (require exact official source):** OUI-038, 042, 049, 050, 054, 055, 060, 073, 074, 078–083, 090, 094, 098, 100–102, 104, 110, 114, 118, 124, 125, 126, 139, 143, 144, 145, 146, 148
- **Version-specific = YES:** OUI-004, 005, 023, 029, 030, 042, 060, 071, 081, 082, 083, 084, 085, 088, 089, 095, 096, 120, 145 — most numeric hex/dp values trace to the **2019 One UI Design Guidelines PDF** (One UI 2 era) and should be treated as generation-specific, not necessarily One UI 7.
