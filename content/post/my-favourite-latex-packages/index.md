---
aliases:
- /post/my-favourite-latex-packages
- /post/2018/6/my-favourite-latex-packages/
categories: []
date: "2018-06-25 22:13:30"
summary: ' '
tags:
- babel
- biblatex
- booktab
- capitalise
- character
- cleveref
- csquote
- english
- favourite
- font
- graphicspath
- graphicx
- hyperref
- hyphenation
- ieee
- inputenc
- midrule
- multicolumn
- packages
- phd
- placein
- refernces
- ""
- sisetup
- siunitx
- toprule
- unit
- usepackage
- utf8
title: My Favourite LaTeX Packages
---

```latex
% english hyphenation
\usepackage[english]{babel}

% for accented characters, load before csquotes
\usepackage[utf8]{inputenc}

% recommended with babel; \enquote{}
\usepackage{csquotes}

% for \graphicspath
\usepackage{graphicx}
\graphicspath{{./fig/}}

% \toprule, \midrule, \multicolumn
\usepackage{booktabs}

% unit formatting
\usepackage[per-mode=symbol]{siunitx}

% siunitx match IEEE font weight
\sisetup{detect-weight=true, detect-family=true}

% \FloatBarrier for stopping floats in REFERNCES section
\usepackage{placeins}

% linked references
\usepackage{hyperref}

% citations
% https://www.sharelatex.com/learn/Bibliography_management_in_LaTeX
\usepackage[
style=ieee,
doi=false,
isbn=false,
url=false,
]{biblatex}
\addbibresource{kuka-collaborative-poke.bib}

% easy referencing, must be loaded last!
\usepackage[capitalise]{cleveref}
```