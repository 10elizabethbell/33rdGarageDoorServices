---
name: 33rd Garage Door Services
description: The garage's own pegboard wall, hung with real door hardware you can grab and swing.
colors:
  emergency-red: "#c8321f"
  emergency-red-pressed: "#a8281a"
  manila-tag: "#ecdcae"
  manila-field: "#fbf4dc"
  manila-chip: "#f7ecca"
  manila-rule: "#8c7a4c"
  tag-ink: "#2a2416"
  tag-ink-soft: "#5c4f30"
  pegboard: "#1d4660"
  pegboard-deep: "#173a51"
  pegboard-lit: "#24556f"
  pegboard-shadow: "#122f42"
  peg-hole: "#0a1f2d"
  board-ink: "#f1f5f7"
  board-ink-soft: "#bcd0dd"
  galvanized: "#c9d3da"
  error-oxide: "#9b2414"
typography:
  display:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(46px, 14vw, 92px)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.025em"
  headline:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(32px, 9vw, 56px)"
    fontWeight: 900
    lineHeight: 0.98
    letterSpacing: "-0.02em"
  statement:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(28px, 7.4vw, 46px)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.015em"
  stamped-number:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(36px, 10.5vw, 60px)"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.02em"
    fontFeature: "tnum"
  title:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(22px, 6vw, 32px)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.01em"
  tag-title:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "26px"
    fontWeight: 900
    lineHeight: 1.05
    letterSpacing: "-0.01em"
  body:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  lede:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 20px)"
    fontWeight: 400
    lineHeight: 1.45
  label:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 800
    lineHeight: 1.3
  button:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "18px"
    fontWeight: 800
    lineHeight: 1.1
  fine:
    fontFamily: "system-ui, -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.45
rounded:
  tag: "6px"
  sheet: "8px"
  button: "10px"
  round: "50%"
spacing:
  gutter-phone: "16px"
  gutter-wide: "32px"
  peg-grid: "24px"
  control-gap: "12px"
  field-gap: "22px"
  tag-gap: "28px"
  column-gap-wide: "64px"
  section-phone: "64px 16px 72px"
  section-wide: "104px 32px 112px"
components:
  button-primary:
    backgroundColor: "{colors.emergency-red}"
    textColor: "#ffffff"
    typography: "{typography.button}"
    rounded: "{rounded.button}"
    padding: "0 22px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.emergency-red-pressed}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.board-ink}"
    typography: "{typography.button}"
    rounded: "{rounded.button}"
    padding: "0 22px"
    height: "56px"
  button-ghost-hover:
    textColor: "{colors.manila-tag}"
  chip:
    backgroundColor: "{colors.manila-chip}"
    textColor: "{colors.tag-ink}"
    rounded: "{rounded.sheet}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.pegboard}"
    textColor: "{colors.board-ink}"
  input:
    backgroundColor: "{colors.manila-field}"
    textColor: "{colors.tag-ink}"
    rounded: "{rounded.sheet}"
    padding: "12px 14px"
    height: "52px"
  work-order-sheet:
    backgroundColor: "{colors.manila-tag}"
    textColor: "{colors.tag-ink}"
    rounded: "{rounded.sheet}"
    padding: "28px 18px 26px"
  parts-tag:
    backgroundColor: "{colors.manila-tag}"
    textColor: "{colors.tag-ink}"
    typography: "{typography.tag-title}"
    padding: "30px 22px 22px"
  service-row:
    textColor: "{colors.board-ink}"
    typography: "{typography.title}"
    padding: "14px 0"
    height: "76px"
  service-row-arrow-hover:
    backgroundColor: "{colors.emergency-red}"
    rounded: "{rounded.round}"
    size: "48px"
  topbar:
    backgroundColor: "{colors.pegboard-lit}"
    textColor: "{colors.board-ink}"
    padding: "10px 16px"
---

# Design System: 33rd Garage Door Services

## Overview

**Creative North Star: "The Pegboard Wall"**

The page is the back wall of the shop: painted steel-blue pegboard on a strict 24px hole grid, with real door hardware (torsion springs, extension springs, rollers, hinges, lift cables, winding bars) hanging from peg hooks, manila parts tags strung on pegs, and a manila work order pinned up for the estimate. Everything that hangs obeys gravity and can be pushed. One color, emergency-release red, is reserved for the action that gets a homeowner's stuck door fixed: text or call.

