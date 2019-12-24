TOPICS: markdown

# Markdown

**Markdown**是一种轻量级的标记语言。通过简单的标记语法，它允许人们使用易读易写的纯文本格式编写文档，并可转换成各种不同的文档格式
（例如：*HTML*, *Word*, 图片, *PDF*, *epub*等）。
同时，由于它能够非常方便地被*Git*或其他版本控制系统进行版本控制，所以非常适合作为源代码的文档编写语言。它也经常被许多论坛、博客主用来编辑论坛贴和博客内容。

Markdown语言在2004由*约翰·格鲁伯*创建。

!!! info "小贴士"
    Markdown编写的文档*后缀*为`.md`或`.markdown`。

## 标题

!!! info "标准Markdown"
    此为*标准Markdown*语法。

**Markdown**输入:

```markdown
# 一级标题

## 二级标题

### 三级标题
```

**HTML**输出:

```html
<h1>一级标题</h1>

<h2>二级标题</h2>

<h3>三级标题</h3>
```

## 段落

!!! info "标准Markdown"
    此为*标准Markdown*语法。

**Markdown**输入:

```markdown
段落1

段落2
```

**HTML**输出:

```html
<p>段落1</p>
<p>段落2</p>
```

## 列表

!!! info "标准Markdown"
    此为*标准Markdown*语法。

### 无序列表

演示示例：

- 列表项目 1
    - 列表项目 1.1
    - 列表项目 1.2
- 列表项目 2

**Markdown**输入:

```markdown
- 列表项目 1
    - 列表项目 1.1
    - 列表项目 1.2
- 列表项目 2
```

**HTML**输出:

```html
<ul>
  <li>列表项目 1</li>
  <ul>
    <li>列表项目 1.1</li>
    <li>列表项目 1.2</li>
  </ul>
  <li>列表项目 2</li>
</ul>
```

### 有序列表

演示示例：

1. 列表项目 1
2. 列表项目 2

**Markdown**输入：

```markdown
1. 列表项目 1
2. 列表项目 2
```

**HTML**输出：

```html
<ol>
  <li>列表项目1</li>
  <li>列表项目2</li>
</ol>
```

### 定义列表

演示示例：

Apple
:   Pomaceous fruit of plants of the genus Malus in
    the family Rosaceae.

Orange
:   The fruit of an evergreen tree of the genus Citrus.

**Markdown**输入：

```markdown
Apple
:   Pomaceous fruit of plants of the genus Malus in
    the family Rosaceae.

Orange
:   The fruit of an evergreen tree of the genus Citrus.
```

**HTML**输出：

```html
<dl>
  <dt>Apple</dt>
  <dd>Pomaceous fruit of plants of the genus Malus in the family Rosaceae.</dd>

  <dt>Orange</dt>
  <dd>The fruit of an evergreen tree of the genus Citrus.</dd>
</dl>
```

## 文本

### 强调文本

!!! info "标准Markdown"
    此为*标准Markdown*语法。

!!! warn
    双下划线`__`不支持中文!

演示示例：

这是**强调文字**

**Markdown**输入：

```markdown
这是**强调文字**

这不支持中文__强调文字__
```

**HTML**输出：

```html
这是<strong>强调文字</strong>

这不支持中文<strong>强调文字</strong>
```

### 斜体文本

!!! info "标准Markdown"
    此为*标准Markdown*语法。

演示示例：

<!-- markdownlint-disable MD036 -->
*次强调文字， 斜体*

_这也是次强调文字，斜体_
<!-- markdownlint-enable MD036 -->

**Markdown**输入：

```markdown
*次强调文字， 斜体*

_这也是次强调文字，斜体_
```

**HTML**输出：

```html
<em>次强调文字， 斜体</em>

<em>这也是次强调文字，斜体</em>
```

### 删除文本

!!! info "标准Markdown"
    此为*标准Markdown*语法。

演示示例：

~~删除的文字~~

**Markdown**输入：

```markdown
~~删除的文字~~
```

**HTML**输出：

```html
<del>删除的文字</del>
```

### 插入文本

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

++插入的文字++

**Markdown**输入：

```markdown
++插入的文字++
```

**HTML**输出：

```html
<ins>插入的文字</ins>
```

### 混合文本

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

混合的文本**强调和 _斜体_**.

**Markdown**输入：

```markdown
混合的文本**强调和 _斜体_**.
```

