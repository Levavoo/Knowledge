# Knowledge Index

This is the main navigation page for the Knowledge DB.

## Main areas

- [Terms](terms/)
- [Concepts](concepts/)
- [Formulas](formulas/)
- [Code](code/)
- [Examples](examples/)
- [Questions](questions/)
- [Books](books/)
- [Sources](sources/)
- [Tags](tags/)
- [Templates](templates/)

## Active book

- [O'Reilly Math Basics for Data Science](books/oreilly_math_basics_for_data_science.md)
- [Source note: O'Reilly Math Basics for Data Science](sources/oreilly_math_basics_for_data_science.md)

## Current source priorities

1. Active book sources, when we are working through a book
2. Related GitHub repository for practical code examples and formulas, if clearly connected to the book
3. scikit-learn documentation and repository for practical machine-learning concepts
4. Stable mathematical/statistical references for formulas

## Entry workflow

Use:

```text
/new [entry name] --options
```

For active book entries, use:

```text
/new [entry name] --book
/new [entry name] --book --formula
/new [entry name] --book --code --example
```

For learning questions, use:

```text
/new question [question text]
```

Common options:

```text
--formula
--code
--example
--rus
--de
--simple
--deep
--source
--book
```
