# Codebook: <your study's short title>

> Copy this file into `03_Project/02_Codebook/`, rename it `codebook.md`, and fill it in.
> Delete this block before you commit.
>
> This template follows the five-part structure in **Chapter 8** of *From Vibes to
> Variables*. Your codebook is the instrument, not paperwork you write afterward. Think
> of it as source code: two coders running it on the same input should produce the same
> output.

**Author:** <name>
**Version:** draft 1
**Date:** <YYYY-MM-DD>

---

## 1. Unit of analysis

State exactly what one coded case is. This has to be unambiguous.

"Code the chat" is not a unit of analysis. "One chat message, defined as one row of
`chat_log`: one sender, one message string, one timestamp" is. If the unit is vague,
every count you report later is vague.

Say here whether each unit is coded independently of the ones around it, and note any
exception a decision rule creates.

> <your unit of analysis>

---

## 2. Variables and their categories

One block per variable. Three variables is the floor for a workable study.

Two rules govern every category list:

- **Exhaustive.** Every case can be coded. This is what the "unclassifiable" or "other"
  catch-all guarantees.
- **Mutually exclusive.** Every case fits exactly one category. If a case honestly fits
  two, your categories overlap, and overlap destroys reliability because two coders will
  split on it forever. Fix it with sharper definitions or a precedence rule.

If more than roughly one case in ten lands in the catch-all, your category scheme is
incomplete.

### Variable 1: <name>

- **Conceptual definition:** what this is, in idea terms
- **Operational definition:** what the coder actually does to produce a value
- **Level of measurement:** nominal / ordinal / interval / ratio
- **Manifest or latent:** can a coder apply this almost mechanically, or does it take
  real judgment?

| Category | Description |
| --- | --- |
| <category> | <what counts, and what does not> |
| <category> | |
| unclassifiable | none of the above criteria settle the question |

### Variable 2: <name>

<same structure>

### Variable 3: <name>

<same structure>

---

## 3. Decision rules

What coders do with the cases that do not sort themselves. **Every ambiguous case in
your Chapter 7 observation log becomes a rule here.** That is what the observation log
was for.

Number them so a coder can cite one during disagreement discussion.

1. **Precedence.** <when two categories both seem to apply, which wins and why>
2. <rule>
3. <rule>

---

## 4. Examples

Two or three prototypical cases per category, so coders have a reference for what good
coding looks like and a set of cases to train on.

| Case | Variable | Code | Why |
| --- | --- | --- | --- |
| <the actual text or record> | <variable> | <category> | <the rule or definition that decides it> |

---

## 5. Special cases

Recurring complications. **Usually empty in a first draft.** It fills in when you pilot
the codebook, which is Chapter 10's work. Leaving it thin now is correct; leaving it
thin after piloting is not.

---

## Reliability protocol

Your codebook is not finished until a second coder has applied it and the agreement has
been measured. The four steps, from Chapter 8:

1. The second coder receives the codebook with **no walk-through and no hints**, and
   codes a training set of 20 to 30 units independently.
2. The two coders compare and discuss **every** disagreement. No production data is
   coded at this stage.
3. The codebook is revised, adding a decision rule for each disagreement found.
4. The second coder codes a **fresh** reliability sample, separate from the training
   set. The agreement on that fresh sample is the kappa you report.

**Threshold.** Cohen's kappa of 0.70 or above (Landis & Koch, 1977). Below it, revise
and repeat. The reliability sample needs at least 50 coded units, and 100 or more if any
code has a low base rate.

`v2v::reliability()` computes kappa with interpretation labels.

Lombard et al. (2002) recommend reporting more than one reliability statistic. Decide
which you would report alongside kappa, and why.

| Round | Date | Units | Statistic | Value | Cleared 0.70? | What was revised |
| --- | --- | --- | --- | --- | --- | --- |
| training | | | | | | |
| reliability | | | | | | |

---

## Revision log

Keep this. Your methods section is easier to write when the history is already recorded,
and a reviewer asking why a category changed gets a real answer.

| Version | Date | What changed and why |
| --- | --- | --- |
| draft 1 | | initial draft from the Chapter 7 observation log |
