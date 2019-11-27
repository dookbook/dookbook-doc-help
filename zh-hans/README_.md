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

## 文档编辑须知

- 文档命名不要包含**空格**，可用下划线`_`代替。
- 同一主题，*中英文*文档**命名一致**。
- 文档中必须包含`TOPIC`或者`TOPICS`元数据，用以说明文档主题，且**不能**与已存在的主题相同。
- 如果文档内容提交者不是原作者，请用`AUTHORS`元数据注明，每个作者占用一行。格式:
  `<作者名称>; <作者邮箱地址>; <账户类别>:<作者账号>`,
  例如：`Bob; bob@github.com; github:bob`
- 请同时提交中英文两种语言的文档，可使用翻译工具，建议使用[Google翻译](https://translate.google.cn/)。
- 文档中引用的外部链接，尽可能使用权威网站来源。
- 文档内容尽可能精简，优先示例，避免长篇累牍的术语介绍。
- 合理使用`**`, `*`来标注重要的文本内容。
- 尽可能使用**Wikilink**或**站内链接**来关联系统已存在的术语。
