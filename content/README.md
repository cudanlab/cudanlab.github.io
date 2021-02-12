# How-To edit and add content

## Adding new entries to the events page   
Every event is a file by its own inside the events folder. For consistency, filenames should start with the date followed by a clear title as in:  
```
2021-02-08-deb-verhoeven-cudan-lecture.md 
```
  
Use this example for new entries:
```
---
bookHidden: true

title: "Lecturer Name – Title of lecture without additional quotation marks"
event:
  start: 2021-02-08T14:00:00-00:00
  end: 2021-02-08T16:00:00-00:00
---

**When:** 2021-02-08 10:00-12:00 (Tallinn time)  
**Where:** CUDAN Open Lab (online)  

The event is public via zoom: https://zoom.us/j/94858442274X  
Websites: https://debverhoeven.com/ & https://kinomatics.com/ 

<!--more-->
**Abstract** – Abstract text goes here. Delete (inculding <!--more--> tag) if there is no addition text.
```


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
