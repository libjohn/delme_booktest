# README  
There are multiple methods for creating a bookdown.  This template enables a streamlined approach where the bookdown template has been overlayed into an RStudio Project which is also a Git repository.

## Bookdown  
[Bookdown](https://bookdown.org/home/about/) is an open source R package that makes it easy to write books.  It works really well within the  RStudio project environment and is the preferred method within the Duke Stats department for producing and submitting honors theses. 

## Procedures  
1. Update/install: R/RStudio.  This workshop assumes you have [Git](https://git-scm.com/) installed.  

    - Windows: install [Rtools](https://cran.r-project.org/bin/windows/Rtools/)  
    
2. Update/install tidyverse, bookdown, tinytex.  Then install TinyTex distribution

```
install.packages(c("tidyverse", "bookdown", "tinytex"))
tinytex::install_tinytex()   
```

3. Clone your customized GitHub repository (https://github.com/DukeStatSci)
3. Create a test Bookdown Book:  `Book Tab > Build Book`.  Your test book should build without errors
4. Develop your analysis; compose and orchestrate your HTML book.  Ignore PDF for now

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
- [*Choose license(s)*](https://docs.google.com/presentation/d/1CcKWMUsH7ADCpLQZ57tfhiUIZYgKahmd_z45pVucVlw/edit#slide=id.g72011cc5c1_1_90)
- A selective list of [uesthis enabled licenses](https://usethis.r-lib.org/reference/licenses.html) can be generated automatically

Creative Commons: Attribution, Non-Commerical  
<https://creativecommons.org/licenses/by-nc/4.0/>

## References  
- [bookdown: Authoring Books and Technical Documents with R Markdown](https://bookdown.org/yihui/bookdown/)
- [R Markdown Cookbook](https://bookdown.org/yihui/rmarkdown-cookbook/)
- [R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/)
- [Tier Protocol - suggested organizational structure](https://www.projecttier.org/tier-protocol/specifications/#overview-of-the-documentation)
- [UseThis](https://usethis.r-lib.org/)
- [Happy Git and GitHub for the useR](https://happygitwithr.com/)



