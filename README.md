# latexcolor

This was an attempt to make latex/pdflatex's ouput readable enough that I wouldn't skim over it.

- Tries to be smart about multiple messages on a line
- Categorizes messges into initialisation, verbosity, typesetting, warnings/errors, basic messages, and unknown
- by default surpresses initialisation and verbosity 
- presents each message on its own line, with the page number it's probably on

So it shows:

![simpler output](/screenshots/simpler.png?raw=true)

instead of the original:

```
This is pdfTeX, Version 3.14159265-2.6-1.40.18 (TeX Live 2017/Debian) (preloaded format=pdflatex)
 restricted \write18 enabled.
entering extended mode
(./Graph.tex
LaTeX2e <2017-04-15>
Babel <3.18> and hyphenation patterns for 7 language(s) loaded.
(/usr/share/texlive/texmf-dist/tex/latex/base/article.cls
Document Class: article 2014/09/29 v1.4h Standard LaTeX document class
(/usr/share/texlive/texmf-dist/tex/latex/base/size10.clo))
(/usr/share/texlive/texmf-dist/tex/latex/graphics/graphicx.sty
(/usr/share/texlive/texmf-dist/tex/latex/graphics/keyval.sty)
(/usr/share/texlive/texmf-dist/tex/latex/graphics/graphics.sty
(/usr/share/texlive/texmf-dist/tex/latex/graphics/trig.sty)
(/usr/share/texlive/texmf-dist/tex/latex/graphics-cfg/graphics.cfg)
(/usr/share/texlive/texmf-dist/tex/latex/graphics-def/pdftex.def)))
(/usr/share/texlive/texmf-dist/tex/latex/wrapfig/wrapfig.sty)
(/usr/share/texlive/texmf-dist/tex/latex/graphics/color.sty
(/usr/share/texlive/texmf-dist/tex/latex/graphics-cfg/color.cfg))
(/usr/share/texlive/texmf-dist/tex/latex/eso-pic/eso-pic.sty
(/usr/share/texlive/texmf-dist/tex/generic/oberdiek/atbegshi.sty
(/usr/share/texlive/texmf-dist/tex/generic/oberdiek/infwarerr.sty)
(/usr/share/texlive/texmf-dist/tex/generic/oberdiek/ltxcmds.sty)
(/usr/share/texlive/texmf-dist/tex/generic/oberdiek/ifpdf.sty)))
(/usr/share/texlive/texmf-dist/tex/latex/amsfonts/amsfonts.sty)
(/usr/share/texlive/texmf-dist/tex/latex/hyperref/hyperref.sty
(/usr/share/texlive/texmf-dist/tex/generic/oberdiek/hobsub-hyperref.sty
(/usr/share/texlive/texmf-dist/tex/generic/oberdiek/hobsub-generic.sty))
(/usr/share/texlive/texmf-dist/tex/generic/ifxetex/ifxetex.sty)
(/usr/share/texlive/texmf-dist/tex/latex/oberdiek/auxhook.sty)
(/usr/share/texlive/texmf-dist/tex/latex/oberdiek/kvoptions.sty)
(/usr/share/texlive/texmf-dist/tex/latex/hyperref/pd1enc.def)
(/usr/share/texlive/texmf-dist/tex/latex/latexconfig/hyperref.cfg)
(/usr/share/texlive/texmf-dist/tex/latex/url/url.sty))
(/usr/share/texlive/texmf-dist/tex/latex/hyperref/hpdftex.def
(/usr/share/texlive/texmf-dist/tex/latex/oberdiek/rerunfilecheck.sty))

LaTeX Warning: Unused global option(s):
    [a4].

(./Graph.aux)
(/usr/share/texlive/texmf-dist/tex/context/base/mkii/supp-pdf.mkii
[Loading MPS to PDF converter (version 2006.09.02).]
) (/usr/share/texlive/texmf-dist/tex/latex/oberdiek/epstopdf-base.sty
(/usr/share/texlive/texmf-dist/tex/latex/oberdiek/grfext.sty)
(/usr/share/texlive/texmf-dist/tex/latex/latexconfig/epstopdf-sys.cfg))
(/usr/share/texlive/texmf-dist/tex/latex/hyperref/nameref.sty
(/usr/share/texlive/texmf-dist/tex/generic/oberdiek/gettitlestring.sty))
(/usr/share/texlive/texmf-dist/tex/latex/amsfonts/umsa.fd)
(/usr/share/texlive/texmf-dist/tex/latex/amsfonts/umsb.fd) (./Graph.toc)
[1{/var/lib/texmf/fonts/map/pdftex/updmap/pdftex.map} <./d.pdf>] [2] [3]
[4] (/usr/share/texlive/texmf-dist/tex/latex/base/omscmr.fd) [5]
Overfull \hbox (28.45276pt too wide) in paragraph at lines 391--392
 []

Underfull \hbox (badness 4060) in paragraph at lines 393--393
[]\OT1/cmr/m/n/10 Figure 1: []Flat track-
[6] [7 <./song.pdf> <./dep.pdf>]

LaTeX Warning: `h' float specifier changed to `ht'.

