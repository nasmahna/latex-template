# LaTeX Template Collection

Simple and practical LaTeX templates for:
- Resume/CV
- Thesis cover page
- Thesis contents page

## Files Included

- `resume.tex`  
  A one-page resume template with sections for summary, experience, education, skills, and projects.

- `thesis-cover.tex`  
  A clean thesis cover page template.  
  Current sizing setup:
  - Thesis title: `16pt`
  - Other text (name, university info, supervisor, date): `12pt`

- `thesis-list-of-pages.tex`  
  A thesis contents page template using `\tableofcontents` with sample chapter structure.

## Requirements

Install a LaTeX distribution:
- macOS (full): [MacTeX](https://www.tug.org/mactex/)
- macOS (lightweight): `brew install --cask basictex`

Optional build helper:
- `latexmk` (recommended)

## How to Compile

From this project folder:

```bash
pdflatex resume.tex
pdflatex thesis-cover.tex
pdflatex thesis-list-of-pages.tex
```

Or with `latexmk`:

```bash
latexmk -pdf resume.tex
latexmk -pdf thesis-cover.tex
latexmk -pdf thesis-list-of-pages.tex
```

Generated output files:
- `resume.pdf`
- `thesis-cover.pdf`
- `thesis-list-of-pages.pdf`

## Notes
- If `pdflatex: command not found`, install MacTeX/BasicTeX first.
- The templates contain placeholders (name, email, university, thesis title, etc.). Replace them with your real data.
- For table of contents updates, compile at least twice so page numbers are refreshed.
