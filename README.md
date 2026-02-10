# Setup LaTeX Action

GitHub Action to install TeX Live with XeLaTeX support.

## Usage

```yaml
- name: Setup LaTeX
  uses: damoun/setup-latex-action@v1
- name: Compile document
  run: latexmk -xelatex document.tex
```

## Installed Packages

- `texlive-xetex` — XeLaTeX engine, fontspec, xltxtra
- `texlive-latex-extra` — progressbar, xifthen, titlesec, enumitem
- `texlive-latex-recommended` — base dependency set
- `texlive-fonts-recommended` — PostScript fonts (pzdr, etc.)
- `latexmk` — build orchestrator

## Performance

First run: ~1-2 minutes (installs packages and populates cache)
Subsequent runs: ~10-30 seconds (restores from cache)

Caches `/usr/share/texlive`, `/usr/share/texmf`, and `/var/lib/texmf`.

## License

MIT
