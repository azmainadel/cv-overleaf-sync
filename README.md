# CV Overleaf Sync

LaTeX source for my CV, kept in sync between Overleaf and GitHub.

## Structure

```text
main.tex                 Preamble, custom commands, header, and section order
sections/
  experience.tex         Work experience
  skills.tex             Technical skills
  projects.tex           Projects and research
  education.tex          Education
  extras.tex             Mentorship and community (teaching, judging, organizing)
```

Sections appear in the order they are `\input` in `main.tex`. To reorder the CV, move
the `\input` lines there.

## Editing

- Content lives in `sections/`. Layout and the custom commands (`\resumeSubheading`,
  `\resumeItem`, and so on) live in `main.tex`.
- Use `--` for date ranges, and keep tech names consistent (`Node.js`, `React`, `Next.js`).
- The CV targets about two pages. Check the page count after larger edits.

## Syncing

Overleaf is linked to this repository through its GitHub sync.

- Pull from Overleaf before editing locally, so the two don't diverge.
- If a file is renamed here, rename it in Overleaf too, or the next sync may conflict.
- Compile in Overleaf. There is no local LaTeX toolchain set up.
