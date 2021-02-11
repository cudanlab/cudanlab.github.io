This is the main branch for the CUDAN website. You need to be a collaborator to edit and add files. Changes will automatically render the static webpage into the gh-pages branch. Do not touch the gh-pages!


# How-To 

# Installation and hugo documentation
https://gohugo.io/getting-started/installing/ 

**IMPORTANT!** Pushing your content overrides the whole public webpage! This means you always need to pull this repository first and make sure you are updating the latest version if you are using git from your local device. Never commit to the gh-pages branch directly! Use the main branch instead. You don't need to render the webpage locally – the static page will be rendered automatically with every commit (see GitHub Actions).   

# Adding new entries to the events page   
Every event is a file by its own inside the events folder. For consistency, filenames should start with the date followed by a clear title as in: 2021-02-08-deb-verhoeven-cudan-lecture.md 

Please use the example file *example-event.md* in the examples folder.   
**IMPORTANT!** The start and end date needs to have the date-format: 2021-02-08T10:00:00-00:00  

Put the abstract text and other additional information that should be hidden in the events page list after this tag:   
\<!--more-->

# General styling rules  
The markdown files are following the markdown syntax:
https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf  
**IMPORTANT!** Linebreaks need two white spaces!  


# Best practice  
Always use your own GitHub account when you commit. The safest method for editing existing content or adding new events is to stay in the GitHub browser and use only https://github.com/cudanlab/cudanlab.github.io/tree/main/content   
**IMPORTANT!** Rendering and pushing your content overrides the whole public webpage! This means you always need to pull this repository first and make sure you are updating the latest version if you are using git from your local device.
