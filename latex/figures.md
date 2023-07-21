# Figures, tables and floating environments

- LaTeX knows where it's best to put figures.  It is right.  Sometimes things are not what you want them to be.

- use `[htbp]` as the qualifier for any floating environment (e.g. figure or table).  This will make LaTeX try it's best to put a figure close to where you want it.



- LaTeX algorithm puts out figures in order and when it can find an appropriate space.  If you have a lot of figures needing a lot of space compared to the space needed for text, then they could be saved up and printed at the end of a chapter (or document).
  
- `\clearpage` will instruct latex to put out the floats now and start a new page.  This may leave a blank and of page, but this is sometimes better than the alternatives.