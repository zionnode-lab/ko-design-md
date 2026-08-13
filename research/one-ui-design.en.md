---
name: 삼성 One UI
design_system_name: One UI
slug: samsung-one-ui
category: developer
last_updated: "2026-08-13"
created_at: "2026-08-13"
sources:
  - https://developer.samsung.com/one-ui/index.html
  - https://design.samsung.com/global/contents/one-ui/
  - https://developer.samsung.com/one-ui/layout/basic.html
  - https://developer.samsung.com/one-ui/layout/grid.html
  - https://developer.samsung.com/one-ui/structure/basic.html
  - https://developer.samsung.com/one-ui/structure/visual-depth.html
  - https://developer.samsung.com/one-ui/color/system.html
  - https://developer.samsung.com/one-ui/color/theme.html
  - https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf
  - https://design.samsung.com/global/contents/samsungone/
  - https://developer.samsung.com/one-ui/iconography/background.html
  - https://developer.samsung.com/one-ui/iconography/color.html
  - https://developer.samsung.com/one-ui/comp/app-bar.html
  - https://developer.samsung.com/one-ui/comp/bottom-bar.html
  - https://developer.samsung.com/one-ui/comp/bottom-navigation.html
  - https://developer.samsung.com/one-ui/comp/button.html
  - https://developer.samsung.com/one-ui/comp/dialog.html
  - https://developer.samsung.com/one-ui/comp/list.html
  - https://developer.samsung.com/one-ui/comp/search.html
  - https://developer.samsung.com/one-ui/comp/toast.html
  - https://developer.samsung.com/one-ui/motion/intro.html
  - https://developer.samsung.com/one-ui/motion/basic.html
  - https://developer.samsung.com/one-ui/sound-and-haptic/sound.html
  - https://developer.samsung.com/one-ui/sound-and-haptic/haptic.html
  - https://developer.samsung.com/one-ui/writing/focused-and-purposeful.html
  - https://developer.samsung.com/one-ui/writing/simple-and-human.html
  - https://developer.samsung.com/one-ui/writing/empowering.html
  - https://developer.samsung.com/one-ui/accessibility/intro.html
  - https://developer.samsung.com/one-ui/accessibility/color-contrast.html
  - https://developer.samsung.com/one-ui/accessibility/layout-and-typo.html
  - https://developer.samsung.com/one-ui/accessibility/interaction-and-control.html
  - https://developer.samsung.com/one-ui/accessibility/focus-order.html
  - https://developer.samsung.com/one-ui/accessibility/content.html
  - https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html
  - https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html
  - https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html
  - https://developer.samsung.com/galaxy-z/multi-window.html
  - https://design.samsung.com/global/contents/one-ui-7/index.html
related_services: []
lang: en
---

# 삼성 One UI — design.md

> A catalog entry for One UI, the OS design language applied across Samsung Galaxy devices (phones, tablets, foldables, watches, PCs), assembled exclusively from publicly accessible official Samsung sources [src:1]. **This document is not an official Samsung release.** It restructures Samsung's published principles and figures into a form usable for downstream UI generation. Because One UI ships no open token package, this document treats **version-independent (evergreen) principles as its default layer** and **quarantines generation-bound figures with an explicit provenance stamp** — most numeric tokens trace to the public One UI Design Guidelines of October 2019 (the One UI 2 generation) [src:9].

## Brand & Style

One UI's stated goal is to create "joyful and comfortable" experiences on any device — phone, tablet, watch, earbud, or PC [src:1]. Samsung's design portal frames the same intent as connecting devices for a seamless experience whose simplicity makes it easy to use [src:2]. One UI is therefore not a single app's brand language but an **OS-level design language that enforces consistency across devices**.

The official principle wording differs by channel. The developer portal states **Focus on the task at hand · Interact naturally · Be visibly comfortable · Make things responsive** [src:1]; the design portal states **One Makes It Natural · One Is Clean and Easy · One Keeps Consistency · One Attracts All Senses** [src:2]; the watch (Tizen) set is different again. No single canonical list is published, so this document takes the **durable concepts shared across the sets** as its spine:

