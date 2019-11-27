TOPICS: readme

# Dookbook Help

Dookbook&reg; (Developers' Cookbook) Document Library (Help Documentation)

## About Dookbook

Please refer to [about Dookbook&reg;](https://dookbook.info/about/)

## Preparation in advance

1. Clone this repo
2. Add original (upstream) repo into your local git.

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

## Document Editing Notes

- **DO NOT** include **spaces** in the document name, use the underscore `_` instead.
- Both *Chinese* and *English* documents have **the same name** on the same subject.
- The document must contain `TOPIC` or `TOPICS` metadata to describe the topic of the document and
  **must not** be the same as an existing topic.
- If the submitter of the document content is not the original author, please use the `AUTHORS`
  metadata to indicate that each author occupies one line. Format:
  `<Author name>; <author email address>; <account type>: <author account>`.
  For example: `Bob; bob@github.com; github:bob`
- Please submit documents in both Chinese and English. Translation tools are available.
  **[Google Translation](https://translate.google.cn/)** is recommended.
- External links referenced in the document should be from authoritative website whenever possible.
- The document content is as concise as possible, giving priority to examples and avoiding lengthy terminology.
- Use `**`, `*` appropriately to mark important text content.
- Wherever possible, use **Wikilink** or **internal links** to correlate existing terms in the system.
