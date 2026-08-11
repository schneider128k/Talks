# Talks, posters and lecture notes

Slides, posters and write-ups from my academic life, with the LaTeX sources they were
made from.

Talks are the largest part of it, and the repository keeps their name. But not everything
here is a talk. There are conference posters; there are lecture notes I wrote up for
courses given by other people, where the mathematics is theirs and the writing is mine;
and there are a few longer pieces of written work that have a repository of their own and
are listed here only for the record.

I was able to reconstruct all of my presentations, going back to my time as an
undergraduate student in Karlsruhe. The oldest one here is from February 1996, in my
third semester. I did not expect that anything from then had survived.

It had, but not in any one place. Thirty years of material sat in layers of backups —
one machine copied onto the next, a directory carried from a DOS floppy to a Unix
account to a laptop to a cloud drive, and mostly never looked at again. I went through
those layers with the help of AI, which read the backups and matched files by their
contents rather than by their names. That is what made the difference: filenames on those
machines were limited to eight characters, and after thirty years of copying from one
machine to the next, the contents are a more reliable guide than the names.

This has sentimental value for me, which is the main reason the repository exists.

## Minimal changes

The older sources, in particular those from the 1990s, were written for versions of
LaTeX that no longer exist. In all of them I changed as little as possible, and only
what was needed to make them compile on a modern distribution.

Nothing was rewritten, reformatted or improved, and I corrected no mistakes. What is
here is what I wrote at the time.

## The documents

**[→ DOCUMENTS.md](DOCUMENTS.md)** — everything in reverse chronological order, with its
occasion, date and supervisors, and links to the presentation and the written version.

## How an entry is arranged

One folder per entry, named `YYYY-MM_short-title`. Each holds the LaTeX sources and the
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

Where the *Ausarbeitung* went into a printed seminar volume it is split in two, as it was
at the time: a `_report.tex` that carries the volume's title page and pulls in a
`_chapter.tex` holding the text itself. The `haupt.sty` and `unilogo.tex` beside them are
the seminar's own template, kept unchanged so the document still builds.

A few entries have no folder at all. Those are longer pieces of written work that live in
a repository of their own; [DOCUMENTS.md](DOCUMENTS.md) records them in their place in the
sequence and links to that repository, rather than duplicating the sources here.

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

A few of the oldest sources are left exactly as they were, because bringing them up to a
modern LaTeX would have changed how they look; the PDF beside those is the one typeset at
the time.

## Licensing

Everything here — sources, figures and compiled PDFs — is under
[CC BY 4.0](LICENSE-CC-BY-4.0). Work made jointly with other people is marked as such
in [DOCUMENTS.md](DOCUMENTS.md) and is not mine alone to license.

The same goes for the few files that came with a seminar template or with the institute's
shared LaTeX setup rather than from me — `haupt.sty`, `mathsym.sty`, `boldmath.sty`,
`diplom.sty`, and `unilogo.tex` and `logo.eps`, the last two being the university's and
the institute's marks. They are here only so that the documents still build, and they are
not my work.

The lecture notes on public key cryptography are a special case: the writing is mine, but
the course was Dr. Willi Geiselmann's and the mathematics and the choice of material in
them are his, so they are not mine alone to license either.
