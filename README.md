This is the main branch for the CUDAN website. You need to be a collaborator to edit and add files. Changes will automatically render the static webpage into the gh-pages branch. Do not touch the gh-pages!

[![Hugo](https://img.shields.io/badge/hugo-0.68-blue.svg)](https://gohugo.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)


# Concept and structure  
The CUDAN webpage is based on the following:  
Hugo: https://github.com/gohugoio/hugo  
Book theme: https://github.com/alex-shpak/hugo-book  
Makdown language: https://www.markdownguide.org/  
  
On top of the Hugo Book Theme, the CUDAN webpage uses customized CSS and html code in the layouts folder (e.g. shortcodes, injects and additional styling):   https://github.com/cudanlab/cudanlab.github.io/tree/main/layouts   

A GitHub Actions worklow file (.github/workflows/gh-pages.yml) renders the static pages automatically into the gh-pages branch, every time a commit is executed. Read more about GitHub Actions here: https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions   

  
# How-To 

# Installation and hugo documentation
https://gohugo.io/getting-started/installing/ 

**IMPORTANT!** Pushing your content overrides the whole public webpage! This means you always need to pull origin of the main branch first to make sure you are updating the latest version (if you are using git from your local machine). Never commit to the gh-pages branch directly! Use the main branch instead. You don't need to render the webpage locally – the static page will be rendered automatically with every commit (see GitHub Actions in .github/workflows/gh-pages.yml).   

# Adding new entries to the events page   
Every event is a file by its own inside the events folder. For consistency, filenames should start with the date followed by a clear title as in: 2021-02-08-deb-verhoeven-cudan-lecture.md 

Please use the example file *example-event.md* in the examples folder as reference: https://github.com/cudanlab/cudanlab.github.io/blob/main/examples/event-example.md     
**IMPORTANT!** The start and end date needs to have the date-format: 2021-02-08T10:00:00-00:00  
The event title cannot contain quotation marks. Any mistake will result in a notification email. 

Put the abstract text and other additional information that should be hidden in the events page list after this tag:   
\<!--more-->

# General styling rules  
The markdown files are following the markdown syntax:
https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf  
**IMPORTANT!** Linebreaks need two white spaces!  

# Best practice  
Always use your own GitHub account when committing changes. The safest method for editing existing content or adding new events is to stay in the GitHub browser and stay only in this directory: https://github.com/cudanlab/cudanlab.github.io/tree/edit/content   
If you want to use git from your local machine, always pull origin fromt he main branch before committing!
