---
layout: default
title: Iain Phillips
---

# LaTeX for your thesis

[Download](luthesis.zip)

Read the docs - last updated September 2021. Note that to successfully
format the luthesis-example.tex file (which is where the documentation
is) you need to comment line 10 (\\setcoofile\....)

Note this is not offcially supported within Loughborough. If you spot
something out of data let me know and I\'ll fix, but errors caused by
using this class will be considered your own.

## Archiving your thesis source code

As luthesis (and the Loughborough Regulations) are under constant
change, it\'s very possible that the version you use in your thesis
today will produce different results in subsequent years. Therefore, if
you plan to archive the source of your thesis, archive the version of
luthesis that you used at the same time.

## Useful other tools

-   [Daum Equation
    Editor](https://chrome.google.com/webstore/detail/daum-equation-editor/dinfmiceliiomokeofbocegmacmagjhe)

## Formatting code listings

A common question. Use the listings package and I suggest the following
in the preamble:

Code to define a language console output, such as collected by the
*script* command

    \lstdefinelanguage{console}{basicstyle=\ttfamily\footnotesize}

An environment to go with this

    \lstnewenvironment{console}{\setstretch{0.9}\lstset{language=console}}{}}

A command to input code from a file.

    \newcommand{\inputconsole}[1]{\begin{spacing}{0.9}\lstinputlisting{#1}\end{spacing}}

Which can be used like this:

    \inputconsole{iain}

Code to create a python environment:

    \lstnewenvironment{python}%
        {\setstretch{1.0}\lstset{language=Python,basicstyle=\footnotesize,%
        stringstyle=\ttfamily,frame=single,numberstyle=\tiny,numbers=left}}%
        {}
