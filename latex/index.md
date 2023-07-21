---
title: LaTeX packages
layout: default
---

# LaTeX questions


## Errors/Warnings

It is very good practice to fix all the errors and warnings produced by
latex when compiling a document. Systems such as Overleaf and TeXShop
often appear to compile the document anyway, but this is short-term bad
thinking as many of your collaborators will use different systems.

Some of the warnings are important and having too many will hide the
important ones away. This will not be good for you in the long term.

## Interword spacing after fullstops

The eagle-eyed will notice that space between words is a different
length to that between sentences. LaTeX distinguishes-interword space
from inter-sentence space by observing the full stop characters. So an
inter-sentence space is placed after every full stop. However, there are
exceptions and places where this is wrong.

- If the letter before the full stop is a capital then LaTeX assumes it
  is an acronym, think I.B.M. and NOT the end of a sentence. To fix this
  use the `\@.` instend of a simple `.`
- If the full stop does not actually mark the end of a sentence, usually
  e.g. or in someone's initials, say `I. W. Phillips`. Here put a \\
  between the . and the following space. This indicates that this should
  be an interword space. You can also use a `~` (tilde) character which
  makes the space the same size, but prevents a line break occurring at
  that point, which is often useful.

## Other things

- [Source layout tips](tips)
- [Reducing space around headings and titles](whitespace)
- [Where have my figures gone?](figures)
