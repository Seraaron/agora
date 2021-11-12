**"A Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions."**
# Text
## Paragraph
Paragraphs are separated by a blank line.

This is another paragraph.

## Font Style
It's very easy to make some words *italic* and other words **bold**.

Any word wrapped with two tildes (like ~~this~~) will appear crossed out.

Words surrounded by two equals signs ==are highlighted== 

If you'd like to quote someone, use the `>` character before the line:

> This is a blockquote.
>
> This is the second paragraph.

### Extra Formatting
<sup>This is some superscript text</sup> and <sub>this is some subscript text.</sub>

this is left-aligned text (default)
<div style="text-align: center">this is center-aligned text (requires html)</div>
<div style="text-align: right">this is right-aligned text (requires html)</div>

But too much text-alignment and sub/super-scripts goes against the core philosophy of markdown files (stated at the top of this file), and snippets of html code aren't guaranteed to run in all markdown preview software. So use with caution.


## Links
You can link to anything, even [Wikipedia](https://en.wikipedia.org/wiki/Main_Page "and add a tooltip").

If you have many things to [link][1] to, or need to link to them [multiple][2] times, it's probably better to keep a [reference list][3]:

[1]: https://en.wikipedia.org/wiki/Hyperlink "you can"
[2]: https://en.wikipedia.org/wiki/Multiple_(mathematics) "also add"
[3]: https://en.wikipedia.org/wiki/Bibliographic_index "tooltips"

## Emojis
Some Markdown applications allow you to insert emoji by typing emoji shortcodes. These begin and end with a colon and include the name of an emoji. E.g.
>Gone camping! ⛺ `:tent:`
>Be back soon. 🙄 `:roll_eyes:`
>That is so funny! 😂 `:joy`

Or you can simply copy an emoji from a source like [Emojipedia](https://emojipedia.org/) and paste it into your document.

# Structure
## Headers
You can structure your texts in the following way:
```
# Title (H1)
## Subtitle (H2)
### Another deeper title (H3)
```
You can use H1 `#` all the way up to H6 `######` six for different title sizes.

### H3 Header

AAAaaa

#### H4 Sub-header

BBBbbb

##### H5 Sub-header

CCCccc

###### H6 subheader

DDDddd

## Lists
Bullet list:
* Start a line with an asterisk
* Food
  * Fruits
    * Oranges
    * Apples
 * indent
	 * indent 2

Numbered list:
1. One
2. Two
3. Three

Check list:
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

## Separator
A horizontal line looks like this:

---
This is text.

## Footnotes
There is no native way to do footnotes in markdown, because markdown sheets doesn't have a concept of page size<sup>1</sup>. But you can kind of fake it using superscript and subscripts and keeping footnotes relative<sup>2</sup> to the current section. You can also link<sup><a href="#note3" id="note3ref">3</a></sup> to a footnote anywhere in the sheet.

<sub>1. so there is no foot to note, per say.</sub>
<sub>2. this does mean you have to track them manually though.</sub>
<sub><a id="note3" href="#note3ref">3</a>. but this reduces readability of the raw markdown code</sub>

## Images
If you want to insert images, this is how you do it:

![The first Wikipedia logo](https://upload.wikimedia.org/wikipedia/commons/3/31/Wiki_logo_Nupedia.jpg)

To link to locally hosted images, put it in a folder in the same directory as the markdown file and type `![image name](./folder%20name/image%20name.png)`

# Tables
| Default aligned | Left aligned | Center aligned | Right aligned |
| --------------- | :----------- | :------------: | ------------: |
| First body part | Second cell  |   Third cell   |   fourth cell |
| Second line     | foo          |   **strong**   |           paz |
| Third line      | bar          |    *italic*    |           boo |

# Code
If you have inline code blocks, you can wrap them in backticks: `var example = true`.

If you've got a longer block of code, you can fence it with ```:

```
if (isNeat){
  return true
}
```
and specific syntax highlighting can be specified with the code language name after the graves (e.g. \`\`\`json`)
```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

## Formulas
You can use $\LaTeX$ to typeset formulas with `$`. A formula can be displayed inline, e.g. $e=mc^2$, or as a block with `$$`:
$$\int_\Omega \nabla u \cdot \nabla v~dx = \int_\Omega fv~dx$$

and even more complicated things like this:
$$
\begin{aligned}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{aligned}
$$
but again, this reduces readability.

Check out the [LaTeX introduction](https://en.wikibooks.org/wiki/LaTeX/Mathematics) for more.
<!--
Note that LaTeX code that uses the pipe symbol | in inline math statements may lead to a line being recognized as a table line. This problem can be avoided by using the \vert command instead of |!
-->

## Escaping
This \`a code segment with\` escaped graves

this is the list of all characters that can be escaped with a backslash `\`
- \\ backslash
- \. period
- \* asterisk
- \_ underscore
- \+ plus
- \- minus / hyphen
- \= equal sign
- \` back tick / grave
- \(\)\[\]\{\}\<\> left and right round / square / curly / angle brackets
- \# hash
- \! bang
- \<\< left guillemet
- \>\> right guillemet
- \: colon
- \| pipe
- \" double quote
- \' single quote
- \$ dollar sign

### Comments
`<!-- this is how you comment -->`
`%% or you can also comment like this %%`
<!-- comments aren't visible in the final document -->

<!-- 
%%# MIT License
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.%%
-->
