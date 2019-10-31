TOPICS: readme

# Dookbook帮助

Dookbook&reg; (Developers' Cookbook) 开发者的日常菜谱 - 文档库帮助文档

## 关于Dookbook

请参考[关于Dookbook&reg;](https://dookbook.info/about/zh-hans/)

## 前期准备

1. 克隆仓库
2. 打开并安装[GitHub App](https://github.com/apps/dookbook)
3. 增加上游仓库地址到你本地

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
