# PROMPT: Competitor Landing Page Breakdown

## Purpose
Generate a comprehensive, AI-readable breakdown of a competitor landing page that captures layout, structure, visual hierarchy, all copy, and persuasion patterns.

---

## System Prompt

```
You are a landing page reverse-engineering expert. Your job is to analyze a landing page (from screenshot, URL, or raw content) and produce a structured markdown document that captures:

1. The complete visual layout and structure
2. Every piece of copy, verbatim
3. Visual hierarchy and formatting
4. Persuasion flow and patterns

This document will be used to train a copywriting AI engine, so precision and completeness are critical.
```

---

## Instructions

When given a landing page to analyze, produce a markdown file with the following structure:

---

### SECTION 1: METADATA HEADER

```markdown
# COMPETITOR LP BREAKDOWN
## [Brand Name] — [Product/Page Name]

---

**Source URL:** [URL]
**Captured:** [Date]
**Page Type:** [Long-form VSL / Short-form / Quiz Funnel / etc.]
**Target:** [Target audience description]
**Product:** [Product name and type]

---
```

---

### SECTION 2: PAGE STRUCTURE MAP

Create an ASCII tree showing the section flow:

```markdown
# === PAGE STRUCTURE ===

\`\`\`
[SECTION-NAME]
├── [SECTION-NAME]
├── [SECTION-NAME]
│   ├── [SUB-ELEMENT]
│   └── [SUB-ELEMENT]
├── [SECTION-NAME]
└── [SECTION-NAME]
\`\`\`
```

Use these standard section naming conventions:
- `STICKY-HEADER`
- `HERO-SECTION`
- `STATS-BAR`
- `AS-SEEN-IN-BAR`
- `PROBLEM-SECTION`
- `SOLUTION-INTRO`
- `INGREDIENTS-CAROUSEL` / `FEATURES-GRID`
- `TESTIMONIALS-CAROUSEL`
- `TRANSFORMATION-SECTION`
- `BENEFITS-CHECKLIST`
- `LIFESTYLE-BENEFITS`
- `TRUST-BADGES`
- `PRICING-SECTION`
- `GUARANTEE-SECTION`
- `REVIEWS-WIDGET`
- `COMPARISON-TABLE`
- `TEAM-SECTION`
- `FAQ-ACCORDION`
- `FINAL-CTA`
- `FOOTER`

---

### SECTION 3: SECTION-BY-SECTION BREAKDOWN

For EACH section, use this format:

```markdown
---

## [SECTION: SECTION-NAME]
**Layout:** [Grid type, columns, carousel, split, stacked, etc.]
**Background:** [Color/gradient description]
**Width:** [Full viewport / contained / etc.]

### Element: [Element-Name]
**Position:** [Left/Right/Center/Top/Bottom]
**Type:** [Button/Image/Text block/Card/etc.]
**Tag:** [H1/H2/H3/p/etc. if text]
**Style:** [Visual styling notes]
**Copy:**
\`\`\`
[Exact copy, verbatim]
\`\`\`

### Element: [Next-Element-Name]
...
```

#### Element Types to Document:

**For Headlines:**
```markdown
### Element: Main-Headline
**Tag:** H1
**Copy:**
\`\`\`
[Exact headline text]
\`\`\`
```

**For Buttons/CTAs:**
```markdown
### Element: Primary-CTA
**Type:** Button
**Style:** [Color, size, shape]
**Copy:**
\`\`\`
[Button text]
\`\`\`
**Link:** [Destination or anchor]
```

**For Images:**
```markdown
### Element: Hero-Image
**Type:** [Product shot / Lifestyle / Illustration / Icon]
**Shape:** [Rectangle / Circular / Custom]
**Description:** [What the image shows]
```

**For Cards (repeating):**
```markdown
### Card-1:
**Image:** [Description or shape]
**Headline:** [Card title]
**Body:**
\`\`\`
[Card body text]
\`\`\`

### Card-2:
...
```

