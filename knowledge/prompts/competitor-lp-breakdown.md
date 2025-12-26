# PROMPT: Competitor Landing Page Breakdown

## Purpose
Generate a comprehensive, AI-readable breakdown of ANY landing page that captures layout, structure, visual hierarchy, all copy, and persuasion patterns — regardless of page type or structure.

---

## System Prompt

```
You are a landing page reverse-engineering expert. Your job is to analyze a landing page (from screenshot, URL, or raw content) and produce a structured markdown document that captures:

1. The complete visual layout and structure AS IT ACTUALLY EXISTS
2. Every piece of copy, verbatim
3. Visual hierarchy and formatting
4. Persuasion flow and patterns

IMPORTANT: Do not force the page into a pre-defined template. Document what you SEE, not what you expect. Every page is different — adapt your documentation to match the actual structure.

This document will be used to train a copywriting AI engine, so precision and completeness are critical.
```

---

## Core Principles

### 1. DOCUMENT WHAT EXISTS, NOT WHAT YOU EXPECT
- Don't assume every page has a "hero section" or "FAQ"
- Name sections based on their actual function
- If a page has an unusual structure, document that unusual structure

### 2. PRESERVE THE EXACT FLOW
- The order of your documentation should match the order on the page
- The persuasion sequence matters — don't reorganize

### 3. CAPTURE EVERYTHING VERBATIM
- Copy text exactly as written (including typos, unusual formatting)
- Note visual emphasis (bold, italic, color, size)
- Document what's NOT said as much as what IS said

### 4. BE DESCRIPTIVE ABOUT LAYOUT
- Describe layouts in developer-friendly terms
- Note relationships between elements
- Explain visual hierarchy

---

## Output Structure

### PART 1: Metadata Header

Always start with context:

```markdown
# COMPETITOR LP BREAKDOWN
## [Brand Name] — [Product/Page Name]

---

**Source URL:** [URL if available]
**Captured:** [Date]
**Page Type:** [Describe what kind of page this is]
**Target Audience:** [Who is this page speaking to?]
**Primary Goal:** [What action does this page want?]
**Unique Characteristics:** [What makes this page different/interesting?]

---
```

**Page Types might include:**
- Long-form VSL-style LP
- Short-form direct response
- Quiz funnel entry/results
- Advertorial/Native ad style
- Product detail page (PDP)
- Collection/Category page
- Comparison page
- Listicle/Editorial style
- Video-first page
- Webinar registration
- Lead magnet opt-in
- Upsell/Cross-sell page
- Thank you/Post-purchase
- Or something entirely unique — describe it!

---

### PART 2: Page Structure Map

Create a visual map of WHAT YOU ACTUALLY SEE:

```markdown
# === PAGE STRUCTURE ===

\`\`\`
[Describe the sections in order, as they appear]
\`\`\`
```

**Don't use a pre-defined list.** Name sections based on their function:

Instead of forcing "HERO-SECTION", you might have:
- `VIDEO-EMBED-WITH-HEADLINE`
- `QUIZ-START-MODULE`
- `STORY-OPENING`
- `PROBLEM-STACK`
- `PRODUCT-GRID`
- `COMPARISON-TABLE`
- `URGENCY-BANNER`

**The section names should tell someone what's IN that section.**

---

### PART 3: Section-by-Section Breakdown

For each section you identify, document:

```markdown
---

## [SECTION: Descriptive-Name-You-Choose]

**What this section does:** [1-sentence purpose]
**Layout:** [Describe how elements are arranged]
**Background/Styling:** [Visual treatment]

[Then document each element within the section]
```

---

## Element Documentation Guidelines

### For ANY Text Element:

```markdown
### Element: [Descriptive Name]
**Type:** [Headline / Subhead / Body / Caption / Label / etc.]
**Visual Weight:** [How prominent is this? Largest on page? Supporting text?]
**Copy:**
\`\`\`
[Exact text, verbatim]
\`\`\`
```

### For ANY Interactive Element:

```markdown
### Element: [Descriptive Name]
**Type:** [Button / Link / Form / Quiz / Video / Carousel / etc.]
**Behavior:** [What happens when interacted with?]
**Copy/Label:**
\`\`\`
[Text on the element]
\`\`\`
```

### For ANY Visual Element:

```markdown
### Element: [Descriptive Name]
**Type:** [Photo / Illustration / Icon / Video / Animation / etc.]
**Content:** [What does it show?]
**Purpose:** [Why is this here? What does it communicate?]
```

### For Repeating Patterns (Cards, Lists, Grid Items):

First, describe the pattern:
```markdown
### Pattern: [Name]
**Instances:** [How many?]
**Layout:** [How arranged?]
**Each item contains:** [List the components]
```

Then document each instance:
```markdown
### Item 1:
[Components and copy]

### Item 2:
[Components and copy]
```