[8] [9 <./dep2.pdf>] [10] [11] [12] [13]
Underfull \hbox (badness 5475) in paragraph at lines 864--864
[][][]\OT1/cmr/m/n/8 Graph Repos-i-tory Query Lan-guage, see [][]$\OT1/cmtt/m/n
/8 http : / / www . uni-[]koblenz . de / FB4 / Institutes / IST / AGEbert /
[14] [15] (./Graph.bbl) [16] (./Graph.aux) )
(see the transcript file for additional information)pdfTeX warning (dest): name
{Hfootnote.20} has been referenced but does not exist, replaced by a fixed one

</usr/share/texlive/texmf-dist/fonts/type1/public/amsfonts/cm/cmbx10.pfb></usr/
share/texlive/texmf-dist/fonts/type1/public/amsfonts/cm/cmbx12.pfb></usr/share/
texlive/texmf-dist/fonts/type1/public/amsfonts/cm/cmmi10.pfb></usr/share/texliv
e/texmf-dist/fonts/type1/public/amsfonts/cm/cmr10.pfb></usr/share/texlive/texmf
-dist/fonts/type1/public/amsfonts/cm/cmr12.pfb></usr/share/texlive/texmf-dist/f
onts/type1/public/amsfonts/cm/cmr17.pfb></usr/share/texlive/texmf-dist/fonts/ty
pe1/public/amsfonts/cm/cmr6.pfb></usr/share/texlive/texmf-dist/fonts/type1/publ
ic/amsfonts/cm/cmr7.pfb></usr/share/texlive/texmf-dist/fonts/type1/public/amsfo
nts/cm/cmr8.pfb></usr/share/texlive/texmf-dist/fonts/type1/public/amsfonts/cm/c
msy10.pfb></usr/share/texlive/texmf-dist/fonts/type1/public/amsfonts/cm/cmti10.
pfb></usr/share/texlive/texmf-dist/fonts/type1/public/amsfonts/cm/cmtt10.pfb></
usr/share/texlive/texmf-dist/fonts/type1/public/amsfonts/cm/cmtt8.pfb>
Output written on Graph.pdf (16 pages, 246090 bytes).
Transcript written on Graph.log.

```



I wrote this just to see whether it'd work and be worth doing, and a decade ago, and was restructured a few times so some codepaths are obscurely structured, so it's going to be messy.

I'm putting it here to see if other people have a use for it. If so, you probably want to use it for inspiration and not would _not_ want to adopt this into other software as-is.


In particular, the splitting between messages needs a cleaner responsibility.




Use as a pipe on latex/pdflatex's output, so e.g.:
    latex foo.tex | colorlatex

## arguments

```
Options:
   -i, -I   Suppress/show initialisation, package imports   (default: suppress)
   -v, -V   Suppress/show verbose details                   (default: suppress)
   -m, -M   Suppress/show basic messages                    (default: show)
   -t, -T   Suppress/show typesetting remarks               (default: show)
   -w, -W   Suppress/show warning and error messages        (default: show)
   -u, -U   Suppress/show unknown messages                  (default: show)
   -a, -A   Suppress/show everything (can be combined)      (default: show)

   By default, only non-common hints are shown.
   -d       Suppress all hints
   -e       Show all hints

   -c, -C   Suppress, force color output      (default: guess color support by term type)
   -l       Suppress page numbers in output
   -D       show message type in output (mostly for debug)

   -h       Show this help
```
