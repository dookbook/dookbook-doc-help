TOPICS: readme

# Dookbook Help

Dookbook&reg; (Developers' Cookbook) Document Library (Help Documentation)

## About Dookbook

Please refer to [about Dookbook&reg;](https://dookbook.info/about/)

## Preparation in advance

1. [GitHub OAuth](https://dookbook.info/helper/github/oauth/en/)
2. Clone this repo
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

## Editing Rules

1. **DO NOT** include **spaces**, `(`, `)`, `?`, `:`, `<`, `>`, `*`, `\`, `/` in the document name, use
   the underscore `_` instead.
2. Both *Chinese* and *English* documents have **the same name** on the same subject.
3. The document must contain `TOPIC` or `TOPICS` metadata to describe the topic of the document and
   **must not** be the same as an existing topic.
4. Do not include acronyms in `TOPIC`/`TOPICS` , please use the full name.
5. If the submitter of the document content is not the original author, please use the `AUTHORS`
   metadata to indicate that *each author occupies one line*. Format:
   `TOPIC: <Author name>; <author email address>; <account type>: <author account>`.
   For example: `Bob; bob@github.com; github:bob`
6. Please submit documents in both Chinese and English. Translation tools are available.
   **[Google Translation](https://translate.google.cn/)** is recommended.
7. External links referenced in the document should be from authoritative website whenever possible.
8. The document content is as concise as possible, giving priority to examples and avoiding lengthy terminology.
9. Use `**`, `*` appropriately to mark important text content.
10. Wherever possible, use **Wikilink** or **internal links** to correlate existing terms in the system.
11. If there is an **illustration** (*images*) in the document, please put the image in the `images`
    directory and submit it with the document. Format of reference image address in the document:
    `![image alt text](/media/<subject-name>__<image-file-name>)`.
    For example: `![Anatomy of an HTML element](/media/glossary__anatomy-of-an-html-element.png)`
12. If there are **abbreviations** in the document, please indicate the metadata `ABBR` at the
    beginning of the document, *each abbreviation occupies one line*. Format:
    `ABBR: <abbr> = <full-word>`. For example: `ABBR: HTML = HyperText Markup Language`
