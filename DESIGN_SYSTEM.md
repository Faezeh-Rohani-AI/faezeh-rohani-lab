# Faezeh Rohani Portfolio Design System

## Design Direction

The portfolio uses a classic academic style: formal, calm, readable, and professional. The visual system is intentionally restrained, using only white and blue tones.

## Color Palette

| Token | Value | Usage |
| --- | --- | --- |
| `--navy` | `#0a2540` | Primary brand color, headings, footer, primary buttons |
| `--navy-soft` | `#163a5c` | Secondary headings, emphasized body text, button hover |
| `--ink` | `#0a2540` | Main text color |
| `--muted` | `#42627f` | Supporting text, captions, navigation links |
| `--line` | `#dbe8f4` | Borders and section dividers |
| `--bg` | `#ffffff` | Page background |
| `--card` | `#ffffff` | Cards and content panels |
| `--accent` | `#0a2540` | Eyebrow labels and list bullets |
| `--accent-soft` | `#eef6ff` | Soft hover states, tags, hero tint |

Allowed colors: white, deep blue, medium blue, muted blue, and pale blue only.

## Typography

### Serif

`Georgia, "Times New Roman", serif`

Used for:

- Site brand
- Main hero name
- Section headings
- Card headings

### Sans Serif

`Arial, Helvetica, sans-serif`

Used for:

- Body copy
- Navigation
- Buttons
- Lists
- Contact details

## Layout

### Container

The main container is:

```css
width: min(1160px, calc(100% - 40px));
margin: 0 auto;
```

This keeps the layout centered and readable on large screens while preserving side spacing on smaller screens.

### Header

The hero uses a two-column layout:

- Left: name, academic title, affiliation, and contact buttons
- Right: portrait card with professional summary

The hero background is white with a subtle pale-blue academic grid and a pale-blue vertical tint.

### Sections

Sections use generous vertical spacing, thin blue dividers, and clear section titles. Content is grouped into white cards with blue borders.

## Components

### Top Navigation

Sticky top navigation with:

- White translucent background
- Blue border divider
- Serif brand text
- Uppercase blue navigation links

### Buttons

Primary button:

- Navy background
- White text
- Navy border

Secondary buttons:

- White background
- Navy text
- Navy border

Hover state:

- Pale blue for secondary buttons
- Softer navy for primary buttons

### Portrait Card

The portrait card includes:

- White background
- Thin pale-blue border
- Subtle blue shadow
- 3:2 image ratio
- Muted blue caption text

Image path:

```text
assets/faezeh-rohani.jpg
```

### Fact Strip

The quick facts are presented as a single bordered strip divided into four columns. On smaller screens, each fact stacks vertically with blue dividers.

### Cards

Cards use:

- White background
- Pale-blue border
- 4px radius
- No heavy shadow

Cards are used for academic content blocks, publications, skills, certifications, and contact details.

### Tags

Research tags use:

- Pale-blue background
- Navy text
- 4px radius
- Bold text

### Lists

Custom lists use small navy circular bullets. This keeps long CV-style content structured without visually overwhelming the page.

### Contact Items

Contact items are card-like links with:

- White background
- Pale-blue border
- Muted blue labels
- Navy values

LinkedIn is a clickable text link without an icon.

## Responsive Behavior

At widths below `920px`:

- Hero becomes one column
- Fact strip stacks vertically
- Two-column and three-column grids become one column
- Contact grid becomes one column

At widths below `680px`:

- Top navigation becomes non-sticky
- Navigation stacks under the brand
- Container side spacing becomes tighter
- Card padding is reduced

## Content Rules

- Use formal academic language.
- Keep headings concise.
- Prefer full institution names.
- Use "PhD" consistently in metadata and brand areas.
- Use "Üsküdar University" and "Türkiye" with correct spelling.
- Keep publication entries readable and grouped in selected lists.

## Accessibility Notes

- The portrait has descriptive alt text.
- Navigation uses an `aria-label`.
- Links use readable text labels.
- Color contrast is maintained through deep navy text on white or pale-blue backgrounds.
