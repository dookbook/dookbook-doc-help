TOPICS: readme

# Dookbook帮助

Dookbook&reg; (Developers' Cookbook) 开发者的日常菜谱 - 文档库帮助文档

## 关于Dookbook

请参考[关于Dookbook&reg;](https://dookbook.info/about/zh-hans/)

## 前期准备

1. 克隆仓库
2. 增加上游仓库地址到你本地

!!! info "小贴士"
    应该替换`<repo-name>`为真实的文档仓库名称。

```bash
git remote add upstream https://github.com/dookbook/<repo-name>.git
```

## 与上游同步

```bash
git pull upstream master

git push origin master
```

## 注意事项

- **强烈建议**用*主题分支*提交文档

```bash
git checkout <topic-branch>
git pull
git rebase master
git push

<commits ...>

git push
```

- 此文档库中所有的文档都是由**Markdown**语言撰写，所支持的语法规则及示例
请参考[Dookbook帮助 - Markdown](https://dookbook.info/zh-hans/help/markdown/)

- 最好每次只提交较小的修改，并写好清晰明确的**Commit Messages（提交说明）**.

## 编辑规则

1. 文档命名不要包含**空格**，可用下划线`_`代替。
1. 同一主题，*中英文*文档**命名一致**。
1. 文档中必须包含`TOPIC`或者`TOPICS`元数据，用以说明文档主题，且**不能**与已存在的主题相同。
1. `TOPIC`/`TOPICS`中不要含有缩略语，请使用全称。
1. 如果文档内容提交者不是原作者，请用`AUTHORS`元数据注明，每个作者占用一行。格式:
   `AUTHORS: <作者名称>; <作者邮箱地址>; <账户类别>:<作者账号>`，
   例如：`Bob; bob@github.com; github:bob`
1. 请同时提交中英文两种语言的文档，可使用翻译工具，建议使用[Google翻译](https://translate.google.cn/)。
1. 文档中引用的外部链接，尽可能使用权威网站来源。
1. 文档内容尽可能精简，优先示例，避免长篇累牍的术语介绍。
1. 合理使用`**`, `*`来标注重要的文本内容。
1. 尽可能使用**Wikilink**或**站内链接**来关联系统已存在的术语。
1. 如文档中有插图，请将图片放至`images`目录下，随文档一并提交。文档中引用图片地址格式：
   `![图片的替代文字](/media/<主题名称>__<图片文件名>)`，例如：假设图片文件名为`anatomy-of-an-html-element.png`,
   那文档中引用图片的格式为`![Anatomy of an HTML element](/media/glossary__anatomy-of-an-html-element.png)`
1. 如果文档中存在缩略语，请在文档开头处注明元数据`ABBR`，每个缩略语占用一行。格式：
   `ABBR: <缩略语> = <全称>`，例如：`ABBR: HTML = HyperText Markup Language`
