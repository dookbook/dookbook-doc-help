TOPICS: readme

# Dookbook Help

Dookbook&reg; (Developers' Cookbook) Document Library (Help Documentation)

## About Dookbook

Please refer to [about Dookbook&reg;](https://dookbook.info/about/)

## Preparation in advance

1. Clone this repo
2. Open and install [GitHub App](https://github.com/apps/dookbook).
3. Add original (upstream) repo into your local git.

!!! info "Tips"
    `<repo-name>` should be replaced by the real repo name.

```bash
git remote add upstream https://github.com/dookbook/<repo-name>.git
```

## Synchronization with original (upstream) repo

```bash
git pull upstream master

git push origin master
```

## Attention

- Submitting documents with *topic branches* is **strongly recommended**

```bash
git checkout <topic-branch>
git pull
git rebase master
git push

<commits ...>

git push
```

- All documents in this library are written in **Markdown**,
more details please refer to [Dookbook Help - Markdown](https://dookbook.info/en/help/markdown/)

- It's better to submit only minor changes at a time and write clear **Commit Messages**.
