---
title: ""
subtitle: ""
author: ""
abstract: ""
titlepage: True
toc: false
citeproc: true
numbersections: true
bibliography: "PATH_TO_.BIB_FILE"
csl: "LINK_TO_CITATION_STYLE"
variable: 
  - papersize=a4paper
  - classoption=twocolumn % two column layout
header-includes: |
	\usepackage{preamble} 
    \usepackage{fancyhdr}
    \pagestyle{fancy}
    \fancyhf[]{}
    \fancyhead[R]{\date{\today}}
    \fancyhead[L]{\nouppercase{\rightmark}}
    \fancyfoot[R]{\thepage}
    \fancyfoot[L]{Author}
    \usepackage[a4paper, portrait, margin=1in]{geometry}
    \fontsize{12pt}{12pt}\selectfont
    \usepackage{setspace}
    \doublespacing
    \newlength\FHoffset
	\setlength\FHoffset{1cm}
	\fancyheadoffset{\FHoffset}
	\usepackage{amsmath}
---
%% Also remember that if you want to export with pandoc then you must forfeit features like wikilinks, DataView tables, admonitions and Templater. Though you can find some workarounds through plugins, lua scripts, etc.%%

%% Inserts the table of contents in pandoc with a line break %%
\tableofcontents
\pagebreak