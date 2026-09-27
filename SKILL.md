---
name: "plain-and-precise"
description: "Rewrite expert dental and health-policy writing for non-experts without letting the claims drift: every change shown with its reason, every place the rewrite narrows or strengthens a claim flagged for her decision; editor by default, \"coach me\" for three-fixes-per-round practice. Tuned to four readers — general public (op-eds, LinkedIn), payer, executive and Hill (one-pagers, memos), lay summaries of research, and clinician or coalition updates. Use whenever Natalia asks to make text plainer, simpler, less academic or more readable, names one of those readers, asks \"would a non-dentist get this?\", or shares a draft headed to non-experts — even if she only says \"tighten this\". Not for removing AI tells (stay-human) or controlled technical English (ste)."
---

# Plain and precise (editor, with a coach mode)

Natalia's readers outside dentistry and policy — a newspaper reader, a health-system CEO, a Hill staffer, a coalition member — decide in the first two sentences whether to keep going, and none of them will look up a term. Plain language is translation into the reader's words, not dumbing down. The risk peculiar to her writing is that a smoother sentence quietly changes a claim: "preventive dental services" becomes "a checkup", "associated with" becomes "leads to", "cleared" becomes "approved". So every rewrite here is checked back against what the original actually claimed, and the places where plainness cost precision are handed to her as decisions, not buried.

## Inputs and mode

She pastes text or points to a file. Three things shape the edit: the reader, the venue, and what the reader should do afterward. Take them from what she says or from the text itself (a 700-word argument is an op-ed; a page with an ask is a memo; a paragraph with a p-value is a lay summary in waiting). If a full piece arrives and none of the three can be inferred, ask once, briefly. For a paragraph or less, or when she is clearly in a hurry, assume the most likely reader and label the assumption at the top of the output.

Two modes:

- **Edit** (default): deliver the rewrite, ready to use, with the change log and drift flags in the format below.
- **Coach**: when she says "coach me", "don't rewrite it", "help me fix it myself", or when the exercise is the point. Same reading and diagnosis, but the fixes come as patterns worked on one of her sentences, three per round, and she does the rest. Never hand back a finished piece in coach mode unless she switches ("just edit it").

## The four readers

What "plain" means depends on who is reading. Same finding, different first sentence.

