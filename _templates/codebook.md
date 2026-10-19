# Codebook: <your study's short title>

> Copy this file into `03_Project/02_Codebook/`, rename it `codebook.md`, and fill it in.
> Delete this block before you commit.
>
> This template follows the five-part structure in **Chapter 8** of *From Vibes to
> Variables*. Your codebook is the instrument, not paperwork you write afterward. Think
> of it as source code: run it twice on the same input, weeks apart, and it should
> produce the same output.

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

You are the only coder in this course, so the check is a **stability** check: how well
you agree with yourself. The codebook is not finished until that figure has been measured.
The four steps:

1. Code the pilot items once, in pass 1, and record the date.
2. After at least 48 hours, code the same items again in pass 2 **with your pass 1 codes
   hidden**, and record that date too. The gap and the hiding are what make the second
   pass independent.
3. Compare every disagreement and add a decision rule for each one found.
4. Report the agreement between the two passes as your stability figure, and name the
   single-coder limitation as such: a second coder is not part of this course.

**Threshold.** Cohen's kappa of 0.70 or above (Landis & Koch, 1977). Below it, revise the
codebook and repeat the two passes on a fresh subset.

`v2v::reliability()` computes kappa or alpha from your two columns of codes. The R
Companion's **Reliability grid** takes pass 1 and pass 2, hides pass 1 while you enter
pass 2, records both dates, saves the codes as a CSV, and writes the `v2v::reliability()`
call (kappa or alpha) into your script. To enter the codes themselves in VS Code instead of a
spreadsheet, **AURA: Open the data viewer** opens your sampled CSV in a grid where you add a coding
column per variable and code each row; the codes save to `data/derived/` at the top of the workspace,
the original file is never changed, and **Insert rebuild code** writes the lines that join them back on.
A spreadsheet still works.

Lombard et al. (2002) recommend reporting more than one reliability statistic. Decide
which you would report alongside kappa, and why.

| Round | Pass 1 date | Pass 2 date | Units | Statistic | Value | Cleared 0.70? | What was revised |
| --- | --- | --- | --- | --- | --- | --- | --- |
| pilot | | | | | | | |
| re-code | | | | | | | |

---

## Revision log

Keep this. Your methods section is easier to write when the history is already recorded,
and a reviewer asking why a category changed gets a real answer.

| Version | Date | What changed and why |
| --- | --- | --- |
| draft 1 | | initial draft from the Chapter 7 observation log |
