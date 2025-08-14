Perfect—here’s a tightened, production-ready **`TASK.md`** with explicit word counts, file outputs, naming conventions, and pass/fail checks so the agent reliably produces **viral how-to** content.

```markdown
# TASK.md

## Task Name
Create Viral How-To Content (Single Topic, Multi-Format)

## Objective
Generate a complete, share-worthy how-to package (article, short video script, social thread, thumbnails/captions) that is credible, actionable, and optimized for discovery and retention.

---

## Inputs (Required)
- `topic` (one clear outcome: e.g., “batch 9 shorts in 60 minutes/week”)
- `audience` (e.g., “solo creators with day jobs”)
- `primary_keyword`
- `format_priority` (`article` | `script` | `thread`; still generate all files unless told otherwise)

---

## Files to Create (Always)
1. `content/article.md` — longform article
2. `content/script.md` — short-form video script (YT Shorts/Reels/TikTok)
3. `content/thread.md` — social thread (X/LinkedIn)
4. `assets/thumbnail.txt` — thumbnail headline + visual prompt
5. `distribution/social-captions.md` — 5 platform-ready captions
6. `distribution/plan.md` — 7-day posting & repurposing plan
7. `meta/seo.yaml` — front matter (mirrors article header)
8. `meta/sources.json` — deduped source list with titles/URLs/year

> Naming: kebab-case; keep ≤60 chars. Example repo layout:
```

/content
article.md
script.md
thread.md
/assets
thumbnail.txt
/distribution
social-captions.md
plan.md
/meta
seo.yaml
sources.json

````

---

## Article Specification (`content/article.md`)
**Total length:** 1,050–1,350 words.