**HTML**输出：

```html
混合的文本<strong>强调和 <em>斜体</em></strong>.
```

## 水平分割线

!!! info "标准Markdown"
    此为*标准Markdown*语法。

**Markdown**输入：

```markdown
***
```

**HTML**输出：

```html
<hr/>
```

## 链接

!!! info "标准Markdown"
    此为*标准Markdown*语法。

演示示例：

此处有[链接](https://dookbook.info/)。

此处有[链接](https://dookbook.info/ "Dookbook主页")。

**Markdown**输入：

```markdown
此处有[链接](https://dookbook.info/)。

此处有[链接](https://dookbook.info/ "Dookbook主页")。
```

**HTML**输出：

```html
此处有<a href="https://dookbook.info/">链接</a>。

此处有<a href="https://dookbook.info/" title="Dookbook主页">链接</a>。
```

## 图片

!!! info "标准Markdown"
    此为*标准Markdown*语法。

**Markdown**输入：

```markdown
![替换文本](URL)
```

**HTML**输出：

```html
<img src="URL" alt="替换文本"/>
```

## 行内代码

!!! info "标准Markdown"
    此为*标准Markdown*语法。

演示示例：

<!-- markdownlint-disable MD031 -->
```markdown
```markdown
`code here`
``` // end
```
<!-- markdownlint-enable MD031 -->

**Markdown**输入：

```markdown
`code here`
```

**HTML**输出：

```html
<code>code here</code>

<value>code here</value>
```

## 表格

### 原始表格

!!! info "标准Markdown"
    此为*标准Markdown*语法。

演示示例：

| 名称 | 描述 | 热度 |
| ------------- | --- | --- |
| 帮助 | 显示帮助窗口。| 5 |
| **关闭** | *关闭*一个`窗口` | 1000 |

**Markdown**输入：

```markdown
| 名称 | 描述 | 热度 |
| ------------- | --- | --- |
| 帮助 | 显示帮助窗口。| 5 |
| **关闭** | *关闭*一个`窗口` | 1000 |

<!-- 1. 至少需要3个短线或虚线分隔表格标题跟表格内容单元。-->

<!-- 2. 最外层的"|"是可选的。你也可以使用Markdown的行内元素。-->
```

**HTML**输出：

```html
<table>
  <thead>
    <tr>
      <th>名称</th>
      <th>描述</th>
      <th>热度</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>帮助</td>
      <td>显示帮助窗口。</td>
      <td>5</td>
    </tr>
    <tr>
      <td><strong>关闭</strong></td>
      <td><em>关闭</em>一个<code>窗口</code></td>
      <td>1000</td>
    </tr>
  </tbody>
</table>
```

### 列对齐

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

| 名称 | 描述 (居中) | 热度 (右对齐) |
| ------------- | :---: | ---: |
| 帮助 | 显示帮助窗口。| 5 |
| **关闭** | *关闭*一个`窗口` | 1000 |

**Markdown**输入：

```markdown
<!-- 冒号可以用来对齐列：右对齐，居中 -->

| 名称 | 描述 (居中) | 热度 (右对齐) |
| ------------- | :---: | ---: |
| 帮助 | 显示帮助窗口。| 5 |
| **关闭** | *关闭*一个`窗口` | 1000 |
```

**HTML**输出：

```html
<table>
  <thead>
    <tr>
      <th>名称</th>
      <th align="center">描述 (居中)</th>
      <th align="right">热度 (右对齐)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>帮助</td>
      <td align="center">显示帮助窗口。</td>
      <td align="right">5</td>
    </tr>
    <tr>
      <td><strong>关闭</strong></td>
      <td align="center"><em>关闭</em>一个<code>窗口</code></td>
      <td align="right">1000</td>
    </tr>
  </tbody>
</table>
```

## 引用块

!!! info "标准Markdown"
    此为*标准Markdown*语法。

演示示例：

As Kanye West said:

> We're living the future so
> the present is our past.

**Markdown**输入：

```markdown
As Kanye West said:

> We're living the future so
> the present is our past.
```

**HTML**输出：

```html
<p>As Kanye West said:</p>

<blockquote>We're living the future so
  the present is our past.</blockquote>
```

## 缩写

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

The HTML specification
is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium

**Markdown**输入：

```markdown
The HTML specification
is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium
```

**HTML**输出：

```html
<p>The <abbr title="Hyper Text Markup Language">HTML</abbr> specification
is maintained by the <abbr title="World Wide Web Consortium">W3C</abbr>.</p>
```

## 代码段

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

```python
print ('Hello world')
``` // end

**Markdown**输入：

<!-- markdownlint-disable MD031 -->
```markdown
```python
print ('Hello world')
``` // end
```
<!-- markdownlint-enable MD031 -->

**HTML**输出：

```html
<pre><code>
print ('Hello world')
</code></pre>
```

!!! warn "Dookbook Markdown"
    *Dookbook Markdown*支持9种语言代码语法高亮：
    `HTML`/`XML`, `CSS`, `JavaScript`, `Python`, `Markdown`,
    `Bash`, `INI`/`TOML`。

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
    *Dookbook Markdown*支持**ES6+**.

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

## 属性列表

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

**Markdown**输入：

```markdown
## Attribute List {: #head-id}

Windows lets you perform most tasks directly from the keyboard. This page lists out the default bindings (keyboard shortcuts). Windows lets you perform most tasks directly from the keyboard. This page lists out the **default**{: attrname="value" } bindings (keyboard shortcuts).
{: #someid .someclass attrname='value' }
```

**HTML**输出：

```html
<h2 id="head-id">Attribute List</h2>
<p attrname="value" class="someclass" id="someid">Windows lets you perform most tasks directly from the keyboard. This page lists out the default bindings (keyboard shortcuts). Windows lets you perform most tasks directly from the keyboard. This page lists out the <strong attrname="value">default</strong> bindings (keyboard shortcuts).</p>
```

## 脚注

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

Footnotes have a label[^label1] and the footnote's content[^label2].

[^label1]: A footnote on the label: "label1".
[^label2]: A footnote on the label: "label2".

///Footnotes Go Here///

**Markdown**输入：

```markdown
Footnotes have a label[^label1] and the footnote's content[^label2].

[^label1]: A footnote on the label: "label1".
[^label2]: A footnote on the label: "label2".

///Footnotes Go Here///
```

**HTML**输出：

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

## 警示

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

!!! info
    You should note that the title will be automatically capitalized.

!!! warn "Don't try this at home"
    You should note that the title will be automatically capitalized.

!!! error ""
    This is a admonition box without a title.

**Markdown**输入：

```markdown
!!! info
    You should note that the title will be automatically capitalized.

!!! warn "Don't try this at home"
    You should note that the title will be automatically capitalized.

!!! error ""
    This is a admonition box without a title.
```

**HTML**输出：

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

## 上标

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

2^10^=1024

**Markdown**输入：

```markdown
2^10^=1024
```

**HTML**输出：

```html
<p>2<sup>10</sup>=1024</p>
```

## 下标

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

演示示例：

H~2~O = water

**Markdown**输入：

```markdown
H~2~O = water
```

**HTML**输出：

```html
<p>H<sub>2</sub>O = water</p>
```

## 元数据

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

```markdown
TOPIC: python
AUTHORS: contributor; contributor@dookbook.info; github:dookbook;

# Heading 1

body text here
```

## 任务清单

!!! warn "GitHub Flavored Markdown"
    此为*GitHub Flavored Markdown*语法。

!!! error "语法不支持"
    *Dookbook Markdown*暂时不支持该语法。

演示示例：

- [x] @mentions, #refs, [links](URL), **formatting**, and ~~tags~~ are supported
- [x] 已完成
- [x] 已完成
- [ ] 未完成

**Markdown**输入：

```markdown
- [x] @mentions, #refs, [links](URL), **formatting**, and ~~tags~~ are supported
- [x] 已完成
- [x] 已完成
- [ ] 未完成
```

## 键盘输入

演示示例：

!!!Ctrl!!! + !!!C!!!

**Markdown**输入：

```markdown
!!!Ctrl!!! + !!!C!!!
```

**HTML**输出：

```html
<kbd>Ctrl</kbd> + <kbd>C</kbd>
```

## 数学 - TeX/LaTex数学公式

Inline:

```markdown
$...$
```

Block:

```markdown
$$
...
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
x = a^2+b^{2+c_0}
$$

**Markdown** Input:

```markdown
$$
x = a^2+b^{2+c_0}
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

### LaTex Notation

![LaTex Notation](/media/help__latex-notation.png)

## 参考资料

- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
- [Writing on GitHub](https://help.github.com/categories/writing-on-github/)
