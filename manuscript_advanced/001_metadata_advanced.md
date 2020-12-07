---
# METADATA
# see https://maehr.github.io/academic-pandoc-template/markdown.html
lang: it # like en, en-UK, en-US, fr, it, it-IT, ...
title: "My advanced book"
subtitle: "subtitle for this book"
subject: "this goes in the PDF metadata"
author: "Stefano Cecere"
date: 07-12-2020
keywords: "Technology, Philosophy, OpenSource"
# thanks: "So Long, and Thanks for All the Fish"
publisher: My Publisher
rights: © 2020 Stefano Cecere, CC BY-NC
identifier:
- scheme: ISBN-10
  text: 1234567890

mainfont: Arial
sansfont: Arial
# mainfont: DejaVuSerif.ttf
# #mainfont: ProximaNova-Reg.ttf
# sansfont: DejaVuSans.ttf
# monofont: DejaVuSansMono.ttf 
# mathfont: texgyredejavu-math.otf 
# sansfont: Calibri.ttf
# monofont: Consolas.ttf

# titlepage: false
# titlepage-color: "FFFFFF"
# titlepage-text-color: "000000"
# titlepage-rule-color: "CCCCCC"
# titlepage-rule-height: 4
# disable-header-and-footer: false
# header-left:
# header-center:
# header-right:
# footer-left: "© Alexey Gumirov"
# footer-center: "License: WTFPL"
# footer-right:

#titlepage-background: manuscript/_img/cover.png
#page-background:  manuscript/_img/cover.png

# Formatting
toc-title: "Index"
toc: true
toc_depth: 2
lof: false # List of figures
lot: false # List of tables

documentclass: book # See https://en.wikibooks.org/wiki/LaTeX/Document_Structure#Document_classes
classoption: [titlepage, onecolumn, openright, draft]
geometry: [paperwidth = 5.5in, paperheight = 8.5in, bindingoffset=0mm, inner=18mm, outer=12mm, top=18mm, bottom=18mm] # See https://ctan.org/pkg/geometry

fontsize: 11pt
onehalfspacing: true

## see https://github.com/Wandmalfarbe/pandoc-latex-template/commit/948150d1720fd3d2afd2318bbe5bc069377ed2c9
# pandoc-latex-environment:
#   tcolorbox: [box]
#   info-box: [info]
#   warning-box: [warning]
#   error-box: [error]


# subparagraph: yes
# - \usepackage{titlesec}
# - \titleformat*{\section}{\Large\bfseries\sffamily\color{red}}

#  - \usepackage{titlesec}

#  - \usepackage{bookmark}
#  - \titleformat*{\section}{\fontsize{16}{20}\filcenter\selectfont}
#  - \titleformat*{\subsection}{\fontsize{13}{15}\filcenter\selectfont}

header-includes:
#  - \setcounter{tocdepth}{1}
#  - \tableofcontents
  
  - \usepackage{setspace}
#  - \onehalfspacing

#  - \usepackage{titlesec}
#  - \titleformat*{\section}{\fontsize{16}{20}\filcenter\selectfont}
#  - \titleformat*{\subsection}{\fontsize{13}{15}\filcenter\selectfont}

# headeing https://en.wikibooks.org/wiki/LaTeX/Customizing_Page_Headers_and_Footers
#  - \usepackage{fancyhdr}  
  - \pagestyle{headings}
#  - \markboth{John Smith\hfill On page styles\hfill}
#  - \markright{alta cosa}
#  - \fancyhead[RO]{\slshape \rightmark}
#  - \fancyhead[LE]{\slshape \leftmark}
#  - \fancyhead[LO,RE]{\thepage}
#  - \renewcommand{\headrulewidth}{0pt}
#  - \renewcommand{\footrulewidth}{0pt}

## multicolumn
  - \usepackage{multicol}
  - \newcommand{\hideFromPandoc}[1]{#1}
  - \hideFromPandoc{
      \let\Begin\begin
      \let\End\end
    }

## boxes
# colors: https://latexcolor.com/
  - \usepackage{tcolorbox}
  - \definecolor{color_box1}{rgb}{0.93, 0.53, 0.18}
  - \definecolor{color_box2}{rgb}{0.13, 0.67, 0.8}
  - \definecolor{quotecolor}{rgb}{0.36, 0.54, 0.66}
  - \newtcolorbox{myquote}{colback=white, colframe=quotecolor}
  - \renewenvironment{quote}{\begin{myquote}}{\end{myquote}}
  - \newtcolorbox{box1}{colback=white, colframe=color_box1, fonttitle=\bfseries, title=Box1,halign title=right}
  - \newtcolorbox{box2}{colback=white, colframe=color_box2,fonttitle=\bfseries, title=Box2}
#  - \newtcolorbox{info-box}{colback=cyan!5!white,arc=0pt,outer arc=0pt,colframe=cyan!60!black}
#  - \newtcolorbox{warning-box}{colback=orange!5!white,arc=0pt,outer arc=0pt,colframe=orange!80!black}
#  - \newtcolorbox{error-box}{colback=red!5!white,arc=0pt,outer arc=0pt,colframe=red!75!black}
#  - \renewenvironment{Shaded}{\begin{error-box}}{\end{error-box}}

#  - \usepackage{xcolor}
#  - |
# ```\lstset {
#    basicstyle=\ttfamily,
#    numbers=left,
#    keywordstyle=\color[rgb]{0.13,0.29,0.53}\bfseries,
#    stringstyle=\color[rgb]{0.31,0.60,0.02},
#    commentstyle=\color[rgb]{0.56,0.35,0.01}\itshape,
#    numberstyle=\footnotesize,
#    stepnumber=1,
#    numbersep=5pt,
#    backgroundcolor=\color[RGB]{248,248,248},
#    showspaces=false,
#    showstringspaces=false,
#    showtabs=false,
#    tabsize=2,
#    captionpos=b,
#    breaklines=true,
#    breakatwhitespace=true,
#    breakautoindent=true,
#    escapeinside={\%*}{*)},
#    linewidth=\textwidth,
#    basewidth=0.5em,
#  }
#```

## frames
#  - \usepackage{framed}

## penalties
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)

  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text


---