**Front Matter (YAML, mandatory at file top):**
```yaml
---
title: ""
slug: ""
description: ""
primary_keyword: ""
secondary_keywords: []
audience: ""
reading_time_min: 0
updated: ""
---
````

**Body Structure & Word Targets**

1. **Hook** (40–60 words)

   * Big promise + tension; mention the audience & outcome.

2. **Credibility Nugget** (25–40 words)

   * Stat or quick proof; cite inline `(Source: Name, Year)`.

3. **What You’ll Learn (Outcomes)** (40–70 words)

   * 3–5 bullets focused on outcomes, not topics.

4. **Quick Win** (90–130 words)

   * 1 action readers can do in <10 minutes; include a mini checklist.

5. **Step-by-Step Playbook** (550–700 words total)

   * 5–9 steps. For each step (90–110 words):

     * **Name** (verb-first)
     * **Why it matters** (1 sentence)
     * **Do this** (3–5 bullets, concrete actions/tools)

6. **Templates / Swipe Files** (120–160 words + code/blocks)

   * Provide at least 2 copy-and-paste blocks.

7. **Pitfalls & Fixes** (120–160 words)

   * 3–5 pitfalls; each with a one-line fix.

8. **Speedrun Recap** (50–80 words)

   * Numbered list of steps (one line each).

9. **CTA** (25–40 words)

   * Single specific next action + soft share/save ask.

10. **References** (not counted in word total)

    * List sources used; match `meta/sources.json`.

**SEO Requirements**

* Primary keyword appears in: title, description, H1, first 100 words, and one H2.
* Include **one** table **or** checklist block in the Playbook section.
* Use 3–5 semantic variants in subheads.
* Paragraphs ≤3 sentences; active voice.

---

## Script Specification (`content/script.md`)

**Total length:** 140–220 words (45–75 seconds spoken).

**Beats & Word Targets**

1. **Cold Open Hook** (15–25 words) — promise + tension in one breath.
2. **Payoff Setup** (20–30 words) — what viewers will get by the end.
3. **Core Beats (3–5 beats)** (20–35 words each)

   * Each beat = micro-hook + action; 1 tangible tip/command.
4. **Speed Recap** (15–25 words) — 3–5 words per step.
5. **CTA** (10–15 words) — comment/share/save + specific next step.

**On-screen cues (inline in brackets)** for B-roll/overlays are encouraged; keep them short.

---

## Thread Specification (`content/thread.md`)

**Total length:** 8–12 posts; **max 260 characters per post**.

**Structure**

1. Post 1: **Outcome Hook** (≤240 chars) + curiosity gap.
2. Posts 2–7/11: **Steps** — 1 step per post; imperative, 1 action + micro-example.
3. Penultimate post: **Pitfall/Fix** — 2 quick gotchas.
4. Final post: **Speedrun Recap + CTA** — numbered list + save/share ask.

---

## Thumbnail Prompt (`assets/thumbnail.txt`)

* **Headline (max 4–6 words)**: outcome + number or “without X”.
* **Visual Direction (2 lines max)**: subject, composition, emotion, prop/icon.
* **Do/Don’t**: one line each (e.g., “Do: big sans; Don’t: thin serif”).

---

## Social Captions (`distribution/social-captions.md`)

Provide **5** captions (one per platform: X, LinkedIn, IG, TikTok, YouTube).
Each: **80–140 characters**, 1 hook + 1 benefit + 1 emoji or hashtag (max 1).

---

## 7-Day Distribution Plan (`distribution/plan.md`)

**Length:** 150–220 words total.

* Day 1: Publish article + 1 teaser clip hook.
* Day 2: Carousel outline (5 frames: hook → 3 steps → CTA).
* Day 3: “Before/After” micro-case (3 bullets).
* Day 4: FAQ post (3 Q/A).
* Day 5: Contrarian angle post (1 claim, 2 supports).
* Day 6: Clip remix (Beat #2).
* Day 7: Recap thread + “results so far”.

Include 3 repurposing hooks and 1 email subject line.

---

## Meta Files

### SEO Front Matter (`meta/seo.yaml`)

```yaml
title: ""
slug: ""
description: ""
primary_keyword: ""
secondary_keywords: []
audience: ""
reading_time_min: 0
canonical_url: ""
og_image: ""
updated: ""
```

### Sources (`meta/sources.json`)

```json
{
  "sources": [
    {"title": "", "url": "", "publisher": "", "year": 0}
  ]
}
```

---

## Hard Rules (Pass/Fail)

* ✅ **Word targets met** within ±10% for each section.
* ✅ **Primary keyword** present in mandated locations.
* ✅ **At least 2 templates/swipes** in the article.
* ✅ **One table or checklist** included in the article body.
* ✅ **Thread has 8–12 posts**; **script 140–220 words**.
* ✅ **All files listed above are created** with non-empty, on-spec content.
* ✅ **All claims with numbers are sourced** in References & `sources.json`.
* ❌ No medical/legal/financial advice beyond general education.
* ❌ No plagiarism; paraphrase and cite.

---

## Workflow (Agent Must Follow)

1. **Clarify Inputs** → if missing, infer defaults and proceed.
2. **Research (15 minutes max)** → gather 3–5 credible sources; capture to `meta/sources.json`; avoid blogs when primary sources exist.
3. **Outline** article/script/thread to match structures/word targets.
4. **Draft** article first (ensures source coherence), then script, then thread.
5. **SEO Pass** → fill `meta/seo.yaml`; verify keyword placements.
6. **Polish** → readability (Grade 6–8), active voice, short paragraphs.
7. **Assemble Distribution** → captions + 7-day plan + thumbnail prompt.
8. **Validate** against Hard Rules. If any fail, fix and re-validate.

---

## Acceptance Checklist (for CI or human review)

* [ ] `content/article.md` word count 1,050–1,350
* [ ] Hook 40–60; Credibility 25–40; Outcomes 40–70; Quick Win 90–130
* [ ] Playbook 5–9 steps, each 90–110 words; Templates 120–160; Pitfalls 120–160; Recap 50–80; CTA 25–40
* [ ] `content/script.md` 140–220 words; structure intact
* [ ] `content/thread.md` 8–12 posts, each ≤260 chars
* [ ] `assets/thumbnail.txt` present with headline + direction + do/don’t
* [ ] `distribution/social-captions.md` has 5 captions (80–140 chars)
* [ ] `distribution/plan.md` 150–220 words with daily breakdown
* [ ] `meta/seo.yaml` complete; `meta/sources.json` has ≥3 sources
* [ ] At least one table or checklist in the article body
* [ ] All numeric claims have inline citations + entry in `sources.json`

---

::contentReference[oaicite:0]{index=0}
```