- **Viewing/interaction split** — the top of the screen is for viewing, the lower part for interaction [src:1]. The design portal confirms the same rule: areas for viewing and touching are clearly distinguished [src:2].
- **One-handed reachability** — interactive elements stay within thumb reach even on large devices [src:1]; single-handed operation is an explicit goal [src:2].
- **Focus on the essential** — simple, intuitive design keeps users on their content [src:1]; unnecessary elements are removed to guide users toward important functions [src:2]; user journeys are kept as short and smooth as possible [src:1].
- **Responsive adaptation** — the layout adapts to any device or screen size while controls remain within reach [src:1].
- **Visual comfort** — Dark mode (reduced eye fatigue and glare), a high-contrast keyboard, and variable font sizes are named accessibility devices [src:1].

Generational visual language varies on top of these principles. One UI 7 (2025, the Galaxy S25 generation) declares the highly scalable **circle** as a screen-wide visual motif, producing soft curved outlines and clarifying information hierarchy across components and content [src:38]. That circle-motif statement is published for One UI 7 only — it is not retroactive to every generation.

The resulting mood: **calm solid surfaces + restrained color + rounded geometry + bottom-weighted interaction**. The style exists to avoid interfering with the task at hand, not to decorate [src:1].

## Colors

> **Published values — One UI 2 generation (2019-10) (verified 2026-08-13).** The numeric tokens below are the role colors stated on the developer portal color page [src:7] and in the public 2019 One UI Design Guidelines PDF [src:9]. The two channels agree with each other, but the PDF is a 2019 (One UI 2 / Android 10 era) document and the developer page carries no version label. **One UI 7's system palette figures are unpublished** [src:38], so treat these values as **the last publicly published generation's values**, not a palette common to all current generations. No full ramp (grays etc.) has been published, so none is listed.

One UI relies on "rich, solid colors," and keeps their brightness and saturation within particular ranges so the most important information stays identifiable and readable [src:7] (the numeric ranges themselves are not published as text — see Known Gaps). Color is defined by role — Primary drives floating action buttons, sliders, input fields, and focused items; Primary dark drives contained-button backgrounds, app-bar text, and dialog buttons; Color control activated drives the active state of selection controls such as checkboxes, radio buttons, and toggles [src:7].

```yaml
primary: oklch(0.617 0.208 255.8)                  # #0381fe · same in Light/Dark · One UI 2 (2019) published value
primary-dark: oklch(0.561 0.186 255.2)             # #0072de · Light-theme value · One UI 2 (2019) published value
primary-dark-on-dark: oklch(0.661 0.182 256.7)     # #3e91ff · Primary dark in the Dark theme · One UI 2 (2019) published value
color-control-activated: oklch(0.661 0.182 256.7)  # #3e91ff · both themes, active selection controls · One UI 2 (2019) published value
white: oklch(0.985 0 0)                            # #fafafa · both themes · One UI 2 (2019) published value
black: oklch(0 0 0)                                # #000000 · Black in the Light theme · One UI 2 (2019) published value
black-dark: oklch(0.134 0 0)                       # #080808 · Dark-theme background (near-black, not pure black) · One UI 2 (2019) published value
```

`{colors.primary-dark-on-dark}` and `{colors.color-control-activated}` sharing one value is not a transcription error — it is the published data [src:7]: the single "Primary dark" role changes value per theme, and its dark-theme value coincides with the activated-control color.

Palette operating model: One UI's palette runs on Android's categorized theme-palette system — changing one category's value updates every on-screen element in that category at once [src:9]. **This is a statement that Samsung uses Android's theming mechanism, not that Material Design's visual rules are One UI rules** — One UI enforces its own role values and placement rules on top of that mechanism (see Do's and Don'ts).

Dark mode is a built-in device, not an option. In Dark mode, backgrounds, menus, and other UI elements turn black or dark gray to reduce glare [src:8], and apps must be tested in both Light and Dark modes before release [src:8]. The rationale for the near-black `{colors.black-dark}` background is also published — on a device with a black bezel, a black background merges the bezel/screen boundary so the screen appears visually expanded [src:9]. Letting users switch to Dark mode at a desired or scheduled time is recommended for every app [src:9].

## Typography

One UI's public typography information is published **without a type scale** — no official document publishes a stepped size/line-height ladder as text (see Known Gaps). What is verifiable:

- Per the 2019 guidelines, One UI's **default system font is Roboto** (the Android system font) [src:9]. Whether later generations replaced the system font is not confirmed in public documents.
- **SamsungOne is a separate brand typeface** — a corporate-identity family covering 26 writing systems, 400+ languages, and 25,000+ glyphs [src:10]. It is never stated as One UI's UI-rendering font. Do not conflate the two.
- Accessibility requirements are the operative typography rules: variable font sizes [src:1], and all text except subtitles and text within images must scale to **200%** without loss of content or functionality [src:30].

```yaml
font-sans: >
  Roboto, "Pretendard Variable", Pretendard, system-ui, sans-serif
font-sans-src: https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap
```

The stack above is a catalog interpretation — Latin loads Roboto per the 2019 publication [src:9], and because Roboto does not cover Korean glyphs, Pretendard sits in the fallback as a web substitution. No official web distribution of Samsung's Korean system font was found. Weights 400/500/700 follow the Roboto distribution, not a published One UI weight policy.

## Spacing

The spacing system is published as rules, not a ladder. Verified rules:

- To avoid conflicts with curved edges and corners, display information and place interactive components with **margins of at least 24 dp on both left and right sides** [src:4]. The same value appears in the 2019 guidelines [src:9].
- Accidental touches in the margins are blocked by two system zones — the **Reject zone** blocks touches in the interaction area, and the **Grip zone** blocks palm and three-finger touches that occur while holding the phone [src:4]. Zone sizes are unpublished.
- The top viewing area uses wide margins to give an impression of open space [src:3] — an intent rule, not a figure.
- Optimize on-screen items to avoid each device's camera cutout (guidance exists for both 90° and 270° orientations) [src:4].

```yaml
margin-side-min: 24px # published as 24dp — the 1dp≈1px web mapping is a catalog interpretation · minimum side margin
```

## Rounded

One UI's rounding consists of the principle of "standardized rounded corners for consistency" [src:2] plus two sets of published 2019 figures.

> **Published values — One UI 2 generation (2019-10) (verified 2026-08-13).** The thumbnail radii below come from the Thumbnail radius section of the 2019 guidelines [src:9]; the button radius comes from the drawable spec on the developer portal's button page [src:16]. One UI 7 describes a shift toward circle-based curvature [src:38] but publishes no figures.

```yaml
radius-thumbnail-l: 26px # published as 26dp · large focus blocks/thumbnails · One UI 2 (2019)
radius-thumbnail-m: 20px # published as 20dp · medium thumbnails · One UI 2 (2019)
radius-thumbnail-s: 12px # published as 12dp · small thumbnails · One UI 2 (2019)
radius-button: 18px # published as 18dp · button mask/background drawable spec
```

Thumbnail radius is chosen among 26/20/12 dp according to the screen grid and target size [src:9]. The button's 18 dp lives in implementation XML on the official page rather than in rule prose, so treat its rule strength accordingly [src:16].

## Elevation & Depth

One UI's depth is defined not as a shadow ladder but as a **division of labor among blur, dim, and shadow** [src:6]:

- **Blur** — emphasizes current information while keeping a connection to the previous screen. Combine with a light or dark dim to match the theme; keep it neither too weak nor too strong [src:6].
- **Dim** — clarifies each level of the hierarchy and concentrates attention on the topmost element. Apply evenly; avoid exposing multiple hierarchy levels on one screen [src:6].
- **Shadow** — a soft shadow is used only to show connections between closely related information. **Never apply dim and shadow at the same time** [src:6].

No figures (blur radius, dim opacity, shadow offsets) are published — port the role rules above without inventing values. One UI 7 adds layered blur, "colored glass" overlays, and gradient backgrounds on certain full-screen apps (Clock, Calendar, Reminder) [src:38] — a One UI 7-only statement.

## Shapes

One UI's geometry is **rounded rectangles and circles**. Elements such as rounded corners are standardized to unify smart-device experiences [src:2], and One UI 7 extends the circle into a screen-wide visual motif [src:38].

Icon rules are explicitly published:

- App icons are **squares with smooth rounded corners and outlines** — the rounding makes icons feel softer and more inviting [src:11]. No corner-radius figure is published.
- Backgrounds default to **bright, vibrant solid colors with white symbols** — the contrast between colored background and white symbol produces an intuitive, distinct identity [src:12].
- If a gradient is used, restrict it to **3 or fewer analogous colors** [src:12].
- Stroke icons use **rounded terminals** while corners stay sharp, creating contrast with the rounded corners [src:9].

(Observation) The icon visuals on the One UI 7 page show circle-based, softly curved forms, but that page states some imagery is AI-generated simulation [src:38], so this stays an observation and is not promoted to a rule.

## Components

Component rules are the most durable part of One UI's publications — most of the rules below are served as current documentation on the developer portal without generation labels. Each component's placement rule concretizes the viewing/interaction-area principle [src:3].

### app-bar

The title bar of the top viewing area. Two forms exist: standard (condensed) and extended [src:13]. Action buttons sit on the right — **no more than three per page** is recommended; overflow goes to More options at the far right [src:13]. Title text may take `{colors.primary-dark}`-family emphasis [src:7].

### app-bar-extended

The extended app bar centers its title **in the middle of the expanded area** [src:13], condenses to standard height on downward scroll, and re-expands on upward scroll [src:13]. The viewing area's wide-margin, center-aligned principles [src:3] are condensed into this component — the expanded app bar *is* the viewing area.

### bottom-bar

The action toolbar at the bottom of the screen. Holds a **maximum of 5** action buttons and **cannot display only one** [src:14]. Beyond five, show the four most-used and push the rest into a More options menu at the far right [src:14]. Buttons must include **both an icon and text** [src:14], and may hide on downward scroll [src:14].

### bottom-navigation

Top-level navigation tabs. **Fewer than 4 recommended, 5 maximum**, and tabs are **text-only** [src:15]. **Swiping between tabs is not supported** [src:15] — a One UI-specific rule that avoids conflicts with gesture navigation, so do not attach a swipe pager. On screens with tabs, the top title may be omitted [src:15].

### button-flat

A button without a background surface. Use flat buttons in toolbars and dialogs to avoid adding unnecessary layers [src:16]. Text color is `{colors.primary-dark}` (or `{colors.primary-dark-on-dark}` in the dark theme) [src:7].

### button-contained

A surfaced button. **A gray background signals moderate emphasis; a colored background signals high emphasis** [src:16]. The high-emphasis background is the `{colors.primary}` family [src:7]; radius is `{rounded.radius-button}` [src:16]. **Use only one button style on any given screen** [src:16] — emphasis is graded by color, never by mixing style systems.

### dialog-choice

Choice/confirmation dialogs appear **at the bottom of the screen** [src:17] — the reachability principle applied to decisions [src:1]. They persist until the user chooses, taps Back, or taps outside the dialog [src:17].

### dialog-info

Information dialogs appear **in the center of the screen** [src:17]. No decision is required, so visibility outranks reachability. Popups themselves are limited to data input, deletion confirmation, personal-information consent, and critical information [src:26].

### list-item

List main text is a noun or short verbal phrase kept **within 31 characters** so it never wraps to a second line [src:18]. If a row needs a toggle, place it **on the right side of the row** [src:18]. Order lists by priority to ease scanning [src:18].

### search

Every One UI search box supports **auto-complete and predictive text**, and surfaces recent searches and contextual suggestions before the user types [src:19].

### toast

Toasts are **about one line — never more than 3 lines in any language** [src:20]. Use them only for relatively minor success/failure information; serious issues use a popup [src:20]. No display-duration figure is published.

## Motion

One UI motion exists for emotional engagement and causal clarity — it helps users understand functions and processes [src:21], responds instantly and naturally to touch [src:21], and keeps transitions smooth and uninterrupted [src:21].

The numeric rules are explicit [src:22]:

- Duration is **at least 100 ms** (the minimum recognizable length) and **never exceeds 500 ms** (to avoid interfering with subsequent tasks).
- The basic easing is the **Basic Path Interpolator `[0.22, 0.25, 0.00, 1.00]`** — accelerate quickly, then decelerate gradually. In CSS this maps to `cubic-bezier(0.22, 0.25, 0, 1)` (the notation mapping is a catalog interpretation).
- Cross-fade rules: for **images**, the new image fades in before the old one fully disappears; for **text**, the new text waits until the old is completely gone before fading in [src:22].

