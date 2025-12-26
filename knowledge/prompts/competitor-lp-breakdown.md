# PROMPT: Competitor Landing Page Breakdown

## Purpose
Convert a landing page (screenshot, URL, or raw content) into a structured, AI-readable markdown document. Pure data capture — no analysis, no strategy extraction. Just the raw information in text form.

---

## System Prompt

```
You are converting a landing page into structured text. Your job is to document EXACTLY what exists on the page:

1. The visual layout and structure
2. Every piece of copy, verbatim
3. Visual hierarchy and formatting
4. Element types and positions

DO NOT analyze, interpret, or extract patterns. Just document what you see — as if you're converting a screenshot into text that another AI can read.

Document what EXISTS. Adapt to whatever structure the page has.
```

---

## Output Structure

### PART 1: Metadata

```markdown
# PAGE CAPTURE
## [Brand Name] — [Page Name]

---

**Source URL:** [URL if available]
**Captured:** [Date]
**Page Type:** [What kind of page is this]

---
```

---

### PART 2: Page Structure Map

```markdown
# === PAGE STRUCTURE ===

\`\`\`
[List sections in order as they appear on the page]
\`\`\`
```

Name sections based on what they contain. Examples:
- `LOGO-AND-NAV-BAR`
- `HEADLINE-WITH-VIDEO`
- `THREE-COLUMN-STATS`
- `PRODUCT-IMAGE-GRID`
- `TESTIMONIAL-SLIDER`
- `PRICING-CARDS`
- `FORM-WITH-FIELDS`

---

### PART 3: Section-by-Section Documentation

For each section:

```markdown
---

## [SECTION: Name]
**Layout:** [How elements are arranged]
**Background:** [Color/style]

### Element: [Name]
**Type:** [What kind of element]
**Position:** [Where in the section]
**Copy:**
\`\`\`
[Exact text]
\`\`\`
```

---

## Element Documentation

### Text:
```markdown
### Element: [Name]
**Type:** Headline / Subhead / Body / Caption / Label
**Tag:** H1 / H2 / H3 / p
**Copy:**
\`\`\`
[Exact text verbatim]
\`\`\`
```

### Buttons/Links:
```markdown
### Element: [Name]
**Type:** Button / Text Link
**Style:** [Color, size if notable]
**Copy:**
\`\`\`
[Button text]
\`\`\`
**Links to:** [Destination if visible]
```

### Images:
```markdown
### Element: [Name]
**Type:** Photo / Icon / Illustration / Logo
**Shape:** Rectangle / Circle / Custom
**Shows:** [What the image depicts]
```

### Repeating Items (Cards, List Items, Grid Items):
```markdown
### Pattern: [Name]
**Count:** [Number of items]
**Layout:** [Grid / Carousel / List]

### Item 1:
**Image:** [Description]
**Headline:** [Text]
**Body:** [Text]

### Item 2:
...
```

### Forms:
```markdown
### Element: Form
**Fields:**
- [Field 1 label] ([type])
- [Field 2 label] ([type])
**Submit Button:**
\`\`\`
[Button text]
\`\`\`
```

### Video:
```markdown
### Element: Video
**Type:** Embedded / Background / Autoplay
**Thumbnail:** [Description if visible]
**Duration:** [If shown]
```

---

## Visual Clues from Raw Data

### Image Filenames:
| Contains | Means |
|----------|-------|
| `ellipse`, `circle` | Circular image |
| `icon` | Small icon |
| `badge`, `seal` | Trust badge |
| `logo` | Brand logo |
| `hero`, `banner` | Large featured image |
| `avatar` | Person photo |

### Content Patterns:
| Pattern | Means |
|---------|-------|
| Same structure 3+ times | Grid or carousel |
| `‹ ›` arrows | Carousel navigation |
| ⭐ stars | Rating display |
| ✓ checkmarks | List items |
| Numbers (1, 2, 3) | Steps/process |
| $ or £ prices | Pricing area |

### Heading Levels:
| Level | Typically |
|-------|-----------|
| H1 | Main page title |
| H2 | Section headers |
| H3 | Card titles, subheads |

---

## Quality Check

Before finishing:

- [ ] Sections are in page order (top to bottom)
- [ ] All visible copy is captured verbatim
- [ ] Layouts are described (columns, grids, etc.)
- [ ] Element types are noted
- [ ] Repeating patterns are documented with all instances

---

## File Naming

```
knowledge/competitor-pages/[brand]-[page-name].md
```

---

## Usage

```
Read the prompt at knowledge/prompts/competitor-lp-breakdown.md

Capture this page: [screenshot / URL / content]
```

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2024-12-26 | Initial prompt |
| 2.0 | 2024-12-26 | Made principle-based |
| 3.0 | 2024-12-26 | Stripped to pure data capture only — no analysis |

