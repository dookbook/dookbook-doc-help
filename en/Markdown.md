TOPICS: markdown

# Markdown

**Markdown** is a simple markup language that allows one to write documents
using a text editor and transform those documents into many different formats,
such as *HTML*, *Word*, images, *PDF*, *epub*, etc.
Among other things, it works beautifully for documenting source code since the
Markdown documents can be checked in and versioned with *Git* or your source
control system of choice.

Markdown language is created by *John Gruber* in 2004.

!!! info "Tips"
    The *suffix* of the documents written by Markdown are `.md` or `.markdown`.

## Heading

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

**Markdown** Input:

```markdown
# Level-1 Heading

## Level-2 Heading

### Level-3 Heading
```

**HTML** Output:

```html
<h1>Level-1 Heading</h1>

<h2>Level-2 Heading</h2>

<h3>Level-3 Heading</h3>
```

## Paragraph

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

**Markdown** Input:

```markdown
Paragraph 1

Paragraph 2
```

**HTML** Output:

```html
<p>Paragraph 1</p>
<p>Paragraph 2</p>
```

## List

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

### Unordered List

Demo:

- Item 1
    - Item 1.1
    - Item 1.2
- Item 2

**Markdown** Input:

```markdown
- Item 1
    - Item 1.1
    - Item 1.2
- Item 2
```

**HTML** Output:

```html
<ul>
  <li>Item 1</li>
  <ul>
    <li>Item 1.1</li>
    <li>Item 1.2</li>
  </ul>
  <li>Item 2</li>
</ul>
```

### Ordered List

Demo:

1. Item 1
2. Item 2

**Markdown** Input:

```markdown
1. Item 1
2. Item 2
```

**HTML** Output:

```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```

### Definition List

Demo:

Apple
:   Pomaceous fruit of plants of the genus Malus in
    the family Rosaceae.

Orange
:   The fruit of an evergreen tree of the genus Citrus.

**Markdown** Input:

```markdown
Apple
:   Pomaceous fruit of plants of the genus Malus in
    the family Rosaceae.

Orange
:   The fruit of an evergreen tree of the genus Citrus.
```

**HTML** Output:

```html
<dl>
  <dt>Apple</dt>
  <dd>Pomaceous fruit of plants of the genus Malus in the family Rosaceae.</dd>

  <dt>Orange</dt>
  <dd>The fruit of an evergreen tree of the genus Citrus.</dd>
</dl>
```

## Text

### Bold Text

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

Demo:

This text will be **bold**

This will also be __bold__

**Markdown** Input:

```markdown
This text will be **bold**

This will also be __bold__
```

**HTML** Output:

```html
This text will be <strong>bold</strong>

This will also be <strong>bold</strong>
```

### Italic Text

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

Demo:

<!-- markdownlint-disable MD036 -->
*This text will be italic*

_This will also be italic_
<!-- markdownlint-enable MD036 -->

**Markdown** Input:

```markdown
*This text will be italic*

_This will also be italic_
```

**HTML** Output:

```html
<em>This text will be italic</em>

<em>This will also be italic</em>
```

### Deleted Text

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

Demo:

~~Deleted Text~~

**Markdown** Input:

```markdown
~~Deleted Text~~
```

**HTML** Output:

```html
<del>Deleted Text</del>
```

### Inserted Text

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

++Inserted Text++

**Markdown** Input:

```markdown
++Inserted Text++
```

**HTML** Output:

```html
<ins>Inserted Text</ins>
```

### Combined Emphasis Text

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

Combined emphasis with **asterisks and _underscores_**.

**Markdown** Input:

```markdown
Combined emphasis with **asterisks and _underscores_**.
```

**HTML** Output:

```html
Combined emphasis with <strong>asterisks and <em>underscores</em></strong>.
```

## Horizontal Rule

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

**Markdown** Input:

```markdown
***
```

**HTML** Output:

```html
<hr/>
```

## Link

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

Demo:

