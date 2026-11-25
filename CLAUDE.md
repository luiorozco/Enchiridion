# Enchiridion

This repository builds the new lui-orozco.com, served with GitHub Pages.
Its content is compiled in a separate folder, the content folder, whose path is in `CLAUDE.local.md`.
`CLAUDE.local.md` is git-ignored; never commit it, and never write its path anywhere else.

## The content folder

Read these files in the content folder at the start of every session:
- `Plan.md`, for the goal, the steps and their state, and the decisions so far.
- `Purpose.md`, for what the site is for, who reads it, and what search needs from the build.
- `Handover.md`, for what the content folder delivers and how; the data model follows it, never the other way round.
- `CLAUDE.md` § What may become public, for what may enter this repository.

Do the step of `Plan.md` that your prompt names.
Update its State in `Plan.md`, in the content folder.
Record a decision about the code or the design of the site in this repository.
Copy nothing from the content folder into this repository; only the hand-over brings content in.

## What may become public

Everything committed here is public for good, because git keeps every file it was ever given.

- Commit nothing that the content folder's rules on what may become public forbid.
- Never write a path of the content folder, or one of its provenance comments, into a committed file; the hook in `.githooks/` refuses both.
- Never commit masters, editable sources, video or archives; `.gitignore` keeps them out as insurance.
- Commit generated images, such as example directions and mock-ups, only when they show nothing that is not already public or cleared.
- Never commit images made by others, such as mood-board references; committing them redistributes them, so link to them instead.
- Commit a font only when its licence allows public redistribution, such as the SIL Open Font License, and put its licence file beside it.

## The hand-over

- `Handover/` reaches this repository whole, through the hand-over script in the content folder.
- Never edit, add to or delete from `Handover/`; `.claude/settings.json` denies it.
- Read `Handover/` where it is; the build never copies or changes it.
- The name `Handover/` is pending a decision in the content folder; rename every reference here once it is made.

## Git

- Commit and push only when Lui asks.
- Write each commit message as a short imperative subject in British English.
- After cloning, run `git config core.hooksPath .githooks`.

## Conventions

- Write British English, except inside quoted titles, which keep their original spelling.
- Use one term per thing, the content folder's terms included: an entry is any item on the site, and a project is one kind of entry.
- Write short sentences, in the active voice; write instructions as imperatives, one per line.
- Write one sentence per line in Markdown.
- Save files as UTF-8 with LF line endings; `.gitattributes` enforces LF.
- Name code and framework files as their language and framework expect.
- Name a Markdown document this repository creates in Hyphenated-PascalCase, as in `Export-Profiles.md`; `README.md`, `CLAUDE.md` and `LICENSE` keep their conventional names.
- State the date of a decision taken here in visible text, as in "Decided 25 November 2026"; add no provenance comments, because git's history is the rest of the record.
