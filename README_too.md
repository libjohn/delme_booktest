# README 

The goal of reproducibility\_stats\_honors is to …

Enable a reproducible environment for your Stats honors thesis written
in [Bookdown](https://www.bookdown.org/)

## Bookdown

[Bookdown](https://bookdown.org/home/about/) is an open source R package that makes it easy to write books.  It works really well within the  RStudio project environment and is the preferred method within the Duke Stats department for producing and submitting honors theses. 

## Procedures

1. Update/install: R/RStudio.  
1. Update/install: tidyverse/tinytex/bookdown packages
1. Follow [steps 1 & 2 of the _Getting Started_ section](https://bookdown.org/home/about/)
1. Add Tier Protocol [organizational directories](https://www.projecttier.org/tier-protocol/specifications/#overview-of-the-documentation) 
1. Create Bookdown 
1. Add .gitignore ; .gitattributes, and license.txt
1. Make RStudio project a Git repository.  Then push to GitHub  (specific CLI git commands in terminal)
1. Develop your analysis; compose and orchestrate your HTML book (ignore PDF for now)


## Tips
1. In bookdown, each chapter is an Rmd file found in the project root.  (index.Rmd, 01, 02, ... 999999)
1. Files and directory names that begin with underscore _ will not be processed `render_book()`
1. Cannot have identical code-chunk names.
1. Cannot have identical identifiers for chapters and sections.  Can have custom identifiers {#foo-identifier}
1. **Merge and Knit** or _Knit and Merge_
1. Eventually you will `git push` your RStudio project into the Stats Department GitHub pages.  https://github.com/dukestatsci
1. .gitignore the _book directory until the end.  Consier, periodically unfreezing and `git push`

## license: “CC BY-NC”

[*Choose license(s)*](https://docs.google.com/presentation/d/1CcKWMUsH7ADCpLQZ57tfhiUIZYgKahmd_z45pVucVlw/edit#slide=id.g72011cc5c1_1_90)

Creative Commong: Attribution, Non-Commerical  
<https://creativecommons.org/licenses/by-nc/4.0/>
