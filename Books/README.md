# Books

This folder is for local book files and reading context.

## Important rule

Do not commit copyrighted PDFs or ebooks to this public repository.

The repository `.gitignore` excludes common book formats:

```text
Books/*.pdf
Books/*.epub
Books/*.mobi
Books/*.azw3
```

Use this folder locally for books, but reference sources inside knowledge entries using front matter such as:

```yaml
source:
  type: book
  title: ""
  chapter: ""
  page: ""
```
