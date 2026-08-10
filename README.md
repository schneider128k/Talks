# Talks

Slides and write-ups of talks I have given, with the LaTeX sources they were made from.

I was able to reconstruct all of my presentations, going back to my time as an
undergraduate student in Karlsruhe. The oldest one here is from February 1996, in my
third semester. I did not expect that anything from then had survived.

It had, but not in any one place. Thirty years of material sat in layers of backups —
one machine copied onto the next, a directory carried from a DOS floppy to a Unix
account to a laptop to a cloud drive, and mostly never looked at again. I went through
those layers with the help of AI, which read the backups and matched files by their
contents rather than by their names. That is what made the difference: the 1996 talk is
in a folder called `Proseminar`, in files called `prosem5.tex` and `profolie.tex`, and
no search for "talk" or "Vortrag" would ever have found it.

Not everything was in folders. Some documents of that period survived only as
attachments inside old Unix mailbox files, in backups of mail accounts I stopped using
twenty years ago. That is not where the talks in this repository came from — those were
on disk — but it is the reason I went through the mail as well.

This has sentimental value for me, which is the main reason the repository exists.

## Minimal changes

For the old documents, in particular the ones from the 1990s, I tried to change as
little as possible. The only aim was to make them compile on a modern LaTeX
distribution. Nothing was rewritten, reformatted or improved.

The 1996 proseminar differs from what I wrote then by two lines. `\documentstyle` became
`\documentclass` plus `\usepackage`, because LaTeX 2.09 syntax no longer exists, and I
fixed the date of the write-up so that rebuilding it does not stamp it with today's. The
page count is the same as in 1996 — 6 and 12 pages. The typos are the ones I made at the
time, and I left them there.

## Talks

In reverse chronological order.

### 1996

**Proseminar, Universität Karlsruhe (TH) — February 1996**
*Fraktale Fouriertransformation* — the fractional Fourier transform, its eigenfunctions,
and its realisation in a quadratic GRIN medium.
Supervisor: Michael Schmid.
Institut für Algorithmen und Kognitive Systeme (IAKS), Fakultät für Informatik,
Prof. Dr. Thomas Beth, Universität Karlsruhe (TH). The institute no longer exists, and
the university is now the Karlsruhe Institute of Technology (KIT).

[→ Presentation (PDF)](1996-02_fractal_fourier_transform/fractal_fourier_presentation.pdf) ·
[→ Report (PDF)](1996-02_fractal_fourier_transform/fractal_fourier_report.pdf) ·
[sources](1996-02_fractal_fourier_transform/)

## How a talk is arranged

One folder per talk, named `YYYY-MM_short-title`. Each holds the LaTeX sources and the
PDF built from them:

```
1996-02_fractal_fourier_transform/
    fractal_fourier_presentation.tex    the slides
    fractal_fourier_presentation.pdf
    fractal_fourier_report.tex          the written version
    fractal_fourier_report.pdf
```

Most of the early talks come in two parts, because that is how a German *Proseminar* or
*Seminar* worked: a *Vortrag*, the talk itself, and an *Ausarbeitung*, a written account
of it handed in afterwards.

## Building

```
pdflatex fractal_fourier_presentation.tex
pdflatex fractal_fourier_report.tex && pdflatex fractal_fourier_report.tex
```

The report is run twice for its table of contents. Both need `german.sty` and `a4.sty`,
which ship with MiKTeX and TeX Live.

## Licensing

The talks — sources, figures and compiled PDFs — are under
[CC BY 4.0](LICENSE-CC-BY-4.0). Talks given jointly with other people are marked as such
in their entry above and are not mine alone to license.
