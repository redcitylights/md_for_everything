---
auto-scaling: fittingHeader,math,code,true
marp: false
---

# Markdown for *\*everything\**

---

# `.md`
<!-- open live demo--->
What is Markdown? A simple markup language that's used to format text, as you might do in MS Word, but just using a plain-text editor.
### Editors
- VSCode
- Notepad
- Vim
- Obsidian

---

## Uses
- Writing
- Note Taking
- Presentations
- Blogging
- Documentation
- Jupyter/R Notebooks
- Discord, Reddit, Some EMail clients

---

## Syntax
Simple to write and read. WYSIWYG
```markdown
*italics*
**bold**
~~strikethrough~~

# Heading 1
## Heading 2
### Heading 3

* Unordered list
* Unordered list

1. Ordered list
1. Ordered list
Horizontal line
---

[Link text](link_me.html)
![Embedded link text](embed_me.html)

> Block Quotes

inline `code` rendering

escape characters that should be rendered \*
```

---

## Note taking
<!--compare to OneNote--->
#### Why:
* The hierarchy of headers can help order ideas in your mind 
<!--to be continued--->
* Notes are easily searchable
* Not restricted by a proprietary file format
	- Notes easier to share
	- Save money
#### How:
* Just save a text file with the `.md` extension
<!--it's really simple--->
<!--open Obsidian demo--->
<!--of course, these are self-imposed rules--->

---

## Presentations
#### Why:
* Lightweight
* Simple formatting helps you focus on content
* Embedded code rendering works better than PowerPoint

#### How:
<!--show presentation code in VSCode--->
* [Marp](https://marp.app/)
	- CLI/Extension generates PDF, PPTX, or HTML
	- `marp -p slideshow.md`
* [RevealJs](https://revealjs.com/markdown/)
	- Boilerplate HTML file you paste your markdown into. More powerful, more complicated

---

## Advanced
- MD to HTML
- Static sites
- Github Flavored Markdown
- Jupyter Notebooks
- Obsidian Shilling
<!--is it shillling if I don't make any money from it?--->

---

### MD to HTML
Everyone has a web browser, so this makes sharing MD files easy
- Pandoc
```bash
pandoc -s filename.md -o filename.html
```
- Online
[Markdown To HTML](https://markdowntohtml.com/)

---

### Static Site Generation
Static site generators take simple content (like MD) and generate plain HTML based on some template, similar to how MARP works.

#### Why:
* Static sites are cheap to host
	- GitHub Pages
* More secure than wordpress
* Content/style seperation
	- Changing themes is *very* easy
* Shortcodes

---

#### How:
- Hugo
- Jekyll
- Obsidian Publish (technically not SSG)
Hugo is better  
[example site](https://letsencrypt.org/)

---

### GitHub Flavored Markdown
(GFM) is used for GitHub README.md files. [example](https://github.com/Leaflet/Leaflet)
- Fenced code blocks
```java
int mult(int a, int b){
	return a * b;
}
```
- Tables

Header 1 | Header 2
---------|---------
cell 1   | pipes must be escaped \|

---

### GFM...
#### TODO lists

- [ ] Get milk
- [x] Get eggs

---

### Obsidian ![](https://obsidian.md/favicon.ico)
Free markdown editor that adds features to markdown.  
I'll just cover a few of those features.

---
#### Obsidian...
- Linking
Syntax:  
```markdown
[[note]]
```

<!--show graph--->
<!--link to unmade notes--->

- Inline $\KaTeX$
- Callouts
> [!TODO] Callout Title
> *Callout* body text. The quick brown fox...

---

#### Obsidian...

- Plugins
	- Diagrams
	- Discord Rich Presence
	- Editor Syntax Highlight
	- Hider
	- Mind Map
	- Note Refactor
	- Vimrc Support
- Mind map
	- Remember I mentioned a 'hierarchy of headers'? We can visualize a markdown document as a mind map.

---

### Notebooks
Jupyter and R notebooks combine MD and code
<!--show header collapsing and code fencing--->⏎ 
