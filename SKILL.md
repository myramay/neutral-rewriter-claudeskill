---
name: neutral-rewriter
description: >
  Rewrites any text in plain, neutral, factual language — removing emotional charge,
  persuasive framing, spin, and loaded wording. Use this skill whenever the user asks
  to "neutralize", "defuse", "depoliticize", "make neutral", "remove bias", "remove spin",
  "rewrite without emotion", "rewrite like Wikipedia", or "make this more objective."
  Also trigger when the user shares a piece of text and asks for a plain, factual, or
  affectless version of it. Applies to any content type: news articles, press releases,
  political statements, marketing copy, opinion pieces, internal memos, social media posts,
  legal language, HR communications, or any other text with detectable tone or slant.
---

# Neutral Rewriter

## Purpose

Transform any text into plain, factual, affectless language. Remove all emotional charge,
persuasive framing, and loaded wording. Keep only the core facts and logical content.
Write like a Wikipedia editor: clear, direct, and completely affectless.

---

## Core Principles

1. **Preserve facts, strip tone.** Every factual claim should survive the rewrite. Every
   emotional or persuasive element should not.

2. **No added commentary.** Do not editorialize, contextualize, or add your own analysis.
   The output is a rewrite of what was provided — not an assessment of it.

3. **One version only.** Produce a single rewritten version. Do not offer multiple options
   unless the user explicitly asks.

4. **Match scope.** If the user gives one sentence, rewrite one sentence. If they give a
   full article, rewrite a full article. Do not summarize unless asked.

5. **No meta-commentary.** Do not explain what you changed, note what was loaded, or add
   a preamble. Output the rewrite and nothing else — unless the user asks for explanation.

---

## What to Remove

| Category | Examples |
|---|---|
| Emotionally loaded nouns | "crisis," "catastrophe," "miracle," "nightmare," "triumph" |
| Charged verbs | "slam," "blast," "expose," "devastate," "celebrate" |
| Evaluative adjectives | "shameful," "bold," "reckless," "stunning," "alarming" |
| Amplifiers and intensifiers | "unprecedented," "shocking," "absolutely," "deeply" |
| Tribal/identity framing | "radical left," "far right," "elites," "real Americans" |
| Rhetorical questions | "How could anyone support this?" |
| Implied causation without evidence | "Obviously this led to..." |
| Appeals to fear or outrage | "If we don't act now..." |
| Passive constructions that obscure agency | "Mistakes were made" → say who made them if known |
| Scare quotes | Remove them and use the term directly |
| Italics or capitalization for emphasis | Normalize formatting |

---

## What to Keep

- All stated facts (who, what, where, when, how much)
- Numerical data and statistics
- Direct quotations (attributed to speaker)
- Named entities (people, organizations, places)
- Causal relationships that are stated explicitly and factually
- Chronology and sequence
- Definitions and technical terms (without spin)

---

## Substitution Patterns

Apply these transforms systematically:

| Loaded phrasing | Neutral equivalent |
|---|---|
| "slammed," "blasted," "ripped" | "criticized" |
| "celebrated," "hailed" | "praised" |
| "admitted" (implying guilt) | "said" or "stated" |
| "claimed" (implying doubt) | "said" or "stated" (unless doubt is factually established) |
| "exposed" | "reported" or "revealed" |
| "quietly" (implying secrecy) | remove or use "without public announcement" |
| "desperate," "forced to" | describe the action taken, omit the characterization |
| "historic," "unprecedented" | check if factually true; if not, remove |
| "finally," "at last" | remove unless timing is factually significant |
| "despite" (used rhetorically) | restructure as two separate facts |

---

## Format

- **Input**: Any text the user provides.
- **Output**: The rewritten text, in the same structure and length as the input (paragraph → paragraph, list → list, etc.). No preamble. No postscript. Just the rewrite.
- **Exception**: If the user asks for explanation, append a brief note after the rewrite describing the main categories of changes made.

---

## Examples

### Example 1: Political statement

**Input:**
> In a devastating blow to working families, the governor callously signed a bill that
> slashes vital benefits for the most vulnerable residents of our state.

**Output:**
> The governor signed a bill that reduces benefit payments for low-income residents.

---

### Example 2: Marketing copy

**Input:**
> Our revolutionary product has transformed the lives of millions. Don't miss your chance
> to finally achieve the results you've always dreamed of.

**Output:**
> The product has been purchased by a large number of customers. It is available for purchase.

---

### Example 3: News headline

**Input:**
> Reckless lawmakers IGNORE science and doom the planet with shocking vote

**Output:**
> Lawmakers voted against a climate bill.

---

### Example 4: Corporate memo

**Input:**
> We are thrilled to announce an exciting opportunity for our team to demonstrate their
> resilience and dedication as we navigate this challenging period of transformation.

**Output:**
> The company is undergoing organizational changes. Employees will be expected to adjust
> their roles or workloads during this period.

---

## Edge Cases

- **Quotations**: Keep direct quotes verbatim and attributed. Do not neutralize what someone
  actually said — instead, neutralize the framing *around* the quote.
- **Satire or fiction**: If the input is clearly satirical or creative, note this and ask
  the user to clarify intent before rewriting.
- **Factual uncertainty**: If a claim in the original cannot be verified from the text
  itself (e.g., "studies show"), keep the claim but render it precisely: "according to
  the author" or "the author states that studies show."
- **Missing facts**: If the original is so vague that no factual content survives removal
  of the spin, output what remains and note that the source contained limited factual content
  (only if the user asked for explanation).
