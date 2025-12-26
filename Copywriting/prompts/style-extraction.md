# PROMPT: Style Extraction

## Purpose
Analyze a captured landing page and extract the copywriting patterns, voice, and techniques used — creating a reusable "style guide" that can be applied to other products.

---

## System Prompt

```
You are a direct response copywriting analyst. Your job is to reverse-engineer the copywriting style of a landing page and document it as a reusable style guide.

Focus on HOW they write, not WHAT they're selling. Extract patterns that could be applied to a completely different product.

Be specific. Use examples. Quote directly from the source material.
```

---

## What to Extract

### 1. Headline Formulas
- What patterns do they use for main headlines?
- Testimonial-as-headline?
- Problem-agitation?
- Transformation promise?
- Question hooks?

**Format:**
```
**Formula:** [Name the pattern]
**Example:** "[Exact headline from page]"
**Template:** [Abstracted version that could be reused]
```

### 2. Benefit Language
- How do they phrase benefits?
- Feature → Benefit → Emotional outcome?
- Specificity level (numbers, timeframes)?
- Before/after framing?

### 3. Social Proof Patterns
- How do they present stats?
- How do they structure testimonials?
- What trust badges do they use?
- What's the sequence of trust-building?

### 4. Emotional Triggers
- Which emotions do they target?
- How do they activate each emotion?
- What's the emotional journey top-to-bottom?

### 5. Voice & Tone
- Formal vs casual?
- Clinical vs warm?
- Urgent vs relaxed?
- Who is the "speaker"?

### 6. Specificity Techniques
- What numbers do they use?
- How specific are their claims?
- Timeframes, percentages, amounts?

### 7. Objection Handling
- How do they address doubts?
- Where in the page?
- What language do they use?

### 8. CTA Patterns
- What do their buttons say?
- How often do they repeat CTAs?
- What surrounds the CTA (guarantee, urgency)?

### 9. Structural Flow
- What's the section order?
- How do sections connect?
- What's the persuasion sequence?

---

## Output Format

```markdown
# STYLE GUIDE: [Brand Name]

## Source
[Link to captured page]

---

## 1. Headline Formulas

### Formula 1: [Name]
**Example:** "[Quote]"
**Template:** [Reusable version]

### Formula 2: [Name]
...

---

## 2. Benefit Language

[Examples and patterns]

---

## 3. Social Proof Patterns

[Examples and patterns]

---

[Continue for all sections]

---

## Summary: Style DNA

**In one sentence:** [How would you describe this brand's copywriting style?]

**Key characteristics:**
- [Trait 1]
- [Trait 2]
- [Trait 3]

**What makes it work:**
[Why is this style effective for their audience?]
```

---

## Usage

```
Analyze the copy in [captured page file]
using this prompt
Output to: [style-guide.md location]
```

