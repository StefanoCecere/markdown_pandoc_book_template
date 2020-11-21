# Markdown -> Pandoc -> Book creation

this template is to create a book in PDF/ePub/html/Docx format from a group of markdown files.

i needed this because i wanted to use Pandoc to have total configuration freedom
and editors book exporters (Ulysses, Scrivener, Zettlr, iA Writer, Marked 2...) were limited

## syntax
```
pandoc -d config_pdf.yaml manuscript/*.md
pandoc -d config_epub.yaml manuscript/*.md
pandoc -d config_docx.yaml manuscript/*.md
```

## thanks
<https://brainbaking.com/post/2020/05/using-pandoc/>
<https://blog.semanticart.com/2014/01/11/writing-hypertext-fiction-in-markdown/>
<https://github.com/maehr/academic-pandoc-template>
<https://github.com/adunning/pandoc-ebook>
<https://github.com/johnpaulada/pandoc-markdown-book-template>
<https://github.com/Carleslc/Readteractive>
<http://mcdemarco.net/tools/scree/>