The system is phone-first. It is judged at 360 to 430px inside Facebook's in-app browser; wider layouts are the phone layout given room (two columns, a wider rack), never a separate design. Type is a heavy uppercase system sans set tight and large, so the page reads like stencilled shop signage and loads with zero font requests. Density is low: one idea per section, big tap targets (44px minimum, 56px for primary actions), generous section padding.

Motion is physical, never decorative easing. Every moving thing is a damped spring or pendulum driven from one shared animation loop that sleeps when nothing is on screen, and every moving thing renders a still frame under prefers-reduced-motion. The category's stock photo of a smiling tech beside a van is the confirmed anti-reference; the hardware itself is the imagery.

**Key Characteristics:**
- Painted pegboard ground with a real 24px hole grid; hardware snaps to the holes.
- Manila (tags, work order) is the only light surface; it carries all reading-heavy and form content that is not a headline.
- Emergency red appears only on primary actions and their hover/active echoes.
- System sans at weight 800 to 900, uppercase for display and section headlines.
- Pendulum and spring physics, pointer-driven, with still frames for reduced motion.

## Colors

A cool steel-blue workshop wall, one warm paper material, and one alarm red.

### Primary
- **Emergency-Release Red** (emergency-red): the red handle on a garage door's emergency release. Fills the primary button ("Text us a photo", "Text this to us"), fills the service-row arrow on hover/focus/press, colours the torsion-spring winding cone and lift-cable tie in the rack, and the stamped phone number on hover. Pressed/hover state darkens to emergency-red-pressed.

### Secondary
- **Manila Tag** (manila-tag): parts tags, the closing phone-number tag, the estimate work order, text selection, and the focus outline on the dark board. Manila-field and manila-chip are its lighter paper tints for inputs and unselected chips; manila-rule is the brown pencil line that borders every manila control.
- **Tag Ink** (tag-ink) and **Tag Ink Soft** (tag-ink-soft): text on manila; soft for ledes, optional markers and fine print.

### Neutral
- **Pegboard** (pegboard): the default page ground and the selected-chip fill. Also the brand theme-color and favicon tile.
- **Pegboard Deep** (pegboard-deep): alternating section ground (services, our word) so sections read as separate painted panels.
- **Pegboard Lit** (pegboard-lit): header bar, hero top of gradient, closing section; the wall nearest the light.
- **Pegboard Shadow** (pegboard-shadow): the root canvas behind overscroll and the footer.
- **Peg Hole** (peg-hole): the punched holes of the grid.
- **Board Ink** (board-ink) and **Board Ink Soft** (board-ink-soft): text on the board; soft for ledes and supporting copy.
- **Galvanized** (galvanized): ghost-button stroke; at 22% opacity the hairline rules between service rows, at 50% the idle arrow ring.
- **Error Oxide** (error-oxide): inline validation text and invalid-field borders on manila only.

### Named Rules
**The One Handle Rule.** Emergency red marks the action that gets help (text or call) and nothing else. No red headings, no red decoration on the page surface; inside the rack it appears only where real hardware is red.

**The Two Materials Rule.** Surfaces are either painted board (blue family) or manila paper. There is no white card, no grey panel, no third material.

## Typography

