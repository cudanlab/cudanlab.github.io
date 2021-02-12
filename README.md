This is the main branch for the CUDAN website. You need to be a collaborator to edit and add files. Changes will automatically render the static webpage into the gh-pages branch. Do not touch the gh-pages!

[![Hugo](https://img.shields.io/badge/hugo-0.68-blue.svg)](https://gohugo.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)


# Basic concept   
The CUDAN webpage is based on the following:  
Hugo: https://github.com/gohugoio/hugo  
Book theme: https://github.com/alex-shpak/hugo-book  
Makdown language: https://www.markdownguide.org/  
  
On top of the Hugo Book Theme, the CUDAN webpage uses customized CSS and html code in the layouts folder (e.g. shortcodes, injects and additional styling):   https://github.com/cudanlab/cudanlab.github.io/tree/main/layouts   

A GitHub Actions worklow file (.github/workflows/gh-pages.yml) renders the static pages automatically into the gh-pages branch, every time a commit is executed. Read more about GitHub Actions here: https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions   

  
# How-To 

## Installation and hugo documentation
https://gohugo.io/getting-started/installing/ 

**IMPORTANT!** Pushing your content overrides the whole public webpage! This means you always need to pull origin of the main branch first to make sure you are updating the latest version (if you are using git from your local machine). Never commit to the gh-pages branch directly! Use the main branch instead. You don't need to render the webpage locally – the static page will be rendered automatically with every commit (see GitHub Actions in .github/workflows/gh-pages.yml).   

## Adding new entries to the events page   
Every event is a file by its own inside the events folder. For consistency, filenames should start with the date followed by a clear title as in: 2021-02-08-deb-verhoeven-cudan-lecture.md 

Please use the example file *event-example.md* in the examples folder as reference: https://github.com/cudanlab/cudanlab.github.io/blob/main/examples/event-example.md     
**IMPORTANT!** In the header of a new event file, define a start and end date for the events parameter in the following format:  
```
---
events:
    start: 2021-02-08T14:00:00-00:00
    end: 2021-02-08T16:00:00-00:00
```
The event title follows the format:
```
title: "Speaker Name - Title of Talk"
---
```  
Don't use nested quotation marks inside the title (this will result in an error notification email and not update the webpage).

Put the abstract text and other additional information that should be hidden in the events page list after the "more" tag:   
```
<!--more-->
**Abstract** - Abstract text goes here.
```

## Best practice  
Always use your own GitHub account when committing changes. The safest method for editing existing content or adding new events is to stay in the GitHub browser and stay only in this directory: https://github.com/cudanlab/cudanlab.github.io/tree/edit/content   
If you want to use git from your local machine, always pull origin fromt he main branch before committing!  


## Basic Syntax

These are the elements outlined in John Gruber's original design document. All Markdown applications support these elements.

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Element</th>
      <th>Markdown Syntax</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="/basic-syntax/#headings">Heading</a></td>
      <td><code># H1<br>
          ## H2<br>
          ### H3</code></td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#bold">Bold</a></td>
      <td><code>**bold text**</code></td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#italic">Italic</a></td>
      <td><code>*italicized text*</code></td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#blockquotes-1">Blockquote</a></td>
      <td><code>> blockquote</code></td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#ordered-lists">Ordered List</a></td>
      <td><code>
        1. First item<br>
        2. Second item<br>
        3. Third item<br>
      </code></td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#unordered-lists">Unordered List</a></td>
      <td>
        <code>
          - First item<br>
          - Second item<br>
          - Third item<br>
        </code>
      </td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#code">Code</a></td>
      <td><code>`code`</code></td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#horizontal-rules">Horizontal Rule</a></td>
      <td><code>---</code></td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#links">Link</a></td>
      <td><code>[title](https://www.example.com)</code></td>
    </tr>
    <tr>
      <td><a href="/basic-syntax/#images-1">Image</a></td>
      <td><code>![alt text](image.jpg)</code></td>
    </tr>
  </tbody>
</table>

## Extended Syntax

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Element</th>
      <th>Markdown Syntax</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="/extended-syntax/#tables">Table</a></td>
      <td><code>
          | Syntax      | Description |<br>
          | ----------- | ----------- |<br>
          | Header      | Title       |<br>
          | Paragraph   | Text        |
      </code></td>
    </tr>
    <tr>
      <td><a href="/extended-syntax/#fenced-code-blocks">Fenced Code Block</a></td>
      <td><code>```<br>
      {<br>
      &nbsp;&nbsp;"firstName": "John",<br>
      &nbsp;&nbsp;"lastName": "Smith",<br>
      &nbsp;&nbsp;"age": 25<br>
      }<br>
      ```
      </code></td>
    </tr>
    <tr>
      <td><a href="/extended-syntax/#footnotes">Footnote</a></td>
      <td><code>
        Here's a sentence with a footnote. [^1]<br><br>

        [^1]: This is the footnote.
      </code></td>
    </tr>
    <tr>
      <td><a href="/extended-syntax/#heading-ids">Heading ID</a></td>
      <td><code>### My Great Heading {#custom-id}</code></td>
    </tr>
    <tr>
      <td><a href="/extended-syntax/#definition-lists">Definition List</a></td>
      <td><code>
        term<br>
        : definition
      </code></td>
    </tr>
    <tr>
      <td><a href="/extended-syntax/#strikethrough">Strikethrough</a></td>
      <td><code>~~The world is flat.~~</code></td>
    </tr>
    <tr>
      <td><a href="/extended-syntax/#task-lists">Task List</a></td>
      <td><code>
        - [x] Write the press release<br>
        - [ ] Update the website<br>
        - [ ] Contact the media
      </code></td>
    </tr>
  </tbody>
</table>

