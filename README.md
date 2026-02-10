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
- `latexmk` — build orchestrator

## License

MIT
