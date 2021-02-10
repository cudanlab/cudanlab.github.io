This is the working repository for the CUDAN HUGO website with the original markdown files. Changes will be rendered into the (public) GitHub Page repository cudanlab.github.io automatically.


# How-To 

**Installation and hugo documentation**  
https://gohugo.io/getting-started/installing/   

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

# Changing content  
To Do.  
**IMPORTANT!** Rendering and pushing your content overrides the whole public webpage! This means you always need to pull his repository first and make sure you are updating the latest version.    

# Rendering the static webpage  
The public folder in this repository has a git submodule pointing to the public cudanlab.github.io repository. You don't have to push the rendered webpage twice!  
**IMPORTANT!** Rendering and pushing your content overrides the whole public webpage! This means you always need to pull his repository first and make sure you are updating the latest version. 


# Best practise  
Always use your own GitHub account when you commit changes.   
**IMPORTANT!** Rendering and pushing your content overrides the whole public webpage! This means you always need to pull his repository first and make sure you are updating the latest version. 
