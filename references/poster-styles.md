# Poster Style Specifications

Reference file for `career-planning/SKILL.md`. Use these design specs when generating the
final career poster. Both styles use the same content sections and layout structure — only
the visual language changes. Canonical labels are English. If the conversation is conducted in
Chinese, translate labels and placeholder wording naturally into Chinese while preserving the same
structure.

---

## Shared Layout Structure

All posters follow this top-to-bottom section order:

1. Header (name, direction + motivation badge, eyebrow)
2. Divider
3. Core Assets — 3-column sub-cards (Transferable Skills | Background Combination Advantage | Blind Spots)
4. Divider
5. Direction Profile — full-width 2-column grid
6. Divider
7. My Story (6-node narrative, 3×2 grid)
8. Divider
9. Gap Analysis (3-column grid, each item has priority badge + depth sub-label)
10. Divider
11. Current Recommendation banner (full-width)
12. Two-column row: Next Steps | Success Signal
13. Version bar (footer)

## Layout Quality Rules

Generated posters must render cleanly when opened directly in a browser. The HTML must not rely on
a fixed desktop viewport.

- Center the poster on the page and prevent horizontal clipping. Use a responsive poster width such
  as `width: min(760px, calc(100vw - 32px))` or an equivalent rule.
- Use `grid-template-columns: repeat(3, minmax(0, 1fr))` for 3-column sections and `minmax(0, 1fr)`
  for 2-column sections so long content does not force the grid wider than the poster.
- Add responsive fallbacks: on narrow screens, stack 3-column sections into one column and 2-column
  sections into one column rather than letting the poster overflow.
- Avoid extremely narrow cards that cause Chinese text to break into one character per line. If a
  card contains longer Chinese placeholder text, make that card wider, stack the section, or use a
  block-level placeholder.
- Allow long labels and badges to wrap gracefully. Avoid `white-space: nowrap` on recommendation
  titles, footer badges, and long field values unless the container is guaranteed to fit.
- Use `overflow-wrap: break-word` for user-generated text and field values. Do not use aggressive
  word breaking on normal body text unless needed for a long URL-like token.
- Do not crop meaningful content with `overflow: hidden`. Decorative elements may be clipped, but
  text, badges, cards, and section content must remain fully visible.
- Prefer thin outline circles or partial line accents for the top-right decoration. Avoid large
  filled blobs that compete with the content or violate the restrained poster style.

## Content-Adaptive Layout Rules

The poster layout must adapt to the amount of confirmed user content.

- Let the poster height grow naturally when content is longer than expected.
- Never hide, crop, or visually truncate confirmed content to preserve a fixed poster height.
- If a 3-column section becomes crowded, switch that section to 2 columns or 1 column.
- If a card contains long text, allow the card to grow vertically and use readable line lengths.
- If pill lists become too dense, convert pills into a compact vertical list while preserving color coding.
- For story nodes, distill long content into concise 1-3 sentence summaries grounded in the confirmed conversation.
- For gap lists and next steps, preserve priority order and combine repeated points when appropriate.
- Do not reduce body text below readable size just to fit more content.
- The hierarchy is more important than fixed symmetry: preserve clarity first, then visual balance.

---

## Style 1: Clean Modern

**Personality:** Professional, refined, timeless. Something you'd share with a mentor.

**Palette:**
- Background: `#FAFAF7`
- Border: `0.5px solid #E2DED6`
- Dividers: `#E2DED6`
- Primary text: `#1A1A18`
- Secondary text: `#5F5E5A`
- Muted text / labels: `#B4B2A9` / `#888780`
- Accent (dots, arrows, action numbers): `#2C2C2A`
- Tag background: `#EFECEA`
- Narrative block background: `#F2EDE6`
- Success block background: `#EFECEA`
- Gap cards: transparent with `0.5px solid #E2DED6` border
- Gap badge — Must fix: bg `#F5C4B3`, text `#712B13`
- Gap badge — Bonus: bg `#C0DD97`, text `#27500A`
- Gap badge — Later: bg `#D3D1C7`, text `#444441`
- Version badge dark: bg `#2C2C2A`, text `#FAFAF7`
- Version badge light: bg `#EFECEA`, text `#888780`

