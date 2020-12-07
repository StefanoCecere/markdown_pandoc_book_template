# Markdown -> Pandoc -> Book creation

this template is to create a book in PDF/ePub/html/Docx format from a group of markdown files.

i needed this because i wanted to use Pandoc to have total configuration freedom
and editors book exporters (Ulysses, Scrivener, Zettlr, iA Writer, Marked 2...) were limited, and my preferred one [Obsidian.md](https://obsidian.md/) doesn't export... yet

## Syntax
```
pandoc -d config_pdf.yaml manuscript/*.md
pandoc -d config_epub.yaml manuscript/*.md
pandoc -d config_docx.yaml manuscript/*.md
pandoc -d config_html.yaml manuscript/*.md
```

## Requirements

- Pandoc: see [Installing Pandoc](https://pandoc.org/installing.html).
- Install a LaTeX distribuition.
under mac i could work with the smaller [BasicTeX](https://www.tug.org/mactex/morepackages.html)

i installed both with:
```
brew install pandoc
brew install homebrew/cask/basictex
```

Update: i've moved to the much bigger but really complete [MacTeX-2020 Distribution](https://www.tug.org/mactex/)

## How To

the book is in the `manuscript/` directory as a group of markdown files.
indeed we call Pandoc with `manuscript/*.md` which feeds all the .md files, that's why we prefix the files with the numered order

most of the book metadata are in the `000_metadata.md` file, check there all the options.

the generated files are in the `output/` directory.

## Thanks
- <https://brainbaking.com/post/2020/05/using-pandoc/>
- <https://blog.semanticart.com/2014/01/11/writing-hypertext-fiction-in-markdown/>
- <https://github.com/maehr/academic-pandoc-template>
- <https://github.com/adunning/pandoc-ebook>
- <https://github.com/johnpaulada/pandoc-markdown-book-template>
- <https://github.com/Carleslc/Readteractive>
- <http://mcdemarco.net/tools/scree/>

## License
This project is loved by Stefano Cecere and .md friends and licensed under the MIT License see [LICENSE.md](LICENSE.md)
