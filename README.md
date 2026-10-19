# V2V Course Workspace

**One VS Code folder for everything you write and build this term.**

This is a GitHub template repository for MC 451 and MC 501 at SIUE. You make your own
copy, open it in VS Code, and keep your journals, reading notes, project files, and
drafts in one place, version-controlled with Git.

Everything here is plain Markdown and plain files. No wiki plugins, no graph views, no
second app to learn. Your work is readable anywhere and it stays yours after the course
ends.

## Part of From Vibes to Variables

[From Vibes to Variables (V2V)](https://aura-lab.siue.edu/v2v/) is the AURA Lab's open methods package for teaching media research at Southern Illinois University Edwardsville. Its parts are built to be used together:

- [Textbook](https://aura-lab.siue.edu/v2v/) ([source](https://github.com/AURA-Lab-SIUE/v2v)): the open textbook that carries the arc from research question to published report.
- [Course hub](https://aura-lab.siue.edu/v2v-hub/) ([source](https://github.com/AURA-Lab-SIUE/v2v-hub)): the course website for MC 451 and MC 501 that sequences the textbook, the labs, and the setup guides.
- [v2v R package](https://github.com/AURA-Lab-SIUE/v2v-r): the companion package with the Twitch practice corpus and the helpers the textbook introduces chapter by chapter.
- [Course workspace](https://github.com/AURA-Lab-SIUE/v2v-workspace) (this repository): the VS Code template students copy for journals, reading notes, and project work.
- [R Companion](https://github.com/AURA-Lab-SIUE/r-companion): the VS Code extension that checks each student's R setup, installs what is missing, and explains common R errors.

A sibling template, [mc427-codespace](https://github.com/AURA-Lab-SIUE/mc427-codespace), gives MC 427 Social Media Analytics the same VS Code and R toolchain in a GitHub Codespace; the R Companion serves MC 427 as well, and the v2v package is not used there.

## Set it up

**1. Make your copy.** Click **Use this template**, then **Create a new repository**.
Name it `mc451-workspace` or `mc501-workspace`, and leave it **Public**. Your graded
submission is the repository URL, so it has to be one anyone can open.

**2. Clone it into VS Code.** Open the Command Palette (`Ctrl/Cmd+Shift+P`), run
**Git: Clone**, paste your repository URL, and pick a location you will remember, for
example `Documents/MC451/`. VS Code offers to open the folder. Say yes.

**3. Install the recommended extensions.** VS Code prompts you the first time you open
the folder. Click **Install**. They are pinned in `.vscode/extensions.json` so the whole
class works in the same environment. Then run **Check my setup** from the Command
Palette (`Ctrl/Cmd+Shift+P`): it finds R, checks the course packages, and installs any
that are missing.

**4. Start your first journal entry.** Copy `_templates/journal-entry.md` into
`01_Journal/`, rename it for the week, and write.

Step-by-step walkthrough with screenshots:
<https://aura-lab.siue.edu/v2v-hub/resources/workspace-setup.html>

## What is in here

```
00_Inbox/           Quick capture. Anything not yet filed.
01_Journal/         Weekly reading reflections. Committed here, submitted in Blackboard.
02_Literature/      Reading notes and Zotero annotations.
03_Project/         Your research project, in the order you build it:
  01_Prospectus/      Research design (Chapter 6)
  02_Codebook/        Data dictionary (Chapter 8)
  03_Data/            Sampled data and analysis (Chapters 10 to 12)
  04_Drafts/          Drafts and the final White Paper (Chapters 13 to 14)
04_Resources/       PDFs, images, attachments.
_templates/         Reusable starting points for journals and codebooks.
.vscode/            Shared extensions and settings.
.devcontainer/      The Codespace route: R and the course package preinstalled on GitHub.
.github/            Copilot's instructions for this course. Leave it in place.
```

`03_Project/` is ordered the way the term is ordered. You will fill it roughly in
sequence, and by the end it holds the whole trail from your first research question to
the finished White Paper.

## Recommended extensions

| Extension | Why |
| --- | --- |
| **Quarto** | Renders the `.qmd` files you write from Chapter 10 onward |
| **R** | Runs R inside VS Code, so the workbook labs work in this same window |
| **GitLens** | Makes your own commit history legible, which matters when you need to find what you changed three weeks ago |
| **AURA Lab R Companion** | **Check my setup** for your course, and **Explain an R error** when a line breaks; later releases add menus that write commented R code into your script |

## Why commit your work

Committing gives you three things: a backup that is not on your laptop, a full history
you can walk backward through, and a record of your work that stays yours after the
course ends.

**Committing is not submitting.** Graded work is turned in through Blackboard, under the
assignment for that week. Commit your work as well, always -- but an entry that was
committed and never submitted has not been turned in.

It also builds the version-control habit you use again for the final portfolio, which is
published from a repository like this one.

Commit early and often. A commit is cheap. Losing a week of work is not.

## Working notes

- **Plain Markdown only.** No `[[wiki-links]]`. To point at another file, use a normal
  relative Markdown link: `[the codebook](../03_Project/02_Codebook/codebook.md)`. Those
  work on GitHub, in VS Code, and in anything you export to later.
- **Do not commit raw data you are not licensed to redistribute.** `03_Project/03_Data/`
  is for your sampled working data. If a dataset came with terms, respect them.
- **Nothing personally identifying about the people in your data.** This is a research
  methods course and the standard applies to your own workspace too.

## Course links

- Course site: <https://aura-lab.siue.edu/v2v-hub/>
- Textbook, *From Vibes to Variables*: <https://aura-lab.siue.edu/v2v/>
- `v2v` R package, the Twitch practice corpus: <https://github.com/AURA-Lab-SIUE/v2v-r>

## License

The template itself (the folder structure, the files in `_templates/`, and this README) is CC BY 4.0. The license covers the template, not the work you create in your own copy; your journals, notes, and project files are yours.

---

AURA Lab, Department of Mass Communications, Southern Illinois University Edwardsville.