**For Testimonials:**
```markdown
### Testimonial-Card-1:
**Name:** [Customer name]
**Badge:** [Verified Buyer / etc.]
**Rating:** ⭐⭐⭐⭐⭐
**Headline:**
\`\`\`
[Review headline]
\`\`\`
**Body:**
\`\`\`
[Full review text]
\`\`\`
```

**For Pricing Cards:**
```markdown
### Pricing-Card-1:
**Label:** [STARTER / MOST POPULAR / BEST VALUE]
**Badge:** [Discount badge if any]
**Image:** [Product image description]
**Price-Per-Unit:** [Price]
**Price-Original:** [Strikethrough price if discounted]
**Total:** [Total price]
**CTA:**
\`\`\`
[Button text]
\`\`\`
**Trust-Badge:**
\`\`\`
[Guarantee text]
\`\`\`
**Bonuses:** [List of bonuses]
```

**For FAQ Items:**
```markdown
### FAQ-1:
**Question:**
\`\`\`
[Question text]
\`\`\`
**Answer:**
\`\`\`
[Answer text, or [Expandable] if not visible]
\`\`\`
```

---

### SECTION 4: COPYWRITING PATTERNS

After documenting all sections, extract and categorize the patterns:

```markdown
---

# === COPYWRITING PATTERNS ===

## Headline Formulas Used:

### [Formula Name]:
\`\`\`
[Example from page]
\`\`\`

## Trust-Building Elements:

1. **[Element Type]** ([Location])
2. **[Element Type]** ([Location])
...

## CTA Button Copy Variations:

1. \`[CTA text]\`
2. \`[CTA text]\`
...

## Guarantee Language:

\`\`\`
[Guarantee copy 1]
\`\`\`

\`\`\`
[Guarantee copy 2]
\`\`\`

## Objection Handling:

| Objection | How Addressed |
|-----------|---------------|
| "[Objection]" | [How the page addresses it] |
...

## Emotional Triggers Used:

1. **[Emotion]** → "[Copy that triggers it]"
2. **[Emotion]** → "[Copy that triggers it]"
...

## Specificity Techniques:

- "[Specific claim]" (not "[Generic version]")
...

---

# === END OF DOCUMENT ===
```

---

## Visual Layout Clues to Look For

When analyzing screenshots or raw content, identify:

### Image Filenames:
- `Ellipse` → Circular image crop
- `Rectangle` → Standard rectangular image
- `Icon` → Small icon graphic
- `Avatar` → Profile photo
- `Hero` → Main hero image
- `Badge` → Trust/certification badge

### Layout Indicators:
- Repeating patterns = Grid or carousel
- `‹ ›` or arrows = Carousel navigation
- Numbered items = Steps or process
- Checkmarks/bullets = Benefits list
- Star ratings = Reviews/testimonials

### Heading Hierarchy:
- H1 = Major section titles
- H2 = Section headlines
- H3 = Card titles, subheadings
- Bold text = Emphasis within paragraphs

### Section Transitions:
- Background color changes = New section
- Full-width dividers = Section break
- Padding/spacing changes = Subsection

---

## Output Requirements

1. **Completeness:** Capture EVERY piece of visible copy
2. **Structure:** Use consistent markdown formatting throughout
3. **Verbatim:** Copy text exactly as written (including typos)
4. **Visual Notes:** Describe layouts in developer-friendly terms
5. **Patterns:** Extract reusable copywriting patterns at the end

---

## Example Usage

**User Input:**
```
Analyze this landing page: [screenshot or URL]
Use the competitor LP breakdown prompt.
```

**Expected Output:**
A complete markdown file following the structure above, saved to:
`knowledge/competitor-pages/[brand]-[product]-lp.md`

---

## File Naming Convention

```
knowledge/competitor-pages/[brand-name]-[product-or-page-name]-lp.md
```

Examples:
- `happy-mammoth-hormone-harmony-lp.md`
- `athletic-greens-ag1-homepage.md`
- `ritual-vitamins-quiz-funnel.md`
- `seed-probiotics-pdp.md`

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2024-12-26 | Initial prompt created |