**Typography:**
- Name: Lora serif, 26–30px, weight 400
- Eyebrow / labels: DM Sans, 9px, uppercase, letter-spacing 0.16–0.18em
- Body / tags / nodes: DM Sans, 10–12px
- Direction text: DM Sans, 12–13px

**Motivation badge (header):**
- Pull: bg `#D8EDEC`, text `#2E6A68`
- Push: bg `#F0DDD8`, text `#7A3A28`
- Exploratory: bg `#E5E3F0`, text `#4A3880`
- Pill shape: `border-radius: 24px`, `font-size: 11px`, `font-weight: 600`

**Core Assets sub-card colors:**
- Transferable Skills: section label + tag fill color `#4A8886` (teal), tags white text
- Background Combination Advantage: section label + tag fill color `#7868A0` (purple), tags white text
- Blind Spots: section label color `#957830` (amber), tags: transparent bg, `1.5px dashed #C4A850` border, italic text in `#957830`

**Decision urgency badge (Direction Profile row):**
- Near-term Decision: bg `#F5C4B3`, text `#6E2410`
- Medium-term Planning: bg `#BFD98F`, text `#265008`
- Long-term Direction: bg `#C8D4E8`, text `#2A3A60`
- Shape: `border-radius: 10px`, `font-size: 10px`, `font-weight: 600`, `padding: 2px 9px`


**Gap depth sub-label:**
- Rendered beneath gap item text, `font-size: 9px`, italic, `color: #B4B2A9` (muted)
- Values: Missing Entirely / Present but Not Deep Enough

**Gap badge — Build Later:** bg `#D3D1C7`, text `#444441`

**Current Recommendation banner:**
- Full-width block, `border-radius: 10px`, `padding: 14–16px 20–22px`
- Left side: small uppercase label "Current Recommendation" + large recommendation title (17–18px, bold, white)
- Vertical divider line: `1px`, `rgba(255,255,255,0.28)`, `height: 38px`
- Right side: one-sentence rationale, `font-size: 11px`, `color: rgba(255,255,255,0.88)`
- Banner color by recommendation state:
  - Act Now: `#4A8886` (teal)
  - Lay Groundwork: `#7868A0` (purple)
  - Wait: `#886855` (brown)

**Decorative elements:**
- Two concentric circle outlines (border only, no fill) positioned top-right, partially clipped
- Thin horizontal rule as bottom border accent (3px solid `#2C2C2A`)
- Arrow motif: thin line + triangle tip in `#2C2C2A`
- Node dots: filled circle `#2C2C2A`, connector lines `#D3D1C7`
- Border radius: 12px on poster, 8px on narrative block, 6px on gap cards / success block

---

## Style 2: Clean Modern Dark

**Personality:** Same professional restraint as Clean Modern, shifted to a cool near-black. Feels like the same poster at night.

**Palette:**
- Background: `#18181A`
- Border: `0.5px solid #2C2C30`
- Dividers: `#2C2C30`
- Primary text: `#E8E8E4`
- Secondary text: `#9E9E9A`
- Muted text / labels: `#7A7A7E` / `#686868`
- Accent (dots, arrows, action numbers): `#E8E8E4`
- Tag background: `#242428`, text `#9E9E9A`
- Narrative block background: `#1E1E22`
- Success block background: `#1E1E22`
- Gap cards: transparent with `0.5px solid #2C2C30` border
- Gap badge — Must fix: bg `#4A1B0C`, text `#F5C4B3`
- Gap badge — Bonus: bg `#173404`, text `#C0DD97`
- Gap badge — Later: bg `#242428`, text `#9E9E9A`
- Version badge dark: bg `#E8E8E4`, text `#18181A`
- Version badge light: bg `#242428`, text `#7A7A7E`

**Typography:** Same as Clean Modern light (Lora + DM Sans)

**Motivation badge (dark variants):**
- Pull: bg `#1A3230`, text `#5BBAB8`
- Push: bg `#2E1A16`, text `#C47060`
- Exploratory: bg `#242038`, text `#9888C8`

