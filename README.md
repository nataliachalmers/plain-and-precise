# plain-and-precise

A Claude skill that rewrites expert health and policy writing for non-expert readers without letting the claims drift: every change explained, every shift in meaning flagged, tuned to four reader types, with an editor mode and a coach mode.

Readers outside your field — a newspaper reader, a health-system CEO, a Hill staffer, a coalition member — decide in the first two sentences whether to keep going, and none of them will look up a term. Plain language is translation into the reader's words, not dumbing down. The risk is that a smoother sentence quietly changes a claim: "preventive dental services" becomes "a checkup", "associated with" becomes "leads to", "cleared" becomes "approved". So every rewrite here is checked back against what the original actually claimed, and the places where plainness cost precision are handed back as decisions, not buried.

## Two modes

- **Edit** (default): the rewrite, ready to paste, with a change log and drift flags.
- **Coach**: say "coach me" or "don't rewrite it." Same reading and diagnosis, but the fixes come as patterns worked on one of your own sentences, three per round, and you do the rest. It never hands back a finished piece in coach mode unless you switch with "just edit it."

## Four readers

What "plain" means depends on who is reading. Same finding, different first sentence.

| Reader | Typical pieces | What plain means here |
|---|---|---|
| General public | Op-eds, LinkedIn posts | One idea, a person in the first two sentences, no acronyms, the first line carries the point |
| Payer, health-system and Hill | One-pagers, memos, letters | The ask and the number in the first paragraph; their currency is cost, access, measurement, precedent; it has to survive being forwarded |
| Lay summary of research | Press-style and blog paragraphs, patient-facing versions | What was studied, what was found, what it means, what it does not show; numbers exact with denominators; associations stay associations |
| Clinicians and coalition partners | Emails, announcements, updates | Action and date first, what changed, what to do; they keep their own vocabulary, so plain means short and structured, not de-jargoned |

## How it works (edit mode)

1. **Read once for meaning** and write a ledger of every claim: numbers with denominators and years, causal or associational statements, regulatory statuses, attributions.
2. **Fix the frame:** reader, venue, and what the reader should do afterward. Inferred where possible, asked once if not, assumed and labeled if you're in a hurry.
3. **Diagnose structure before sentences** and name the single biggest problem: usually a buried point, a piece about a system rather than a person, three ideas where the reader can carry one, or a missing ask.
4. **Rewrite from the outside in:** structure, then paragraphs, then sentences (jargon to the reader's word, passive to the actor, nominalizations to verbs, empty hedges to the number or gone, abstractions to a concrete scene), keeping the writer's voice and avoiding AI cadence.
5. **Check the rewrite against the ledger.** Every claim must keep its scope, direction, magnitude and certainty. Anything that moved is recorded as drift and handed back as a choice. Nothing is added: no statistic, quote or example the writer didn't supply.
6. **Measure and deliver:** words, average and longest sentence, acronyms remaining, computed rather than guessed.

## What you get

Reader, venue and intended action (assumptions labeled) · the biggest problem in one sentence · the rewrite · a "what changed, and why" table of the ten or so edits that carry a pattern · a meaning-drift section with your options for each · claims that need a source · before-and-after numbers.

## Example

Original: *"Utilization of preventive dental services among Medicaid-enrolled adults remains suboptimal, with significant implications for downstream emergency department utilization and associated expenditures."*

Rewrite for a general reader: *"Too few adults on Medicaid get preventive dental care, and more of them end up in the emergency room with dental pain."*

Meaning drift the skill would flag: a tempting version of that first clause is "get a routine dental checkup," which narrows "preventive dental services" (they also include cleanings, fluoride and sealants), so the broader term stays unless the writer chooses otherwise. Needs a source: the emergency-room and cost claim, which plain wording has made sharper and therefore easier to check.

## Rules, each with its reason

The reader's words, not the smallest words. Point first. A person in the first two sentences. Precision beats plainness when they conflict, and the skill says which it chose. Keep the hedges that carry information ("was associated with"), cut the ones that don't ("significant," "robust"). Add nothing. Regulatory and clinical words keep their exact meaning: cleared is not approved, requires is not encourages, introduced is not passed. One idea per piece. The writer's voice survives the edit. Shorter is usual, not the rule: a lay summary can run longer than the abstract it came from. Ask once, then proceed.

The skill also carries a swaps table of about twenty terms that recur in dental and health-policy writing (utilization, beneficiaries, prior authorization, fee-for-service, value-based care, caries, periodontal disease, edentulous, radiograph, oral-systemic, interoperability, FDA-cleared) with the general reader's version of each.

## When it triggers

Ask to make text plainer, simpler, less academic or more readable; name one of the four readers; ask "would a non-dentist get this?"; or share a draft headed to non-experts, even if you only say "tighten this." It is not for removing AI tells or for controlled technical English; those are separate skills.

## Install

**Claude Code:** clone this repository into your personal skills folder, then type `/plain-and-precise` or paste a draft and say who it's for.

```bash
git clone https://github.com/YOUR-USERNAME/plain-and-precise.git ~/.claude/skills/plain-and-precise
```

**Claude apps (claude.ai, desktop):** add the skill from the Skills section of Settings, either by uploading this folder or by pasting the contents of `SKILL.md` into a new skill.

## Adapting it

The ledger-and-drift method, the two modes and the output format are general. The four readers and the swaps table are specific to U.S. dental and Medicaid/Medicare policy: replace the readers with the audiences you write for and the swaps with the jargon of your own field, and keep the rest.
