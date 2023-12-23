---
title: "A cool title"
subtitle: "This is the subtitle"
author: "Marcos Nicolau"
titlepage: True
toc: false
citeproc: true
numbersections: true
bibliography: "/home/marcos/.zotero/export.bib"
csl: "/home/marcos/Zotero/styles/the-lancet.csl"
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

\tableofcontents
\pagebreak

## A header

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec libero tellus, dapibus eu nulla ut, tristique rutrum tortor. Morbi eget pharetra dolor.

### Sub-header

ras ornare augue bibendum finibus cursus. Vivamus maximus felis sed mauris feugiat, nec blandit sem rhoncus. Aliquam non feugiat urna, id lacinia enim. Vestibulum eget convallis felis. Sed suscipit nulla eget quam interdum, nec tempus mauris ultrices. Aenean ac vestibulum elit. Sed pretium ex efficitur mi luctus lobortis.

##### Fundamental theorem of calculus

_Let f be a continuous real-valued function defined on a closed interval [a, b]. Let F be the function defined, for all x in [a, b], by_
$$F(x) = \int _a^x f(t)dt$$

_Then F is uniformly continuous on [a, b] and differentiable on the open interval (a, b), and_
$$F'(x) = f(x)$$
for all x in (a, b) so F is an antiderivative of f.

#### Sub-header 2

| Is HTML | a programming language?       |     |
| ------- | ----------------------------- | --- |
| 1       | No, it is a markup language ; |     |
| 2       | Yes ;)                        |     |

```
 <html>
   <head>
     <title>Test</title>
   </head>
```
