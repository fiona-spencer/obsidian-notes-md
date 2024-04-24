
## Paragraphs
This is a paragraph

## Headings
'#' This is heading 1
'##' This is heading 2
'###' This is heading 3
'####' This is heading 4
'#####' This is heading 5
'######' This is heading 6

## Bold, Italics, Highlights
Regular Text
__Bold Text__
_Italic Text_
~~Strikeout Text~~
==Highlighted text==
**Bold text and _nested italic_ text**
***Bold and Italic Text***

\*Formatting can be forced to display in plain text by adding a backslash in front

## Internal Links
Wikilink: [[]]
Markdown: []

## External Links
[Link Text] (URL)
[Google] (https://www.google.com)

### Escape Blank Spaced in Links
If URL contains black spaces, replace with %20 or wrapping with angle brackets (<>)
[My Note](obsidian://open?vault=MainVault&file=My%20Note.md)
[My Note](<obsidian://open?vault=MainVault&file=My Note.md>)

## External Images
Add a ! symbol before an external link
Change image dimensions, by adding | width x height
![Image | 200 x 200](https://png.pngtree.com/png-vector/20191121/ourmid/pngtree-blue-bird-vector-or-color-illustration-png-image_2013004.jpg)

## Quotes
Quote text by adding a > symbol before the text
> Human beings face ever more complex and urgent problems, and their effectiveness in dealing with these problems is a matter that is critical to the stability and continued progress of society. 

\- Doug Engelbart, 1961

## Lists
Create an unordered list by adding -, \*, or + before the text
- First list item
- Second list item
- Third list item
Create an ordered list by starting each line with a number followed by .
1. First list item
2. Second list item
3. Third list item

## Task Lists
To create a task list, start each list item with a hyphen a space followed by [ ]
- [x] This is a completed task
- [ ] This is a incomplete task

### Nested Lists
All list types can be nested by indenting one or more list items
Tab or Shift+Tab to indent or unindent
1. First list item
	1. Ordered nested list item
2. Second list items
	- Unordered nested list item

## Horizontal Rule
Three or more starts, hyphens, or underscores to create a horizontal line

## Code
Format code both inline within a sentence, or in its own block

### Inline Code
Text inside `backticks` on a line will be formatted like code

### Code Blocks
```
cd ~/Desktop
```

```js
function fancyAlert(arg){
	if(arg){
	$.facebox({div: '#foo'})}
}
```

## Link to File
[mern-blog file](<file:///Users/mac/Desktop/Projects%202024/CURRENT/mern-blog>)

```zsh
cd Desktop/
```