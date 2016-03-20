---
layout: post
title:  Build blog post in Rstudio
date: 2016-03-10
published: true
tags: [R, blog, Rstudio, Rmarkdown]
---

## Requirement
* [R](https://www.r-project.org/) 
* [Rstudio](https://www.rstudio.com/)
* [Ruby](https://www.ruby-lang.org/en/documentation/installation/) for the installation of jekyll
* [RubyGem](https://rubygems.org/pages/download)
* [jekyll](https://jekyllrb.com/)
* Remote server that supports jekyll: [Amazon S3](https://aws.amazon.com/tw/s3/),[Github](https://github.com) 
* Local repository managed by version control system(e.g., git)

## Install Ruby and RubyGem
* For windows
 - [Rubyinstaller](http://rubyinstaller.org/)
 - Fresh user better use the least version
 - Choose the version based on your OS is 32bits or 64bits.
* For other OS
+ Follow the instructions on the [official website]((https://www.ruby-lang.org/en/documentation/installation/))
* Install RubyGem
+ Turn on `command line`
- Windows: input `cmd` in the dialogue `Run`
+ Input the commands on [official page](https://rubygems.org/pages/download)

## Install Jekyll
- Quick Way: Check [homepage of official site](https://jekyllrb.com/)
- Always run `jekyll serve` in `command line` when test personal blog/websit locally out of Rstudio.

## Initialize local repository
- Clone or download a [jekyll theme](http://jekyllthemes.org/) 
- Build folder `_source`; Gather .Rmd files for posters in this folder.
- install R packages as following(from [Brendan Rocks' blog](https://brendanrocks.com/blogging-with-rmarkdown-knitr-jekyll/)):  

        install.packages(c("knitr", "servr", "devtools"))     # To process .Rmd files  
        devtools::install_github("hadley/lubridate")         # brocks reqs dev version  
        devtools::install_github("brendan-r/brocks")         # My lazy wrapper funs
  
- 