## Sound & Haptics

Sound is used **only when necessary** — overuse irritates users [src:23]. General input and cancel/delete actions get different sounds so the direction of an action is audible [src:23], and the **sine waveform** is used for a soft, clean feel [src:23].

Haptics are designed **crisp and restrained** to avoid overstimulation [src:24]. Keyboard haptics differentiate special keys — Delete, Spacebar, Function — so key type is distinguishable by touch alone [src:24], and vibration timing and nuance are synchronized exactly with the accompanying visual movement [src:24].

## Writing

- **No purposeless text** — every bit of text helps users make a choice, take an action, or understand what is happening; anything else is left out [src:25]. Give an action instead of a dead end [src:25].
- **Interrupt with popups only for important cases** — data input, deletion confirmation, personal-information consent, critical information [src:26].
- **Inclusive language** — gender-neutral wording, singular "they," never "he/she" constructions [src:26] (a rule for English copy; no public document defines a Korean honorific register for One UI copy — see Known Gaps).
- **Limit rhetorical questions to one** [src:27]; when a problem has a solution, state the solution [src:27]; never blame the user — prefer "Remove filter to take burst shots" over "Can't take burst shots while filter applied" [src:27].

## Accessibility

One UI accessibility follows the 4C principles — **Consideration (empathize with the user's point of view) · Comprehensiveness · Coherence (make every device accessible) · Co-creation (design together with users)** [src:28].

Numeric rules:

- Small text needs a contrast ratio of **at least 4.5:1** against its background; large text (over 18 dp normal, or 14 dp bold) needs **at least 3:1** [src:29]. The 2019 guidelines publish this as a per-size table (12–13 dp → 4.5:1; 14 & 17 dp → 4.5:1 regular / 3:1 bold; 18 dp+ → 3:1) [src:9]. These are WCAG-derived thresholds that Samsung formally adopted and published.
- All text except subtitles and text within images must survive **200% scaling** [src:30].
- Provide **stop controls for auto-playing content that lasts more than 5 seconds** [src:31].

Non-numeric rules:

- Touch areas must be "large enough to touch easily, with enough spacing to prevent missed touches" [src:30]. **No official touch-target dp figure is published** — do not substitute an arbitrary 48 dp; port the sufficiency rule instead.
- Provide alternatives for complex gestures (drag-and-drop, multi-finger), and keep control locations consistent [src:31].
- Focus flows logically; show a focus mark when an accessibility device is active; never focus decorative elements, auxiliary images, or empty space. **Looping is not supported** [src:32].
- Never identify controls by shape, color, or location alone — "Tap Start" works, "Tap the square button below" does not [src:33]. Pair audio cues with visual representation; avoid strobing and sudden rapid brightness changes [src:33].
- Never convey information through color alone — add visual marks, and check by switching the UI to grayscale [src:29].

## Do's and Don'ts

**Do**

- Split the screen into a top viewing area (title, non-interactive) and a lower interaction area, and gather controls at the bottom [src:3].
- Put decision dialogs at the bottom of the screen [src:17].
- Keep side margins at `{spacing.margin-side-min}` (24 dp) minimum [src:4].
- Use one button style per screen; grade emphasis by background — gray (moderate) vs colored (high) [src:16].
- Give bottom-bar buttons both an icon and text [src:14].
- Test in both Light and Dark modes before release [src:8].
- Run motion within 100–500 ms on a fast-acceleration, slow-deceleration curve [src:22].
- Verify text survives 200% scaling and small-text contrast reaches 4.5:1 [src:29][src:30].
- On large screens, open pop-ups near the triggering element to reduce hand travel [src:34].

**Don't**

- Don't attach swipe-based tab switching to bottom navigation — One UI does not support it [src:15].
- Don't apply the dim effect and the shadow effect at the same time [src:6].
- Don't convey state or information through color alone [src:29].
- Don't invent unpublished figures — touch-target dp, shadow values, a type scale, and dim opacity do not exist in One UI's public documents. When a value this document lacks is needed, label it as your product's own decision, not One UI's.
- **Don't treat Material Design defaults as One UI rules** — One UI uses Android's theming mechanism [src:9], but its visual rules (bottom-anchored dialogs, text-only bottom tabs, no swipe paging, the viewing/interaction split) differ from Material defaults. Don't leave Material components untouched and call the result "One UI style."
- Don't transplant Samsung's device/OS product domain — foldable hardware concepts, cover/main screens [src:36], system surfaces like Lock/Home/Recents/Quick panel/Edge panel [src:5], Galaxy Settings copy — into an unrelated product. Borrow the visual and behavioral language, not the Galaxy product context.
- Don't surface the design system's own name ("One UI" wordmark, "Samsung"/"Galaxy" branding, `sec_*` / `one_ui_*`-style naming) in the generated product's headers, titles, labels, or class names — if attribution is needed, keep it to a footer note.
- Don't present this document or anything built from it as an official Samsung release or specification — the One UI trademark and the original guidelines remain Samsung Electronics'.

## Responsive Behavior

One UI is designed for every display size, resolution, and aspect ratio — phones, tablets, foldables, DeX monitors, and split-screen [src:4]. The dp thresholds below are served as current documentation on the developer portal.

### Window classes

| Class | Width (dp) | Representative devices | Navigation [src:34] |
| --- | --- | --- | --- |
| Compact | < 600 | Phone in portrait [src:35] | Navigation bar + modal drawer |
| Medium | 600 ≤ w < 840 | Z Fold portrait/landscape, small tablet portrait [src:35] | Navigation rail + modal drawer |
| Expanded | 840 ≤ w | Tablet portrait/landscape [src:35] | Navigation rail + modal/standard drawer |

Use a large-screen layout at 600 dp and above [src:35].

### Large screens

- Never stretch the phone layout — stretched apps are harder to read and waste the space; use a multi-pane layout to show more at once [src:34].
- Multi-pane ratios: **42% : 58% at 600 ≤ w < 960 dp**, **38% : 62% at 960 dp and above** [src:34]. (The 840 dp window-class threshold and the 960 dp ratio threshold are two different published systems — recorded as published.)
- The four large-screen principles: show menus together with content, adjust grids for large screens, avoid switching context (pop-overs instead of full-screen transitions for small inputs), keep things reachable [src:35].

### Foldables

- The foldable-only pane split is **50% : 50%** [src:34].
- App continuity: on fold/unfold transitions, fill the entire screen, preserve the scroll position, and keep the in-progress text input and keyboard state [src:36].
- Display correctly on both the cover screen and the main screen, fill the screen without letterboxing, and support landscape [src:36].
- **Avoid interactive elements near the crease** in the middle of the screen [src:36]. No keep-out figure is published.
- Flex mode (half-folded): content on top, controls on the bottom, with a visual transition in and out [src:36]. Some screens — a settings list, for example — may not need a layout change [src:36].

### Multi-window

Large screens support **up to 3 split-screen views plus 5 pop-up views** simultaneously [src:34]. Supporting drag-and-drop between visible windows and multiple app instances is recommended [src:37].

## Applied Guidance for LLMs

This section is a **catalog interpretation** that translates the cited principles above into generation-time directives — each item's evidence lives in the sections above.

When generating a screen:

1. **Vertical structure first** — titles and summaries go in the top viewing area (wide margins, center-aligned, non-interactive); buttons, inputs, and lists go below in the interaction area. The very bottom of the screen is where the most important action lives.
2. **Decisions at the bottom** — build confirmation/choice dialogs as bottom sheets; informational notices as centered dialogs.
3. **Tabs are text, five at most** — no icon-only tabs and no swipe pager on bottom navigation.
4. **One button system per screen** — pick flat or contained, and raise emphasis only through background color (gray → colored).
5. **Color by role** — bind `{colors.primary}` to FABs and input focus, `{colors.primary-dark}` to emphasized/text buttons, `{colors.color-control-activated}` to active toggles and checkboxes. Keep the role structure even when rebranding the values.
6. **Dark mode is near-black** — use `{colors.black-dark}`-level near-black instead of pure black, and always generate both themes together.
7. **Motion within 100–500 ms** — `cubic-bezier(0.22, 0.25, 0, 1)`, fast in, gentle out. Text swaps fade sequentially; image swaps overlap.
8. **600 dp is the fork** — above it, switch to multi-pane (42:58, then 38:62 from 960 dp; 50:50 on foldables) and rail navigation.
9. **Stamp the generation when citing figures** — carry this document's hex/radius values together with their "One UI 2 (2019) published value" stamp. Removing the stamp turns them into an impersonation of a universal rule.
10. **Say when a value doesn't exist** — if asked for a type scale, touch-target size, or shadow values, state that One UI publishes none and mark the choice as the product's own decision.

## Known Gaps

- **No canonical principle wording** — the developer portal and the design portal publish different four-principle sets, and the watch (Tizen) line uses a third [src:1][src:2]. This document canonizes only the concepts they share.
- **Most numeric tokens are One UI 2 (2019) published values** [src:9] — One UI 7's palette and radius figures are unpublished [src:38]. Do not strip the generation stamps from the color and rounding tokens.
- **No published type scale** — the 2019 guidelines' size table exists only as an image and could not be machine-read; the system font as of 2019 is Roboto [src:9]. SamsungOne is a separate brand typeface [src:10]. No public document defines a Korean honorific register for UI copy either.
- **No official touch-target figure** — the accessibility docs require only sufficiency of size and spacing [src:30]. Also unpublished: the brightness/saturation ranges [src:7], dim/blur/shadow figures [src:6], toast duration [src:20], and Reject/Grip zone sizes [src:4].
- **One UI 7 visuals are observational evidence** — the page states some imagery is AI-generated simulation [src:38]. Colored glass, gradients, and circular icons are a direction, not tokens.

## References

1. https://developer.samsung.com/one-ui/index.html — One UI overview. The developer portal's four principles (Focus on the task at hand · Interact naturally · Be visibly comfortable · Make things responsive), cross-device philosophy, and the principle-level statement of the viewing/interaction split and reachability.
2. https://design.samsung.com/global/contents/one-ui/ — the design portal's One UI page. A differently-named four-principle set (One Makes It Natural etc.), single-handed operation, Focus Block, and the consistent upward swipe.
3. https://developer.samsung.com/one-ui/layout/basic.html — basic layout. Defines the viewing area (top · titles · wide margins · center-aligned · non-interactive) and interaction area (bottom · logical grouping · list/card/2col/3col).
4. https://developer.samsung.com/one-ui/layout/grid.html — grid system. Minimum 24 dp side margins, Reject/Grip zones, camera-cutout avoidance, all-display support statement.
5. https://developer.samsung.com/one-ui/structure/basic.html — basic structure. The five system surfaces: Lock/Home/Recents/Quick panel/Edge panel.
6. https://developer.samsung.com/one-ui/structure/visual-depth.html — visual depth. The blur/dim/shadow division of labor and the ban on simultaneous dim+shadow.
7. https://developer.samsung.com/one-ui/color/system.html — color system. Roles and published hex for Primary · Primary dark · Color control activated; the brightness/saturation-range statement (numeric ranges unpublished as text).
8. https://developer.samsung.com/one-ui/color/theme.html — theme. Dark mode's background behavior and the both-themes testing requirement.
9. https://design.samsung.com/global/contents/one-ui/download/oneui_design_guide_eng.pdf — One UI Design Guidelines PDF (2019-10, Mobile UX Center). **The primary source of this document's figures — a One UI 2-generation document.** Palette (incl. White/Black), 24 dp margins, thumbnail radii 26/20/12 dp, the per-size contrast table, Roboto as default font, icon stroke-terminal rule, dark-mode recommendation, the bezel/screen-boundary statement.
10. https://design.samsung.com/global/contents/samsungone/ — the SamsungOne brand typeface (26 writing systems · 400+ languages · 25,000+ glyphs). Basis for distinguishing the corporate brand typeface from the UI system font.
11. https://developer.samsung.com/one-ui/iconography/background.html — icon background. Rounded-corner square backgrounds with outlines.
12. https://developer.samsung.com/one-ui/iconography/color.html — icon color. Vibrant solid backgrounds + white symbols; gradients limited to 3 or fewer analogous colors.
13. https://developer.samsung.com/one-ui/comp/app-bar.html — app bar. Standard/extended forms, centered title when expanded, scroll condensing, ≤3 action buttons recommended.
14. https://developer.samsung.com/one-ui/comp/bottom-bar.html — bottom bar. Max 5 buttons, no single button, overflow rule, icon+text.
15. https://developer.samsung.com/one-ui/comp/bottom-navigation.html — bottom navigation. Fewer than 4 recommended / max 5, text-only tabs, no swiping.
16. https://developer.samsung.com/one-ui/comp/button.html — buttons. Flat/Contained types with three emphasis grades, one style per screen, the 18 dp radius in the drawable spec.
17. https://developer.samsung.com/one-ui/comp/dialog.html — dialog. Choice/confirmation at the bottom, information centered, decision-dialog persistence.
18. https://developer.samsung.com/one-ui/comp/list.html — lists. Main text within 31 characters, right-side toggles, priority ordering.
19. https://developer.samsung.com/one-ui/comp/search.html — search. Auto-complete/predictive text, pre-typing recents and suggestions.
20. https://developer.samsung.com/one-ui/comp/toast.html — toasts. About one line, never over 3, minor information only.
21. https://developer.samsung.com/one-ui/motion/intro.html — motion introduction. Emotional engagement, instant response, smooth transitions.
22. https://developer.samsung.com/one-ui/motion/basic.html — motion basics. The 100–500 ms range, Basic Path Interpolator [0.22, 0.25, 0.00, 1.00], image/text cross-fade rules.
23. https://developer.samsung.com/one-ui/sound-and-haptic/sound.html — sound. Only when necessary, distinct input vs cancel/delete sounds, sine waveform.
24. https://developer.samsung.com/one-ui/sound-and-haptic/haptic.html — haptics. Crisp and restrained, special-key differentiation, visual synchronization.
25. https://developer.samsung.com/one-ui/writing/focused-and-purposeful.html — writing: purposeful. Drop text that doesn't aid choice/action/understanding; no dead ends.
26. https://developer.samsung.com/one-ui/writing/simple-and-human.html — writing: simple. The four popup-worthy cases; singular "they."
27. https://developer.samsung.com/one-ui/writing/empowering.html — writing: empowering. One-question limit, state the solution, never blame the user.
28. https://developer.samsung.com/one-ui/accessibility/intro.html — the accessibility 4C principles.
29. https://developer.samsung.com/one-ui/accessibility/color-contrast.html — contrast. The 4.5:1/3:1 thresholds, large-text definition (18 dp/14 dp), no color-only information, grayscale check.
30. https://developer.samsung.com/one-ui/accessibility/layout-and-typo.html — layout & typography. 200% scaling; qualitative touch-area size/spacing requirement (no figure published).
31. https://developer.samsung.com/one-ui/accessibility/interaction-and-control.html — interaction. Stop controls for >5 s auto-play, alternatives to complex gestures, consistent control locations.
32. https://developer.samsung.com/one-ui/accessibility/focus-order.html — focus order. Logical flow, focus mark, no looping, decorative elements excluded.
33. https://developer.samsung.com/one-ui/accessibility/content.html — content. No shape/color/location-only references, visual pairing for audio, no strobing.
34. https://developer.samsung.com/one-ui/largescreen-and-foldable/intro.html — designing for large screens. Multi-pane ratios (42:58 / 38:62 / foldable 50:50), navigation per window class, 3 split + 5 pop-up, near-trigger pop-ups.
35. https://developer.samsung.com/one-ui/largescreen-and-foldable/large_screen_layout.html — large-screen layout. The 600 dp threshold, window classes (600/840 dp) with device mapping, the four large-screen principles.
36. https://developer.samsung.com/one-ui/largescreen-and-foldable/designing_for_foldable.html — designing for foldables. The three app-continuity rules, cover/main screens, no letterboxing, crease avoidance, Flex mode.
37. https://developer.samsung.com/galaxy-z/multi-window.html — multi-window (developer documentation). 3+ simultaneous apps, drag-and-drop, multi-instance.
38. https://design.samsung.com/global/contents/one-ui-7/index.html — the One UI 7 design page. Circle motif, layered blur · colored glass · gradients. No figures; the page notes some imagery is AI-generated simulation — visuals treated as observational evidence only.
