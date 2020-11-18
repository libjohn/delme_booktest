# README  
The goal of reproducibility\_stats\_honors is to …

Enable a reproducible environment for your Statistics honors thesis written
in [Bookdown](https://www.bookdown.org/)

## Bookdown  
[Bookdown](https://bookdown.org/home/about/) is an open source R package that makes it easy to write books.  It works really well within the  RStudio project environment and is the preferred method within the Duke Stats department for producing and submitting honors theses. 

## Procedures  
1. Update/install: R/RStudio

    - Windows: install [Rtools](https://cran.r-project.org/bin/windows/Rtools/)  
    
1. Update/install tidyverse, bookdown, tinytex packcages.  Then install TinyTex distribution

```
install.packages(c("tidyverse", "bookdown", "tinytex"))
tinytex::install_tinytex()   # not sure if Mac needs to do this.
```

3. Follow [step 2 of the _Getting Started_ section](https://bookdown.org/home/about/)
1. Add Tier Protocol [organizational directories](https://www.projecttier.org/tier-protocol/specifications/#overview-of-the-documentation): `_data_original`, `_data_analysis`, `_scripts_development` 
1. Create Bookdown Book (Book Tab > Build Book) 
1. Add .gitignore ; .gitattributes, and license.txt
1. Make RStudio project a Git repository.  Then push to GitHub  (Using specific CLI git commands from GitHub, push existing directory from within RStudio terminal)
1. Develop your analysis; compose and orchestrate your HTML book (ignore PDF for now)
1. Continue development with `git commit` and `git push` into your GitHub repository
1. At the end of your project, you may need to change the `git remote` so you can `git push` your RStudio project into the [Statistics Department GitHub pages](https://github.com/dukestatsci)


## Tips  
1. In bookdown, each chapter is an Rmd file found in the project root.  (index.Rmd, 01, 02, ... 999999)
1. Files and directory names that begin with underscore _ will not be processed by `bookdown::render_book()`
1. Cannot have identical code-chunk names
1. Code chunks that produce visualizations should have a code chunk _name_
1. Synchronize the file_name for each chapter with H1 in in line 1
1. Cannot have identical identifiers for chapters and sections.  Can have custom identifiers {#foo-identifier}
1. [**Merge and Knit** or _Knit and Merge_](https://bookdown.org/yihui/bookdown/new-session.html)
1. .gitignore the _book directory until the end.  Consider, periodically unfreezing and `git push`

## license: “CC BY-NC”  
[*Choose license(s)*](https://docs.google.com/presentation/d/1CcKWMUsH7ADCpLQZ57tfhiUIZYgKahmd_z45pVucVlw/edit#slide=id.g72011cc5c1_1_90)

Creative Commong: Attribution, Non-Commerical  
<https://creativecommons.org/licenses/by-nc/4.0/>

## References  
- [Getting started with Bookdown](https://bookdown.org/home/about/)
- [bookdown: Authoring Books and Technical Documents with R Markdown](https://bookdown.org/yihui/bookdown/)
- [R Markdown Cookbook](https://bookdown.org/yihui/rmarkdown-cookbook/)
- [R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/)
- [Tier Protocol - suggested organizational structure](https://www.projecttier.org/tier-protocol/specifications/#overview-of-the-documentation)