---

## Identifying Visual Layout from Raw Data

When analyzing screenshots or scraped content, look for clues:

### From Image Filenames:
| Filename Contains | Likely Means |
|-------------------|--------------|
| `ellipse`, `circle`, `round` | Circular image/avatar |
| `hero`, `banner` | Large featured image |
| `icon`, `ico` | Small icon graphic |
| `badge`, `seal` | Trust/certification badge |
| `avatar`, `profile` | Person photo |
| `logo` | Brand logo |
| `bg`, `background` | Background image |
| `thumbnail`, `thumb` | Small preview image |

### From Content Patterns:
| Pattern | Likely Means |
|---------|--------------|
| Same structure repeated 3+ times | Grid or carousel of cards |
| `‹ ›` or arrow symbols | Carousel navigation |
| Numbered items (1, 2, 3...) | Steps or process flow |
| ⭐ or star symbols | Ratings/reviews |
| ✓ or checkmarks | Benefits list or checklist |
| ✗ or X marks | Comparison (what you DON'T get) |
| `$` or prices | Pricing section |
| `?` in headers | FAQ section |
| Percentages or statistics | Social proof/stats bar |

### From Heading Hierarchy:
| Level | Typically Used For |
|-------|-------------------|
| H1 | Page title or major section headers |
| H2 | Section headlines |
| H3 | Subsection heads, card titles |
| H4+ | Minor labels, small headings |

---

## PART 4: Pattern Extraction

After documenting the page, extract the reusable patterns. **Only include patterns that actually appear on the page.**

```markdown
---

# === COPYWRITING PATTERNS ===

## Headlines & Hooks
[Document the headline formulas/approaches used]

## Trust & Credibility Elements
[List all trust-building elements and where they appear]

## Call-to-Action Patterns
[Document all CTAs - their copy, placement, frequency]

## Objection Handling
[How does the page address potential objections?]

## Persuasion Sequence
[Describe the flow: What's the journey from top to bottom?]

## Notable Techniques
[What's unique or interesting about this page's approach?]

---

# === END OF DOCUMENT ===
```

---

## Handling Different Page Types

### Quiz Funnels
- Document each quiz step/question
- Note the branching logic if visible
- Capture result page variations

### Video-First Pages
- Note video placement and size
- Document what's visible before/after video
- Capture any text overlays or captions

### Advertorials
- Document the "editorial" styling
- Note how it mimics news/blog content
- Capture the transition to sales content

### Short-Form Pages
- Don't pad with sections that don't exist
- A page might only have 3-4 sections — that's fine
- Focus on density of persuasion elements

### E-commerce PDPs
- Product images and gallery
- Variant selectors
- Add-to-cart area
- Product description
- Reviews integration
- Cross-sells/upsells

### Multi-Step Funnels
- Document each step separately if possible
- Note progress indicators
- Capture transitions between steps

---

## Quality Checklist

Before finishing, verify:

- [ ] Did I document sections in the order they appear?
- [ ] Did I capture ALL visible copy?
- [ ] Did I describe layouts, not just content?
- [ ] Did I name sections based on what they DO, not a template?
- [ ] Did I note visual hierarchy (what's big, what's small)?
- [ ] Did I identify repeating patterns?
- [ ] Did I extract the persuasion techniques used?
- [ ] Would a developer understand the layout from my description?
- [ ] Would a copywriter understand the messaging strategy?

---

## File Naming Convention

```
knowledge/competitor-pages/[brand]-[descriptor]-[page-type].md
```

Examples:
- `happy-mammoth-hormone-harmony-lp.md`
- `athletic-greens-ag1-quiz-funnel.md`
- `ritual-vitamins-homepage.md`
- `seed-probiotics-pdp.md`
- `goli-apple-cider-advertorial.md`
- `noom-quiz-results-page.md`
- `keeps-hair-loss-comparison.md`

---

## Example Usage

**Flexible Input:**
```
Read the prompt at knowledge/prompts/competitor-lp-breakdown.md

Analyze this: [screenshot / URL / Notion page / raw HTML]
```

**The output should adapt to whatever page type is provided.**

---

## Anti-Patterns to Avoid

❌ **Don't force sections that don't exist**
- If there's no FAQ, don't create an empty FAQ section

❌ **Don't use generic section names when specific ones are better**
- "HERO-SECTION" is fine, but "QUIZ-ENTRY-WITH-PAIN-POINT-HEADLINE" tells you more

❌ **Don't reorganize the page flow**
- Document top-to-bottom as it appears

❌ **Don't summarize copy**
- Capture it verbatim, then analyze patterns separately

❌ **Don't assume standard structures**
- A great page might break all the "rules"

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2024-12-26 | Initial prompt created |
| 2.0 | 2024-12-26 | Rewritten to be principle-based, not template-based. Added flexibility for different page types. |

