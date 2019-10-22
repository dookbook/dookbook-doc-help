TOPIC: markdown

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

```markdown
# Level-1 Heading

## Level-2 Heading

### Level-3 Heading
```

```html
<h1>Level-1 Heading</h1>

<h2>Level-2 Heading</h2>

<h3>Level-3 Heading</h3>
```

## Paragraph

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

```markdown
Paragraph 1

Paragraph 2
```

```html
<p>Paragraph 1</p>
<p>Paragraph 2</p>
```

## List

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

### Unordered List

```markdown
- Item 1
  - Item 1.1
  - Item 1.2
- Item 2
```

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

```markdown
1. Item 1
1. Item 2
```

```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```

### Definition List

```markdown
Apple
:   Pomaceous fruit of plants of the genus Malus in
    the family Rosaceae.

Orange
:   The fruit of an evergreen tree of the genus Citrus.
```

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

```markdown
This text will be **bold**

This will also be __bold__
```

```html
This text will be <strong>bold</strong>

This will also be <strong>bold</strong>
```

### Italic Text

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

```markdown
*This text will be italic*

_This will also be italic_
```

```html
<em>This text will be italic</em>

<em>This will also be italic</em>
```

### Deleted Text

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

```markdown
~~Deleted Text~~
```

```html
<del>Deleted Text</del>
```

### Inserted Text

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

```markdown
++Inserted Text++
```

```html
<ins>Inserted Text</ins>
```

### Combined Emphasis Text

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

```markdown
Combined emphasis with **asterisks and _underscores_**.
```

```html
Combined emphasis with <strong>asterisks and <em>underscores</em></strong>.
```

## Horizontal Rule

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

```markdown
***
```

```html
<hr/>
```

## Link

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

```markdown
[Link Text](URL)

[Link Text](URL "Tip Text")
```

```html
<a href="URL">Link Text</a>

<a href="URL" title="Tip Text">Link Text</a>
```

## Image

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

```markdown
![Alt Text](URL)
```

```html
<img src="URL" alt="Alt Text"/>
```

## Inline Code

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

```markdown
`code here`
```

```html
<code>code here</code>

<value>code here</value>
```

## Table

### Raw Table

!!! info "Standard Markdown"
    This is the *standard Markdown* syntax.

```markdown
| Name | Description | Hot |
| ------------- | --- | --- |
| Help | Display the help window.| 5 |
| **Close** | *Closes* a `window` | 1000 |

<!-- 1. There must be at least 3 dashes separating each header cell. -->

<!-- 2. The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown. -->
```

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

```markdown
<!-- Colons can be used to align columns: right-aligned, centered, and neat -->

| Name | Description (centered) | Hot (right-aligned) |
| ------------- | :---: | ---: |
| Help | Display the help window.| 5 |
| **Close** | *Closes* a `window` | 1000 |
```

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

```markdown
As Kanye West said:

> We're living the future so
> the present is our past.
```

```html
<p>As Kanye West said:</p>

<blockquote>We're living the future so
  the present is our past.</blockquote>
```

## Abbreviations

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

```markdown
The HTML specification
is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium
```

```html
<p>The <abbr title="Hyper Text Markup Language">HTML</abbr> specification
is maintained by the <abbr title="World Wide Web Consortium">W3C</abbr>.</p>
```

## Code Block

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

<!-- markdownlint-disable MD031 -->
```markdown
```python
print ('Hello world')
``` // end
```
<!-- markdownlint-enable MD031 -->

```html
<pre><code>
print ('Hello world')
</code></pre>
```

## Attribute List

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

```markdown
## Attribute List {: #head-id}

Windows lets you perform most tasks directly from the keyboard. This page lists out the default bindings (keyboard shortcuts). Windows lets you perform most tasks directly from the keyboard. This page lists out the **default**{: attrname="value" } bindings (keyboard shortcuts).
{: #someid .someclass attrname='value' }
```

```html
<h2 id="head-id">Attribute List</h2>
<p attrname="value" class="someclass" id="someid">Windows lets you perform most tasks directly from the keyboard. This page lists out the default bindings (keyboard shortcuts). Windows lets you perform most tasks directly from the keyboard. This page lists out the <strong attrname="value">default</strong> bindings (keyboard shortcuts).</p>
```

## Footnote

!!! warn "Dookbook Markdown"
    This is the *Dookbook Markdown* syntax.

```markdown
Footnotes have a label[^label1] and the footnote's content[^label2].

[^label1]: A footnote on the label: "label1".
[^label2]: A footnote on the label: "label2".

///Footnotes Go Here///
```

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

```markdown
!!! note
    You should note that the title will be automatically capitalized.

!!! danger "Don't try this at home"
    You should note that the title will be automatically capitalized.

!!! important ""
    This is a admonition box without a title.
```

```html
<div class="admonition note">
  <p class="admonition-title">Note</p>
  <p>You should note that the title will be automatically capitalized.</p>
</div>

<div class="admonition danger">
  <p class="admonition-title">Don't try this at home</p>
  <p>You should note that the title will be automatically capitalized.</p>
</div>

<div class="admonition important">
<p>This is a admonition box without a title.</p>
```

## References

- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
- [Writing on GitHub](https://help.github.com/categories/writing-on-github/)
