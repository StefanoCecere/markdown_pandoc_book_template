# TEST Markdown

## Diagram

\setlength{\unitlength}{1mm}
\thicklines
\begin{picture}(10,6)
\put(2,2.2){\line(1,0){6}}
\put(2,2.2){\circle{2}}
\put(6,2.2){\oval(4,2)[r]}
\end{picture}

## tiz figure usepackage{tikz}

\begin{tikzpicture}

\draw (-2,0) -- (2,0);
\filldraw [gray] (0,0) circle (2pt);
\draw (-2,-2) .. controls (0,0) .. (2,-2);
\draw (-2,2) .. controls (-1,0) and (1,0) .. (2,2);

\end{tikzpicture}

---

\begin{tikzpicture}
\filldraw[color=red!60, fill=red!5, very thick](-1,0) circle (1.5);
\fill[blue!50] (2.5,0) ellipse (1.5 and 0.5);
\draw[ultra thick, ->] (6.5,0) arc (0:220:1);
\end{tikzpicture}

## Emojis
🤣 :heart_eyes:

[❤️](#gdt_carcassonnejr)

[🤣](https://stefanocecere.com) 

\Psi \Omega 

usepackage{wasysym}: \smiley{} \frownie{} \blacksmiley{}



## Boxes

> questo è un block quote generico
> This is a blockquote e qui funzionano **i strong**

\begin{box1}
Hi, i am box 1
\end{box1}

\begin{box2}
and i am box 2
\end{box2}

| let's test this
| text with starting pipes

```
text in blockquotes
```

::: box
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam aliquet libero
quis lectus elementum fermentum.
:::

::: error
**Error**: This is a custom box that may be used to show error messages in your
document.
:::

## Multi column

\Begin{multicols}{2}

1. Item 1
2. Item 2
3. Item 3
4. Item 4
5. Item 5

\End{multicols}



## Text Color

\textcolor{red}{red}, violets are \textcolor{blue}{blue}.


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

Highlights ==this part of text.==

## Links

### External links
[www.google.com](https://www.google.com)  
[www.google.com with title](https://www.google.com "Google's Homepage")  

URLs and URLs in angle brackets will automatically get turned into links.
http://www.example.com or <http://www.example.com> and sometimes
example.com (but not on Github, for example).

### Internal links
This links to the [Introduction](#introduction)  
This links to [The End](#the-end)  
This links to [Chapter 2.2 via manual Anchor](#chap22_anchor)  

## Definitions

Parola da definire
: è una cosa che si fa e non si dice

## css

questo è un box
{:.box}


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

## Maths

$$
y = -2.2x + 0.5
$$

$a+b= \frac{c}{c}$
$$a+b= \frac{c}{c}$$

$\lim{n \to \infty} x^{n+9}$
$$\lim{n \to \infty} x^{n+9}$$

$$\begin{aligned}
  a+b &= c           \
  b &= c - a         \
  1 &= \frac{b}{c-a} \
\end{aligned}$$

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