TOPIC: markdown

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

```markdown
# 一级标题

## 二级标题

### 三级标题
```

```html
<h1>一级标题</h1>

<h2>二级标题</h2>

<h3>三级标题</h3>
```

## 段落

!!! info "标准Markdown"
    此为*标准Markdown*语法。

```markdown
段落1

段落2
```

```html
<p>段落1</p>
<p>段落2</p>
```

## 列表

!!! info "标准Markdown"
    此为*标准Markdown*语法。

### 无序列表

```markdown
- 列表项目 1
  - 列表项目 1.1
  - 列表项目 1.2
- 列表项目 2
```

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

```markdown
1. 列表项目 1
1. 列表项目 2
```

```html
<ol>
  <li>列表项目1</li>
  <li>列表项目2</li>
</ol>
```

### 定义列表

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

## 文本

### 强调文本

!!! info "标准Markdown"
    此为*标准Markdown*语法。

!!! warn
    双下划线`__`不支持中文!

```markdown
这是**强调文字**

这不支持中文__强调文字__
```

```html
这是<strong>强调文字</strong>

这不支持中文<strong>强调文字</strong>
```

### 斜体文本

!!! info "标准Markdown"
    此为*标准Markdown*语法。

```markdown
*次强调文字， 斜体*

_这也是次强调文字，斜体_
```

```html
<em>次强调文字， 斜体</em>

<em>这也是次强调文字，斜体</em>
```

### 删除文本

!!! info "标准Markdown"
    此为*标准Markdown*语法。

```markdown
~~删除的文字~~
```

```html
<del>删除的文字</del>
```

### 插入文本

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

```markdown
++插入的文字++
```

```html
<ins>插入的文字</ins>
```

### 混合文本

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

```markdown
混合的文本**强调和 _斜体_**.
```

```html
混合的文本<strong>强调和 <em>斜体</em></strong>.
```

## 水平分割线

!!! info "标准Markdown"
    此为*标准Markdown*语法。

```markdown
***
```

```html
<hr/>
```

## 链接

!!! info "标准Markdown"
    此为*标准Markdown*语法。

```markdown
[链接文字](URL)

[链接文字](URL "提示文字")
```

```html
<a href="URL">链接文字</a>

<a href="URL" title="提示文字">链接文字</a>
```

## 图片

!!! info "标准Markdown"
    此为*标准Markdown*语法。

```markdown
![替换文本](URL)
```

```html
<img src="URL" alt="替换文本"/>
```

## 行内代码

!!! info "标准Markdown"
    此为*标准Markdown*语法。

```markdown
`code here`
```

```html
<code>code here</code>

<value>code here</value>
```

## 表格

### 原始表格

!!! info "标准Markdown"
    此为*标准Markdown*语法。

```markdown
| 名称 | 描述 | 热度 |
| ------------- | --- | --- |
| 帮助 | 显示帮助窗口。| 5 |
| **关闭** | *关闭*一个`窗口` | 1000 |

<!-- 1. 至少需要3个短线或虚线分隔表格标题跟表格内容单元。-->

<!-- 2. 最外层的"|"是可选的。你也可以使用Markdown的行内元素。-->
```

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

```markdown
<!-- 冒号可以用来对齐列：右对齐，居中 -->

| 名称 | 描述 (居中) | 热度 (右对齐) |
| ------------- | :---: | ---: |
| 帮助 | 显示帮助窗口。| 5 |
| **关闭** | *关闭*一个`窗口` | 1000 |
```

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

## 缩写

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

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

## 代码段

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

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

## 属性列表

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

```markdown
## Attribute List {: #head-id}

Windows lets you perform most tasks directly from the keyboard. This page lists out the default bindings (keyboard shortcuts). Windows lets you perform most tasks directly from the keyboard. This page lists out the **default**{: attrname="value" } bindings (keyboard shortcuts).
{: #someid .someclass attrname='value' }
```

```html
<h2 id="head-id">Attribute List</h2>
<p attrname="value" class="someclass" id="someid">Windows lets you perform most tasks directly from the keyboard. This page lists out the default bindings (keyboard shortcuts). Windows lets you perform most tasks directly from the keyboard. This page lists out the <strong attrname="value">default</strong> bindings (keyboard shortcuts).</p>
```

## 脚注

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

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

## 警示

!!! warn "Dookbook Markdown"
    此为*Dookbook Markdown*语法。

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

## 参考资料

- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
- [Writing on GitHub](https://help.github.com/categories/writing-on-github/)
