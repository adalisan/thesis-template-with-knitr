# thesis-template-with-knitr
Thesis template with individual chapters as different Sweave/knitr 


I used **Sweave/knitr** to generate (majority of ) analyses and the figures in  my thesis. I used the style files in https://github.com/weitzner/jhu-thesis-template 


Each chapter is a separate *Rnw* file. The *Rnw* files include  R code chunks which are run with *knitr* ( http://yihui.name/knitr/ ), and the *tex* files are generated with the figures as outputs of the R chunks. For fast simulations/analyses this works nicely, as you don't need to remember which R script you used to generate a figure. For simulations that take a long amount of time, there is a cache option, so that the R code chunk is not run unless you made a change.
I would suggest using RStudio so that you can do version control, running simulations and building a pdf in one software tool.

There are some Latex packages that are required for building a pdf (available in MikTex distribution).
