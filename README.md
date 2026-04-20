# neutral-rewriter

> A Claude skill that strips spin, bias, and emotional framing from any text — rewrites like a Wikipedia editor.

---

## What It Does

Paste in any text and get back a clean, affectless version. The skill removes emotional charge, persuasive framing, and loaded wording — keeping only the core facts and logical content.

No preamble. No commentary. Just the rewrite.

---

## Supported Content Types

- News articles and headlines
- Political statements and press releases
- Marketing and advertising copy
- Corporate memos and HR communications
- Social media posts
- Legal or policy language
- Opinion pieces

---

## How to Trigger It

Use phrases like:

- *"Neutralize this"*
- *"Remove the spin"*
- *"Rewrite this like Wikipedia"*
- *"Make this more objective"*
- *"Remove the bias from this"*
- *"Depoliticize this"*
- *"Rewrite without emotion"*

---

## What Gets Removed

| Category | Examples |
|---|---|
| Emotionally loaded nouns | "crisis," "catastrophe," "triumph," "nightmare" |
| Charged verbs | "slammed," "blasted," "exposed," "celebrated" |
| Evaluative adjectives | "reckless," "stunning," "shameful," "bold" |
| Intensifiers | "unprecedented," "shocking," "deeply," "absolutely" |
| Tribal framing | "radical left," "elites," "real Americans," "far right" |
| Rhetorical questions | "How could anyone support this?" |
| Appeals to fear or outrage | "If we don't act now..." |
| Scare quotes and emphasis formatting | Normalized to plain text |

---

## What Gets Kept

- All stated facts (who, what, where, when, how much)
- Numerical data and statistics
- Direct quotations, attributed to speaker
- Named entities (people, organizations, places)
- Explicit causal relationships and chronology

---

## Example

**Before:**
> In a devastating blow to working families, the governor callously signed a bill that slashes vital benefits for the most vulnerable residents of our state.

**After:**
> The governor signed a bill that reduces benefit payments for low-income residents.

---

**Before:**
> Reckless lawmakers IGNORE science and doom the planet with shocking vote

**After:**
> Lawmakers voted against a climate bill.

---

**Before:**
> We are thrilled to announce an exciting opportunity for our team to demonstrate their resilience and dedication as we navigate this challenging period of transformation.

**After:**
> The company is undergoing organizational changes. Employees will be expected to adjust their roles or workloads during this period.

---

## Installation

1. Download `neutral-rewriter.skill`
2. Open Claude → **Settings → Skills → Install from file**
3. Select the `.skill` file

---

## License

MIT
