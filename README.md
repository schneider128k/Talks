# Research record

What I have published, the talks and posters I have given, and the notes and coursework I wrote as
a student in Karlsruhe — kept as three lists, in reverse chronological order, with the LaTeX sources
behind them. It runs from 1996 to the present, through the university years and the industrial ones
that followed.

## How this is organised

Three lists, each in reverse chronological order, newest first.

**[→ PUBLICATIONS.md](PUBLICATIONS.md)** — papers and theses. Almost everything is on the arXiv,
so this is a list of links rather than a store of sources: each entry points at the preprint and,
where there is one, at the published version.

The three theses each have a dedicated repository of their own, linked in place. The Studienarbeit
and the Diplomarbeit go further than the thesis text: alongside the original implementation, where
there is one, each holds a modern Python reimplementation of the algorithm — finished for the
diffractive beam shaper, still in progress for Brill-Noether. I intend to carry that work further.

**[→ TALKS.md](TALKS.md)** — talks and posters, with the occasion, the date, the people the work
was done with, and links to the slides or the poster and to the sources.

**[→ NOTES.md](NOTES.md)** — the lecture notes on public key cryptography, the Übung on the
entropy function, and the seminars and proseminars. Two of the entries are write-ups of courses
given by other people, where the mathematics is theirs and the writing is mine.

Entries in TALKS.md and NOTES.md are being added one at a time, and the talks I gave after 2020
are not yet reconstructed. The recovery itself is finished; the publishing is not.

## Folder layout

Everything with sources lives under `documents/`, one folder per entry, named
`YYYY-MM_short-title`, holding the LaTeX sources and the PDF built from them:

```
documents/1996-02_fractal_fourier_transform/
    fractal_fourier_presentation.tex    the slides
    fractal_fourier_presentation.pdf
    fractal_fourier_report.tex          the written version
    fractal_fourier_report.pdf
```

Most of the early entries come in two parts, because that is how a German *Proseminar* or
*Seminar* worked: a *Vortrag*, the talk itself, and an *Ausarbeitung*, a written account of it
handed in afterwards.

Where the *Ausarbeitung* went into a printed seminar volume it is split in two, as it was at the
time: a `_report.tex` that carries the volume's title page and pulls in a `_chapter.tex` holding
the text itself. The `haupt.sty` and `unilogo.tex` beside them are the seminar's own template,
kept unchanged so the document still builds.

Some entries have no folder. Those are papers that live on the arXiv, and longer pieces of written
work that have a repository of their own; the lists record them in their place in the sequence and
link out, rather than duplicating anything.

## Minimal changes

The older sources, in particular those from the 1990s, were written for versions of LaTeX that no
longer exist. In all of them I changed as little as possible, and only what was needed to make
them compile on a modern distribution.

Nothing was rewritten, reformatted or improved, and I corrected no mistakes. What is here is what
I wrote at the time.

## Building

Every entry with sources builds from them in its own folder with

```
pdflatex <file>.tex
```

run twice where the document has a table of contents. A recent MiKTeX or TeX Live is enough.

The slide sources that take their colour from `colordvi` are the exception. They are built

```
latex <file>.tex
dvips -Ppdf -G0 <file>.dvi
ps2pdf <file>.ps
```

A few of the oldest sources are left exactly as they were, because bringing them up to a modern
LaTeX would have changed how they look; the PDF beside those is the one typeset at the time.

## Licensing

Everything here — sources, figures and compiled PDFs — is under
[CC BY 4.0](LICENSE-CC-BY-4.0). Work made jointly with other people is marked as such in the
lists, where the co-authors are named.

The same goes for the few files that came with a seminar template or with the institute's shared
LaTeX setup rather than from me — `haupt.sty`, `mathsym.sty`, `boldmath.sty`, `diplom.sty`, and
`unilogo.tex` and `logo.eps`, the last two being the university's and the institute's marks. They
are here only so that the documents still build, and they are not my work.

The lecture notes on public key cryptography are a special case: the writing is mine, but the
course was Dr. Willi Geiselmann's, and the mathematics and the choice of material in them are his.

There is no code in this repository, so there is no software licence here. The code sits in the
thesis repositories instead — the original implementations and the modern Python reimplementations —
and each of those carries its own licence for it.
