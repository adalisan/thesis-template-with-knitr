# thesis-template-with-knitr
Thesis template with individual chapters as different Sweave/knitr 


I used **Sweave/knitr** to generate (majority of ) analyses and the figures in  my thesis. I used the style files in https://github.com/weitzner/jhu-thesis-template 


Each chapter is a separate *Rnw* file. The *Rnw* files include  R code chunks which are run with *knitr* ( http://yihui.name/knitr/ ), and the *tex* files are generated with the figures as outputs of the R chunks. For fast simulations/analyses this works nicely, as you don't need to remember which R script you used to generate a figure. For simulations that take a long amount of time, there is a cache option, so that the R code chunk is not run unless you made a change.
I would suggest using RStudio so that you can do version control, running simulations and building a pdf in one software tool.
A non-complete list of requirements:
=================
  *Latex (Miktex can install them automatically)
  These are some Latex packages that are required for building a pdf (available in MikTex distribution).
media9
\usepackage{cmbright} %clean look
\usepackage{cite}
\usepackage{amssymb,amsmath,amsthm,amscd}
\usepackage{pgfplots}
\usepackage{graphicx}
\usepackage{subcaption}
\usepackage{ mathrsfs, bm}
\usepackage[pdfa]{hyperref}
\usepackage{algorithm2e}
\usepackage{url}
\usepackage{ragged2e}
\usepackage{fixltx2e}
\usepackage{array}

\usepackage{wrapfig} 
\usepackage[T1]{fontenc}
\usepackage[latin1]{inputenc}
\usepackage{verbatim}
\usepackage{multirow}
\usepackage{fancyhdr}    % Use nice looking headers along with the required footer page numbers   

\usepackage{lscape} 
\usepackage[refpage]{nomencl}
\usepackage{makeidx}

%shorthand commands
\input{common.tex}


\usepackage{hyperxmp}
%\usepackage[T1]{fontenc}
%SA: This package is not necessary unless you want to create a slideshow-like  plot window like I did.
\usepackage{animate}


  *R

ggplot2 


