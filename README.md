# Research record

What I have published, the talks and posters I have given, and the notes and coursework I wrote as
a student in Karlsruhe — kept as three lists, in chronological order, with the LaTeX sources
wherever I still have them. It runs from 1996 to the present, through the university years and the
industrial ones that followed.

## How this is organised

Three lists, each in chronological order, oldest first.

**[→ PUBLICATIONS.md](PUBLICATIONS.md)** — papers and theses. Almost everything is on the arXiv,
so this is a list of links rather than a store of sources: each entry points at the preprint and,
where there is one, at the published version.

The three theses each have a dedicated repository of their own, linked in place. The Studienarbeit
and the Diplomarbeit go further than the thesis text: alongside the original implementation, where
it survives, each holds a modern Python reimplementation of the algorithm — finished for the
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
thesis repositories instead — the original implementations, where they survive, and the modern
Python reimplementations — and each of those carries its own licence for it.

---

## How the old material survived

This concerns the Karlsruhe years, and mostly the oldest part of them. Nothing from 2000 onwards had
to be recovered — those papers were published and are on the arXiv.

The early work was written on a PC and carried on floppy disks over to the Sun workstations at the
institute, where my university account lived. When I left Karlsruhe I burned that account onto a
CD-ROM, and then moved continents. The disc was copied onto one machine after another for the next
twenty years, mostly unread, and that is the only reason any of it still exists. The oldest thing
here is from February 1996, my third semester. I did not expect that anything from then had survived.

It had, but not in one place. Putting it back together turned out to be a genuinely enjoyable piece
of digital forensics and archaeology. The same file existed in a dozen copies under a dozen names, so
things had to be matched by their contents rather than by their names — filenames on those machines
were limited to eight characters, and after that much copying the contents are the more reliable
guide. Much of the history had to be read off the artifacts rather than the documents: when a build
was last run, which version of LaTeX a source expected, what a compiler had complained about at the
time.

Two papers I had almost forgotten came back with it: one written out of the Studienarbeit, with
Michael Schmid and Thomas Beth, and one written out of the Diplomarbeit, with Gaétan Haché.
Neither was ever published, and I am glad they are not lost.

## Thomas Beth

Thomas Beth was my *Doktorvater*. He supervised my dissertation, and before it my Proseminar and my
Studienarbeit, and he was a co-author on much of the early work here.

His interests were unusually wide: design theory and cryptography, where he was one of the founders
of the field in Germany, then optical and diffractive computing, and then quantum computing. I took
his course on quantum computing as an undergraduate, held shortly after Shor published his factoring
algorithm. I had always wanted to do doctoral research; that course is what made it this subject.

He shaped my scientific education — what I think is worth asking, and the habit of turning a problem
over and over until it looks different. I owe him a great deal, and I am grateful for it.

He died in 2005, at fifty-five, far too young. Three obituaries, the first of them written by three
of my colleagues at the IAKS:

- Markus Grassl, Andreas Klappenecker and Martin Rötteler, *In Memoriam: Thomas Beth*, Quantum
  Information Processing **5** (2006), 1–4 —
  [doi](https://doi.org/10.1007/s11128-005-0006-x)
- Gerd Leuchs, Wolfgang Mathis and Wolfgang Schleich, *Nachruf auf Thomas Beth*, *Physik Journal*
  **4** (2005), Nr. 11 —
  [pdf](https://pro-physik.de/zeitschriften/download/16138)
- Andy Clark for the IACR —
  [iacr.org](https://www.iacr.org/misc/beth.html)

The IAKS — the Institut für Algorithmen und Kognitive Systeme — no longer exists, and Universität
Karlsruhe (TH) is now the Karlsruhe Institute of Technology (KIT).
