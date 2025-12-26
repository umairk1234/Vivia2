# Project: PDP Copy Rewrite v1

**Goal:** Rewrite Vivia PDP copy inspired by Happy Mammoth's copywriting style  
**Target Page:** https://www.byvivia.com/products/pdp3  
**Inspiration:** Happy Mammoth Hormone Harmony LP  
**Constraint:** Keep existing PDP structure, rewrite the copy only

---

## Pipeline

```
┌─────────────────────────────────────────────────────────────┐
│                     PDP REWRITE PIPELINE                     │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  STEP 1: INPUTS (DONE)                                      │
│  ├── Happy Mammoth LP capture ✅                             │
│  ├── Product brief ✅ (from Notion)                          │
│  └── Audience brief ✅ (from Notion)                         │
│                                                              │
│  STEP 2: STYLE EXTRACTION                                   │
│  └── Analyze HM copy → patterns, voice, techniques          │
│      Output: style-guide.md                                 │
│                                                              │
│  STEP 3: CURRENT PDP CAPTURE                                │
│  └── Document current Vivia PDP structure + copy            │
│      Output: current-pdp-capture.md                         │
│                                                              │
│  STEP 4: COPY GENERATION                                    │
│  └── Style + Product + Audience + Structure → New copy      │
│      Output: output/pdp-v1.md                               │
│                                                              │
│  STEP 5: REVIEW & ITERATE                                   │
│  └── Human review → feedback → regenerate                   │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

---

## Step 1: Inputs ✅

### 1A. Happy Mammoth LP Capture
**Location:** `knowledge/competitor-pages/happy-mammoth-hormone-harmony-lp.md`  
**Status:** Complete (1,301 lines)

### 1B. Product Brief
**Source:** Notion — FAQs, Product Overview, State of Business  
**Key Info:**

| Field | Value |
|-------|-------|
| **Product** | Intimate Bloom by Vivia |
| **What it is** | Bioidentical estriol cream (topical) |
| **What it does** | Rebuilds vaginal tissue, restores natural moisture |
| **How it's different** | Local action (not systemic HRT), European standard for 50+ years |
| **Key ingredients** | Estriol (bioidentical hormone) |
| **How to use** | Topical application |
| **Price point** | ~$54 (single), bundles available |
| **Guarantee** | 60-day money back |
| **Target symptom** | Vaginal dryness, atrophy, painful sex |

### 1C. Audience Brief
**Source:** Notion — Persona document (extremely detailed)  
**Summary:**

| Field | Value |
|-------|-------|
| **Who** | Women 45-65, menopausal/perimenopausal |
| **Demo** | Suburban, $90K HHI, married, grown kids |
| **Primary pain** | Vaginal dryness, painful sex, relationship strain |
| **Emotional state** | Feels broken, dismissed by doctors, desperate |
| **What she's tried** | KY, Replens, Revaree, coconut oil, systemic HRT — all failed |
| **What she wants** | To feel normal, to want her husband again, to not be in pain |
| **Trust barriers** | Scared of hormones (2002 study), burned by doctors |
| **Language** | "Broken," "sandpaper," "dread," "dry down there" |

---

## Step 2: Style Extraction ⏳

**Goal:** Analyze Happy Mammoth LP and extract copywriting patterns

**What to extract:**
- Headline formulas (testimonial-as-headline, problem-agitation, etc.)
- Benefit language patterns (how they phrase benefits)
- Trust-building sequence (what order, what elements)
- Emotional triggers (which emotions, how activated)
- Specificity techniques (numbers, timeframes, details)
- Voice/tone markers (casual vs clinical, warm vs urgent)
- Structural patterns (how sections flow)

**Output:** `style-guide.md`

**Prompt to use:** `Copywriting/prompts/style-extraction.md`

---

## Step 3: Current PDP Capture ⏳

**Goal:** Document current Vivia PDP structure and copy

**What to capture:**
- Every section in order
- All copy verbatim
- Layout/structure notes
- What to KEEP vs what to REWRITE

**Output:** `current-pdp-capture.md`

**Method:** Screenshot PDP → use `knowledge/prompts/competitor-lp-breakdown.md`

---

## Step 4: Copy Generation ⏳

**Goal:** Generate new PDP copy

**Inputs:**
- Style guide (from Step 2)
- Product brief (Step 1B)
- Audience brief (Step 1C)
- Current PDP structure (Step 3)

**Constraints:**
- Keep existing structure/sections
- Apply HM style patterns to Vivia's product + audience
- Maintain Vivia brand voice (medical authority + empathy + anger on her behalf)

**Output:** `output/pdp-v1.md`

**Prompt to use:** `Copywriting/prompts/copy-rewriter.md`

---

## Step 5: Review & Iterate

**Human review criteria:**
- Does it sound like Vivia (not Happy Mammoth)?
- Does it speak to OUR audience's specific pain?
- Is the medical credibility maintained?
- Is the gaslighting angle preserved?
- Does it feel authentic, not templated?

**Iteration loop:**
- Feedback → adjust prompt/inputs → regenerate
- Version outputs: `pdp-v2.md`, `pdp-v3.md`, etc.

---

## Key Differences: Happy Mammoth vs Vivia

| Aspect | Happy Mammoth | Vivia |
|--------|---------------|-------|
| **Product** | Oral supplement (capsules) | Topical cream (estriol) |
| **Mechanism** | Natural extracts, adaptogens | Bioidentical hormone |
| **Target symptom** | Hormonal weight gain, mood | Vaginal dryness, painful sex |
| **Brand voice** | Warm, girlfriend energy | Medical authority + advocacy |
| **Trust angle** | 62K reviews, clinical studies | European standard, doctor-led |
| **Core message** | "Melt hormonal fat" | "You're not broken, the system failed you" |

**Implication:** We're borrowing HM's STYLE (how they write), not their MESSAGE (what they say).

---

## Files to Create

- [ ] `style-guide.md` — Extracted HM patterns
- [ ] `current-pdp-capture.md` — Current Vivia PDP documented
- [ ] `output/pdp-v1.md` — First generated version

---

## Next Action

**Step 2:** Run style extraction on Happy Mammoth LP capture

```
Analyze the copy in knowledge/competitor-pages/happy-mammoth-hormone-harmony-lp.md
using the prompt at Copywriting/prompts/style-extraction.md
Output to: Copywriting/projects/pdp-rewrite-v1/style-guide.md
```