A [link](https://dookbook.info/) here.

A [link](https://dookbook.info/ "Dookbook Homepage") here.

**Markdown** Input:

```markdown
A [link](https://dookbook.info/) here.

A [link](https://dookbook.info/ "Dookbook Homepage") here.
```

**HTML** Output:

```html
A <a href="https://dookbook.info/">link</a> here.

A <a href="https://dookbook.info/" title="Dookbook Homepage">link</a> here.
```

## Image

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

**Markdown** Input:

```markdown
![Alt Text](URL)
```

**HTML** Output:

```html
<img src="URL" alt="Alt Text"/>
```

## Inline Code

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

Demo:

<!-- markdownlint-disable MD031 -->
```markdown
```markdown
`code here`
``` // end
```
<!-- markdownlint-enable MD031 -->

**Markdown** Input:

```markdown
`code here`
```

**HTML** Output:

```html
<code>code here</code>

<value>code here</value>
```

## Table

### Raw Table

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

Demo:

| Name | Description | Hot |
| ------------- | --- | --- |
| Help | Display the help window.| 5 |
| **Close** | *Closes* a `window` | 1000 |

**Markdown** Input:

```markdown
| Name | Description | Hot |
| ------------- | --- | --- |
| Help | Display the help window.| 5 |
| **Close** | *Closes* a `window` | 1000 |

<!-- 1. There must be at least 3 dashes separating each header cell. -->

<!-- 2. The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown. -->
```

**HTML** Output:

```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
      <th>Hot</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Help</td>
      <td>Display the help window.</td>
      <td>5</td>
    </tr>
    <tr>
      <td><strong>Close</strong>/td>
      <td><em>Closes</em> a <code>window</code></td>
      <td>1000</td>
    </tr>
  </tbody>
</table>
```

### Column Alignment

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

| Name | Description (centered) | Hot (right-aligned) |
| ------------- | :---: | ---: |
| Help | Display the help window.| 5 |
| **Close** | *Closes* a `window` | 1000 |

**Markdown** Input:

```markdown
<!-- Colons can be used to align columns: right-aligned, centered, and neat -->

| Name | Description (centered) | Hot (right-aligned) |
| ------------- | :---: | ---: |
| Help | Display the help window.| 5 |
| **Close** | *Closes* a `window` | 1000 |
```

**HTML** Output:

```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th align="center">Description (centered)</th>
      <th align="right">Hot (right-aligned)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Help</td>
      <td align="center">Display the help window.</td>
      <td align="right">5</td>
    </tr>
    <tr>
      <td>Close</td>
      <td align="center"><em>Closes</em> a <code>window</code></td>
      <td align="right">1000</td>
    </tr>
  </tbody>
</table>
```

## Blockquote

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

Demo:

As Kanye West said:

> We're living the future so
> the present is our past.

**Markdown** Input:

```markdown
As Kanye West said:

> We're living the future so
> the present is our past.
```

**HTML** Output:

```html
<p>As Kanye West said:</p>

<blockquote>We're living the future so
  the present is our past.</blockquote>
```

## Abbreviations

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

The HTML specification
is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium

**Markdown** Input:

```markdown
The HTML specification
is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium
```

**HTML** Output:

```html
<p>The <abbr title="Hyper Text Markup Language">HTML</abbr> specification
is maintained by the <abbr title="World Wide Web Consortium">W3C</abbr>.</p>
```

## Code Block

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

```python
print ('Hello world')
``` // end

**Markdown** Input:

<!-- markdownlint-disable MD031 -->
```markdown
```python
print ('Hello world')
``` // end
```
<!-- markdownlint-enable MD031 -->

**HTML** Output:

```html
<pre><code>
print ('Hello world')
</code></pre>
```

!!! warn "Dookbook Markdown"
    *Dookbook Markdown* supports for code syntax highlight for 9
    languages: `HTML`/`XML`, `CSS`, `JavaScript`, `Python`, `Markdown`,
    `Bash`, `INI`/`TOML`.

### HTML

```html
<!DOCTYPE html>
<html>
<head>
  <title>Title</title>
  <style>body {width: 500px;}</style>
</head>
<body>
  <p checked class="title" id='title'>Title</p>
  <!-- here goes the rest of the page -->

  <script>
    function $init() {return true;}
  </script>
</body>
</html>
```

### XML

```xml
<xml>
  <tag1 attr="value">tag-1 text</tag>
</xml>
```

### CSS

```css
@font-face {
  font-family: Chunkfive; src: url('Chunkfive.otf');
}

body, .usertext {
  color: #F0F0F0; background: #600;
  font-family: Chunkfive, sans;
}

@import url(print.css);
@media print {
  a[href^=http]::after {
    content: attr(href)
  }
}
```

### JavaScript

!!! warn "Dookbook Markdown"
    *Dookbook Markdown* supports for **ES6+**.

```javascript
function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1)
      return process(block, true, 0x0F) +
             ` class="${cls}"`;
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i < classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      console.log('undefined');
  }
}

export  $initHighlight;
```

### Python

```python
import sys

print('hello')
sys.exit()

@requires_authorization
def somefunc(param1='', param2=0):
    r'''A docstring'''
    if param1 > param2: # interesting
        print 'Gre\'ater'
    return (param2 - param1 + 1 + 0b10l) or None

class SomeClass:
    pass

>>> message = '''interpreter
... prompt'''
```

### Markdown <!-- markdownlint-disable MD024 -->

```markdown
## Heading 2

### Heading 3

A paragraph with a **strong** text and *italic* text.
```

### Bash

```bash
#!/bin/bash

###### CONFIG
ACCEPTED_HOSTS="/root/.hag_accepted.conf"
BE_VERBOSE=false

if [ "$UID" -ne 0 ]
then
 echo "Superuser rights required"
 exit 2
fi

genApacheConf(){
 echo -e "# Host ${HOME_DIR}$1/$2 :"
}
```

### INI/TOML

```toml
; boilerplate
[package]
name = "some_name"
authors = ["Author"]
description = "This is \
a description"

[[lib]]
name = ${NAME}
default = True
auto = no
counter = 1_000
```

## Attribute List

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

**Markdown** Input:

```markdown
## Attribute List {: #head-id}

Windows lets you perform most tasks directly from the keyboard. This page lists out the default bindings (keyboard shortcuts). Windows lets you perform most tasks directly from the keyboard. This page lists out the **default**{: attrname="value" } bindings (keyboard shortcuts).
{: #someid .someclass attrname='value' }
```

**HTML** Output:

```html
<h2 id="head-id">Attribute List</h2>
<p attrname="value" class="someclass" id="someid">Windows lets you perform most tasks directly from the keyboard. This page lists out the default bindings (keyboard shortcuts). Windows lets you perform most tasks directly from the keyboard. This page lists out the <strong attrname="value">default</strong> bindings (keyboard shortcuts).</p>
```

## Footnote

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

Footnotes have a label[^label1] and the footnote's content[^label2].

[^label1]: A footnote on the label: "label1".
[^label2]: A footnote on the label: "label2".

///Footnotes Go Here///

**Markdown** Input:

```markdown
Footnotes have a label[^label1] and the footnote's content[^label2].

[^label1]: A footnote on the label: "label1".
[^label2]: A footnote on the label: "label2".

///Footnotes Go Here///
```

**HTML** Output:

```html
<p>Footnotes have a label<sup id="fnref:label1"><a class="footnote-ref" href="#fn:label1" rel="footnote">1</a></sup> and the footnote's content<sup id="fnref:label2"><a class="footnote-ref" href="#fn:label2" rel="footnote">2</a></sup>.</p>

<div class="footnote">
  <hr>
  <ol>
    <li id="fn:label1">
      <p>A footnote on the label: "label1".&#160;<a class="footnote-backref" href="#fnref:label1" rev="footnote" title="Jump back to footnote 1 in the text">&#8617;</a></p>
    </li>
    <li id="fn:label2">
      <p>A footnote on the label: "label2".&#160;<a class="footnote-backref" href="#fnref:label2" rev="footnote" title="Jump back to footnote 2 in the text">&#8617;</a></p>
    </li>
  </ol>
</div>
```

## Admonition

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

!!! info
    You should note that the title will be automatically capitalized.

!!! warn "Don't try this at home"
    You should note that the title will be automatically capitalized.

!!! error ""
    This is a admonition box without a title.

**Markdown** Input:

```markdown
!!! info
    You should note that the title will be automatically capitalized.

!!! warn "Don't try this at home"
    You should note that the title will be automatically capitalized.

!!! error ""
    This is a admonition box without a title.
```

**HTML** Output:

```html
<div class="admonition info">
  <p class="admonition-title">Note</p>
  <p>You should note that the title will be automatically capitalized.</p>
</div>

<div class="admonition warn">
  <p class="admonition-title">Don't try this at home</p>
  <p>You should note that the title will be automatically capitalized.</p>
</div>

<div class="admonition error">
<p>This is a admonition box without a title.</p>
```

## Superscript

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

2^^10^^=1024

**Markdown** Input:

```markdown
2^^10^^=1024
```

**HTML** Output:

```html
<p>2<sup>10</sup>=1024</p>
```

## Subscript

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

Demo:

H~2~O = water

**Markdown** Input:

```markdown
H~2~O = water
```

**HTML** Output:

```html
<p>H<sub>2</sub>O = water</p>
```

## Meta Data

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

```markdown
TOPIC: python
AUTHORS: contributor; contributor@dookbook.info; github:dookbook;

# Heading 1

body text here
```

## Task List

!!! warn "GitHub Flavored Markdown"
    This is the *GitHub Flavored Markdown* syntax.

!!! error "Unsupported Syntax"
    *Dookbook Markdown* does **NOT** support for this syntax.

Demo:

- [x] @mentions, #refs, [links](URL), **formatting**, and ~~tags~~ are supported
- [x] list syntax is required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

**Markdown** Input:

```markdown
- [x] @mentions, #refs, [links](URL), **formatting**, and ~~tags~~ are supported
- [x] list syntax is required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```

## Keyboard Input

Demo:

!!!Ctrl!!! + !!!C!!!

**Markdown** Input:

```markdown
!!!Ctrl!!! + !!!C!!!
```

**HTML** Output:

```html
<kbd>Ctrl</kbd> + <kbd>C</kbd>
```

## Math - TeX/Latex Mathematical Formulae

Inline:

\\(x = a + b - c \pm d * e / f\\)

```markdown
\\(x = a + b - c \pm d * e / f\\)
```

Block:

$$
x = a + b - c \pm d * e / f
$$

```markdown
$$
x = a + b - c \pm d * e / f
$$
```

### `+`, `-`, `*`, `/`, `=`

$$
x = a + b - c \pm d * e / f
$$

**Markdown** Input:

```markdown
$$
x = a + b - c \pm d * e / f
$$
```

### `frac`

$$
x = \frac{a}{b + c} + d
$$

**Markdown** Input:

```markdown
$$
x = \frac{a}{b + c} + d
$$
```

### Subscript

$$
x = a_0 + \frac{1}{a_1 + \frac{1}{a_2 + \frac{1}{a_3 + a_4}}}
$$

**Markdown** Input:

```markdown
$$
x = a_0 + \frac{1}{a_1 + \frac{1}{a_2 + \frac{1}{a_3 + a_4}}}
$$
```

### Superscript

$$
x = a^2 + b^{2 + c_0}
$$

**Markdown** Input:

```markdown
$$
x = a^2 + b^{2 + c_0}
$$
```

### `sqrt`

$$
-b \pm \sqrt{b^2 - 4ac} \over 2a
$$

**Markdown** Input:

```markdown
$$
-b \pm \sqrt{b^2 - 4ac} \over 2a
$$
```

### Set

$$
\forall x \in X, \quad \exists y \leq \epsilon
$$

**Markdown** Input:

```markdown
$$
\forall x \in X, \quad \exists y \leq \epsilon
$$
```

### Limits

$$
\lim\limits_{x\rightarrow\infty}\frac{1}{x}
$$

**Markdown** Input:

```markdown
$$
\lim\limits_{x\rightarrow\infty}\frac{1}{x}
$$
```

### Calculus

$$
\int f(x)dx
$$

**Markdown** Input:

```markdown
$$
\int f(x)dx
$$
```

$$
\int_{a}^{b}f(x)dx
$$

**Markdown** Input:

```markdown
$$
\int_{a}^{b}f(x)dx
$$
```

### LaTex Notation

![LaTex Notation](/media/help__latex-notation.png)

## References

- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
- [Writing on GitHub](https://help.github.com/categories/writing-on-github/)