**Display Font:** system-ui (with -apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
**Body Font:** the same stack
**Label/Mono Font:** none distinct; numbers use tabular figures

**Character:** One family pushed to its heaviest weights and set uppercase and tight reads as stencilled shop lettering. The system stack is a deliberate house choice under Ellie's pitch-site rules (zero font requests, instant render on cellular inside an in-app browser), not a fallback; do not "upgrade" it to a webfont.

### Hierarchy
- **Display** (900, uppercase, see `display`): the hero headline only.
- **Headline** (900, uppercase, see `headline`): section titles. Balanced wrapping.
- **Statement** (800, sentence case, see `statement`): the one pull-statement in the business's own words; the only headline that is not uppercase, because it is a sentence spoken by the crew.
- **Stamped Number** (900, tabular, see `stamped-number`): the phone number as an object on the closing tag. The number is stamped, not printed small.
- **Title** (800, see `title`): service rows; each row is a full-width tap target.
- **Tag Title** (900, uppercase, see `tag-title`): step names on parts tags, with the step numeral in pegboard blue.
- **Body** (400, 17px, 1.55): running copy, capped at 44 to 52ch for ledes.
- **Lede** (400, fluid 17 to 20px): the hero promise, capped at 30ch.
- **Label** (800, 16px): form legends and field labels on the work order.
- **Button** (800, 18px): all buttons.
- **Fine** (15px): form fine print, errors, link-buttons.

### Named Rules
**The Shop Lettering Rule.** Headlines are weight 900, uppercase, negative tracking (-0.02 to -0.025em), line-height under 1. Body never goes below 15px; phone-first body is 17px.

**The Tabular Number Rule.** Every phone number (header, closing tag, footer) uses tabular figures and never wraps.

## Layout

Single column on phones with a 16px gutter; content max-width 1120px (header 1184px). Sections are full-bleed painted panels with 64px top / 72px bottom padding on phones and 104 / 112px from 1024px.

Breakpoints: below 380px the header tightens (phone icon drops, wordmark shrinks); 640px puts paired actions side by side, lays tags out in three columns and widens the work order padding; 1024px turns the hero into a copy column plus a rack column filling the rest of the viewport, and splits sections into asymmetric two-column grids (5/7 services, 7/5 statement, 4/7 estimate with a sticky heading), 56 to 64px column gaps.

**The Hole Grid Rule.** The pegboard grid is 24px (`--grid`). Hanging hardware snaps its hook to a hole centre; anything that hangs on the board lands on the grid. In the hero, the hole pattern is masked out behind the copy (measured live as `--copy-h` / `--copy-w`) so text never sits on holes.

**The Seam Rule.** Sections never meet at a bare edge. Each boundary is a 56px stretched extension spring overlapping both panels by 28px, its canvas painting the upper panel colour above the midline and the lower below.

## Elevation & Depth

Depth is literal: things hang off the board and cast soft shadows down and to the right, as if lit from upper left. Shadows are always blurred, warm-free navy (rgba 4,16,26), never hard offsets. Page panels themselves are flat and differ only by tone (deep / base / lit).

### Shadow Vocabulary
- **Hanging part** (offset 7px 11px, blur 9px, 42% navy): every hardware part in the rack, drawn from the part's own silhouette.
- **Parts tag** (`filter: drop-shadow(5px 9px 7px rgba(4,16,26,.45))`): follows the tag's clipped silhouette.
- **Pinned sheet** (`box-shadow: 0 18px 30px -14px rgba(4,16,26,.65)`): the work order hanging away from the board.
- **Peg head** (`box-shadow: 0 2px 3px rgba(0,0,0,.45)`): the small steel pegs holding tags and the sheet.
- **Primary button lift** (`box-shadow: 0 6px 16px -6px rgba(5,15,25,.6)`): the red button only.
- **Spring seam** (stroke shadow offset 5px 8px, 35% navy).

**The Upper-Left Light Rule.** All cast shadows fall down and to the right. A new hanging object gets a blurred down-right shadow; nothing floats with a centred glow.

## Shapes

Mostly gently rounded rectangles: 6px on tag tops, 8px on the sheet, chips and fields, 10px on buttons; full circles for pegs, peg holes, the arrow ring and tag eyelets. The parts tag is the signature silhouette: a manila rectangle with the top corners clipped at 18% / 14px into a classic shipping-tag shoulder, a punched eyelet showing the board through it, hung by a string from a steel peg. Steel is rendered with linear gradient "bands" across the part (galvanized: light centre; oil-tempered: near-black with a blue sheen).

## Components

### Buttons
Big, blunt, and thumb-sized.
- **Shape:** gently rounded (10px), 2px border, minimum 56px tall.
- **Primary:** emergency red fill and border, white text, SVG line icon at 20px leading the label, primary lift shadow. Hover darkens to the pressed red.
- **Ghost:** transparent with a 2px galvanized stroke and board-ink text; on hover-capable devices the stroke and text turn manila.
- **Press:** every button nudges down 1px on active.
- **Focus:** 3px manila outline, 3px offset, on the board; 3px pegboard-blue outline on manila.
- **Pairing:** stacked full width on phones, side by side from 640px, primary first.

### Chips
- **Style:** paper-tint fill, 2px manila-rule border, 8px radius, 46px tall, weight 700. They are radio buttons for "What's going on?" and "How soon?".
- **State:** selected chips fill pegboard blue with board-ink text, as if the option were painted onto the board. Invalid groups turn chip borders error-oxide.

### Cards / Containers
- **Work order sheet:** manila, 8px radius, two steel pegs pinning its top corners, pinned-sheet shadow, max 720px. Padding grows to 36px from 640px.
- **Parts tag:** see Shapes; 30px 22px 22px padding, the step numeral in pegboard blue before the uppercase title. Used for process steps and for the closing phone number.

### Inputs / Fields
- **Style:** lighter paper fill, 2px manila-rule border, 8px radius, 52px minimum height (textarea 104px), 17px text.
- **Focus:** 3px pegboard-blue outline, 1px offset.
- **Error:** border turns error-oxide and an inline sentence appears below in bold error-oxide; the first invalid field scrolls into view and takes focus.

### Navigation
A single header bar on pegboard-lit: the "33rd" wordmark (weight 900, superscript "rd") beside a two-line uppercase "Garage Door Services" mark on the left, the phone number with a line phone icon on the right. No menu; the page is one scroll.

### Service Rows
Whole-row links separated by galvanized hairlines, 76px minimum. Only the circular arrow reacts: its ring fills emergency red on hover, focus and press. Each row opens a pre-filled text.

### Hero Rack (signature)
A canvas of door hardware hanging on peg hooks snapped to the hole grid: five parts on phones, ten on wide screens. Each part is a damped pendulum (gravity 1500, damping 1.1) with a low three-frequency wind drift. The pointer pushes parts it passes (push radius 64px); a press on a part grabs it (stiffness 260, damping 22) so it can be dragged and flicked, and the extension spring stretches under the grab and recoils (spring k 90). On touch, a finger on empty board scrolls the page; only a finger on a part holds it. Device pixel ratio is capped at 1.5.

### Spring Seams (signature)
Galvanized extension springs strung hook-to-hook across each section boundary, simulated as a damped string (tension 2600, damping 1.6) with a slow two-wave swell in the coil spacing. A pointer or a finger whose page scrolls under it plucks the coils it crosses.

### Swaying Tags (signature)
Parts tags hang from their peg and sway a few hundredths of a radian (max 0.06 rad) on a spring (k 30, damping 3.4). A tap swings them away from the tap side; a horizontal swipe across pushes them.

### Motion Grammar
One shared requestAnimationFrame loop drives every system; each system runs only while intersecting the viewport (80px margin) and the loop stops when none are visible. Under prefers-reduced-motion the loop never starts: each system draws one still frame (redrawn on resize), grab is disabled, the rack returns touch to the page, and smooth scrolling is off. CSS transitions are limited to colour changes (0.15 to 0.2s) and the 1px button press (0.1s).

## Do's and Don'ts

### Do:
- **Do** hang new content on the board: manila for anything the visitor reads closely or fills in, steel for imagery.
- **Do** snap anything that hangs to the 24px hole grid and give it a blurred down-right shadow.
- **Do** separate sections with a spring seam whose top and bottom colours match the neighbouring panels.
- **Do** keep primary actions emergency red, 56px tall, icon-led, and stacked full width on phones.
- **Do** give every moving element a physical model (pendulum or spring) on the shared loop, and a still frame under prefers-reduced-motion.
- **Do** keep the system font stack and weights 800 to 900 for headings.

### Don't:
- **Don't** use emergency red for headings, decoration or non-action elements.
- **Don't** introduce stock photography, illustrated people or vans; the hardware is the imagery.
- **Don't** add a white or grey card material; surfaces are board or manila.
- **Don't** let a touch on empty board capture the scroll; only a touch on hardware may hold it.
- **Don't** animate with keyframe tweens or easing curves for the world's motion; only state colour changes use CSS transitions.
- **Don't** load a webfont.
