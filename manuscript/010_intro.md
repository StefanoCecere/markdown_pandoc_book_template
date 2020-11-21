---
tags: [published]
---
# Introduction

Welcome to this template to generate a book via Markdown and Pandoc.


# Write Markdown

Here are some samples for Markdown formatting and chapters.

## Headings 2

Text under Heading 2

### Heading 3

Text under Heading 3

#### Heading 4

Text under Heading 4

##### Heading 5

Text under Heading 5

## Emphasis

Emphasis, aka italics, with *asterisks* or _underscores_.  
Strong emphasis, aka bold, with **asterisks** or __underscores__.  
Combined emphasis with **asterisks and _underscores_**.  
Strikethrough uses two tildes. ~~Scratch this.~~  

## Lists

1. First ordered list item
2. Another item
3. Another item
4. Another item
   - Unordered sub-list.
   - Unordered sub-list.
   - Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
   1. Ordered sub-list
   1. Ordered sub-list
   1. Ordered sub-list
4. the last item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

To have a line break without a paragraph, you will need to use two trailing spaces.  
Note that this line is separate, but within the same paragraph.  
(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

## Links

[I'm an inline-style link](https://www.google.com)  

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a relative reference to a repository file](../blob/master/LICENSE.md)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links.
http://www.example.com or <http://www.example.com> and sometimes
example.com (but not on Github, for example).

## Images

Save your image (jpg or png format only) to `img/` and insert it like this:

![Figure 1 caption text](img/image.jpg "Image Title Text 1")

we can have many images.. here is another one:

![Figure 2 caption text](img/image.jpg "Image Title Text 2")

## Tables

We can have nice tables.  
Colons can be used to align columns.  

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

Table: Table captions are done like this.

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

## Blockquotes

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote.


## Footnotes

Footnotes are best placed right after the paragraph first used.[^footnote]

[^footnote]: But you can also put them at the end of the document.

If you want to use endnotes instead turn them on in document options.


## Comments

We can have comments in the text

<!-- Comments are not shown in the final PDF -->

```markdown
here we can write code.  
or **strong** test
```