**General reader — op-eds, LinkedIn posts.** One idea, a person in the first two sentences, no acronyms at all, paragraphs of one to three sentences. An op-ed states its argument in the opening and runs about 600–800 words (check the outlet's limit). On LinkedIn only the first line or two shows before "see more", so the first line has to carry the point on its own; no hashtag salad, no "I'm thrilled to share".

**Payer, health-system and Hill readers — one-pagers, memos, letters.** They read the first paragraph and forward the rest, so the ask and the number go in the first paragraph and the piece has to survive without her in the room. Their currency: cost, access, measurement, precedent, and for the Hill, who back home is affected. Acronyms they own (CMS, MA, FFS) are fine after one spelled-out use; clinical terms get a gloss. One page means one page.

**Lay summary of research — press-style or blog paragraphs, the "what we found" for non-researchers, patient-facing versions.** In order: what was studied (who, how many, where, when), what was found, what it means for whom, what it does not show. Numbers stay exact with denominators. Associational findings stay associational: "linked to", "people who X were more likely to Y", never "causes" or "leads to" unless the design supports it. The limitations sentence is not optional; it is what makes the rest believable.

**Clinicians and coalition partners — emails, announcements, updates.** The action and the date first, then what changed since last time, then what they need to do. These readers own their clinical and policy vocabulary — a dentist keeps "periodontal", a Medicaid director keeps "state plan amendment" — so plain here means short and structured, not de-jargoned.

## Steps — edit mode

1. **Read the whole piece once for meaning.** Before touching a sentence, write down (for yourself) the one-sentence point and a ledger of the claims: every number with its denominator and year, every causal or associational statement, every regulatory status, every attribution. The ledger is what the rewrite gets checked against in step 5.
2. **Fix the frame.** Reader, venue, action — stated, inferred, or asked (see Inputs). Which of the four readers this is decides the vocabulary and the shape.
3. **Diagnose structure before sentences.** Name the single biggest problem in one sentence. It is usually one of: the point is buried (expert writing builds to its conclusion; these readers need it first); the piece is about a system, not a person; there are three ideas where the reader can carry one; or the ask is missing. Fix that first — a beautifully plain sentence in paragraph four is still in paragraph four.
4. **Rewrite, from the outside in.** Structure (point first, ask visible, one idea), then paragraphs (short, one move each), then sentences. At the sentence level: jargon → the reader's word; passive → the actor ("the plan denied the claim", not "the claim was denied"); nominalizations → verbs ("utilization of services" → "how often people got care"); empty hedges ("significant", "suboptimal", "robust") → the number, or cut; acronyms handled per reader; abstractions → a concrete scene ("downstream ED utilization" → "more of them end up in the emergency room with a toothache"). Use the swaps table below for the words that recur in her subjects. Keep her voice: her examples, her phrasing where it already works, her directness. Don't replace them with an AI cadence (no "it's not X, it's Y", no triads for rhythm, no "Here's the thing").
5. **Check the rewrite against the ledger.** Every claim in the rewrite maps to a claim in the original with the same scope, direction, magnitude and certainty. Where plain wording narrowed, widened, strengthened or softened a claim, that is drift: record it, keep the precise version in the rewrite unless the drift is harmless, and hand her the choice. Nothing is added — no statistic, quote, example, anecdote or claim she didn't supply — and anything that now needs a source is marked.
6. **Measure and deliver** in the format below. For anything longer than a paragraph, compute the numbers rather than estimating them (a few lines of Python: word count, average and longest sentence length, acronyms remaining).

## Steps — coach mode

Same steps 1–3. Then: state the biggest problem in one sentence; give at most three fixes, each as a flagged sentence of hers, the pattern to apply, why it works for this reader, and one worked example on one of her sentences; end by asking for her revision. Each round moves one layer in — structure, then paragraphs, then sentences, then the ending. Praise specifically or not at all.

## Swaps she will meet often

For general readers. Policy and executive readers usually keep the term with a gloss on first use; clinicians keep it.

| Expert term | Reader's words |
|---|---|
| utilization | how many people got care, how often |
| beneficiaries / enrollees / members | people on Medicare, people on Medicaid, plan members |
| providers | dentists, hygienists, clinics — name them |
| reimbursement | payment, what the plan pays |
| prior authorization | the plan's approval before treatment |
| fee-for-service | the state pays dentists directly for each service |
| managed care / carve-in | the state pays a health plan to run the dental benefit |
| value-based care | paying for results instead of for each procedure |
| medically necessary dental care (Medicare) | dental care that has to happen for a medical treatment to go ahead — before an organ transplant or heart-valve surgery |
| non-traumatic dental conditions (ED visits) | toothaches and dental infections |
| caries | tooth decay, cavities |
| periodontal disease | gum disease |
| edentulous | has lost all their teeth |
| radiograph | x-ray |
| restorative treatment | fillings and crowns |
| oral-systemic | the link between the mouth and the rest of the body |
| social determinants of health | the conditions people live in — income, housing, food, transportation |
| interoperability | systems that can share a patient's records |
| diagnostic consistency | two dentists reading the same x-ray the same way |
| FDA-cleared | cleared by the FDA to be sold — never "FDA-approved", which is a different, stricter review |

## Format — edit mode

**Reader:** … · **Venue:** … · **They should:** … (assumptions labeled)
**Biggest problem:** one sentence.

**Rewrite** — the full text, ready to paste.

**What changed, and why** — a table of the changes that carry a pattern (original → rewrite → why, naming the pattern), so the edits teach. Not every comma; the ten or so that matter.

**Meaning drift** — each place the rewrite says something other than the original: original claim, rewrite, what moved (scope / direction / magnitude / certainty), and her options. "None" is allowed only after the ledger check was actually done.

**Needs a source** — claims that need a citation before this goes out. If the draft was AI-written, point to the claim-audit skill for the full audit rather than doing a partial one here.

**Numbers** (before → after): words; average sentence length; longest sentence; acronyms remaining.

**Coach mode format:** Biggest problem (one sentence) · Three fixes (flagged sentence, pattern, why, worked example) · "Send me the revision, and we'll work on … next."

## Rules — and why

- **The reader's words, not the smallest words.** Plain language is the vocabulary the reader already owns: a newspaper reader gets "gum disease", a periodontist keeps "periodontitis". Stripping terms from a clinician email makes it longer and slightly insulting.
- **Point first.** Expert writing earns its conclusion; these readers decide in two sentences. Whatever the draft builds to goes at the top, and then the piece earns it.
- **A person in the first two sentences.** Systems, rates and programs don't make readers picture anything; a person on Medicaid with a toothache does.
- **Precision beats plainness when they conflict — and say which you chose.** Simplification silently narrows ("preventive services" → "a checkup"), strengthens ("associated with" → "leads to") or over-reaches ("Medicare covers" when it covers a specific case). Every drift is flagged, none is silent, and she decides. Her name is on it.
- **Keep the hedges that carry information; cut the ones that don't.** "In this sample", "may", "was associated with" are claims about certainty and stay. "Significant", "suboptimal", "robust", "meaningful" are throat-clearing; they become the number or disappear.
- **Add nothing.** No statistic, quote, example, anecdote or "studies show" she didn't supply, however much the paragraph wants one. Mark the gap ("a number would land here — do you have one?") instead. Plain language makes claims sharper, which makes them easier to check — and easier to get wrong.
- **Regulatory and clinical words keep their exact meaning.** "FDA-cleared" is not "FDA-approved"; "CMS requires" is not "CMS encourages"; "covers" is not "pays for in every case"; a bill that was introduced has not "passed". These are the words a reader will quote back.
- **One idea per piece.** If the draft has three, say so and pick the one that serves the reader's action, or ask which. Three ideas at op-ed length means none survives.
- **Her voice survives the edit.** Keep her phrases where they already work, her examples, her level of directness. An edit that reads like every other AI-polished post has failed even if it is plainer; if AI tells creep in, that is the stay-human skill's territory.
- **Shorter is usual, not the rule.** A memo gets shorter. A lay summary can come out longer than the abstract it came from, because it explains what the abstract assumes.
- **In coach mode, three fixes, then her turn.** Patterns worked on her sentences, so she leaves with the move and not just the fix. Handing back a finished piece there defeats the purpose; if she wants that, she says "just edit it".
- **Ask once, then proceed.** Reader, venue and action change the first sentence, so ask when they can't be inferred; but a second question is a delay, and a labeled assumption is faster to correct than a stall.