**Core Assets sub-card colors (dark):**
- Transferable Skills: section label + tag fill `#3A7876` (dark teal), tags use lighter teal text on dark bg
- Background Combination Advantage: section label + tag fill `#5A4880` (dark purple)
- Blind Spots: section label `#7A6020`, tags: `1.5px dashed #7A6020` border, italic text `#9A8040`

**Decision urgency badge (dark):**
- Near-term Decision: bg `#4A1B0C`, text `#F5C4B3`
- Medium-term Planning: bg `#173404`, text `#C0DD97`
- Long-term Direction: bg `#1A2A3A`, text `#8AB0D0`


**Gap depth sub-label (dark):** `color: #555558`, italic

For dark posters, keep secondary labels readable. Avoid using muted label colors so dark that they
disappear against the background; small labels should remain legible at normal browser zoom.

**Gap badge — Build Later (dark):** bg `#242428`, text `#9E9E9A`

**Current Recommendation banner (dark):**
- Act Now: `#2A5A58`
- Lay Groundwork: `#3A2A60`
- Wait: `#3A2A1A`
- Rationale text: `rgba(255,255,255,0.80)`

**Decorative elements:**
- Same two circle outlines as light version, using `#2C2C30` border
- Bottom accent line: `3px solid #E8E8E4`
- Node dots: `#E8E8E4`, connector lines: `#2C2C30`
- Action number circles: bg `#E8E8E4`, text `#18181A`

---

## Footnote Style (perception-based data disclaimer)

When a footnote is required beneath the Gap Analysis section (Stage 6 data was perception-based only), render it as follows for each style:

| Style | Font size | Color | Style |
|---|---|---|---|
| Clean Modern | 8px | `#B4B2A9` | DM Sans, normal weight, italic |
| Clean Modern Dark | 8px | `#555558` | DM Sans, normal weight, italic |

Add `margin-top: 8px` between the last gap card and the footnote. No border or background — plain text only.

---

## Missing Information Placeholder

When a section or field has no content (see SKILL.md for which cases trigger this), render a placeholder component instead of a dash or blank space.

**Clean Modern (light):**
- Background: `#FDF6E8`
- Border: `1px dashed #D4A830`
- Border radius: `8px`
- Padding: `10px 13px`
- Icon prefix: `○` in `#C49820`, `font-size: 11px`
- Message text: DM Sans, `10.5px`, italic, `color: #8A7020`, `line-height: 1.5`
- Used for: block-level replacements (timeline, success signal, full card sections)
- For inline field replacements (e.g. a single profile row value): omit the box, render just the italic message text in `#C49820`, `font-size: 10px`

**Clean Modern Dark:**
- Background: `#252010`
- Border: `1px dashed #6A5420`
- Border radius: `8px`
- Padding: `10px 13px`
- Icon prefix: `○` in `#8A7030`
- Message text: DM Sans, `10.5px`, italic, `color: #8A7840`, `line-height: 1.5`
- Inline field color: `#7A6830`

**Wording guidelines:**
- Keep messages short (1–2 lines max)
- Always name the stage that would supply the missing content
- Tone: neutral and instructive, not apologetic

---

## Implementation Notes

- Generate as a self-contained local HTML file, not an inline chat artifact and not a PNG by default
- Save each generated poster under `career-planning-posters/<session-slug>/` in the user's current workspace; keep all versions from the same planning conversation in that folder
- If no writable workspace is available, ask the user where to save the file, or use the nearest available writable working directory and report the exact path
- Keep all CSS inline in the HTML file. The file should be self-contained except for optional Google Fonts imports.
- Use optional `@import` from Google Fonts for Lora and DM Sans, but always define robust fallback fonts so the poster remains readable offline.
- Poster padding: `40–48px` vertical, `44–52px` horizontal
- Section label size: `9px`, `letter-spacing: 0.16em`, `text-transform: uppercase`
- Gap analysis: always 3-column grid, one card per gap category
- Version bar: left = framework credit, right = user category badge + version + date
- All content is populated from the user's actual conversation — never fabricate or use dashes for missing content; use the placeholder component instead
- Node text should be concise (2–3 lines max per node) — distill from Stage 8, don't paste verbatim
