# Knowledge

Personal knowledge database for data analytics, machine learning, statistics, programming, and exam preparation.

This repository is organized around small atomic entries. Each entry should explain one term, concept, formula, code example, question, or source.

## Core workflow

Use this chat with commands like:

```text
/new decision tree --example --source
/new variance --formula
/new linear regression --code --example
/new API --rus
/new question Why does gradient descent need a learning rate?
```

The output should be saved into the matching folder.

## Active book workflow

Current active reading source:

```text
books/oreilly_math_basics_for_data_science.md
sources/oreilly_math_basics_for_data_science.md
```

When an entry comes from the active book, use:

```text
/new [term or concept] --book
/new [term or concept] --book --formula
/new [term or concept] --book --code --example
/new question [question text]
```

Book-related entries should include the tag:

```md
#oreilly-math-data-science
```

## Folder structure

```text
terms/       Short definitions and vocabulary entries
concepts/    Larger conceptual explanations
formulas/    Mathematical formulas and notation
code/        Code examples plus matching documentation files
examples/    Practical worked examples and use cases
questions/   Questions encountered while learning or reading
books/       Uploaded books, book notes, and reading context
sources/     Source notes and approved reference sources
tags/        Tag index pages
templates/   Reusable entry templates
```

## Entry standard

Every knowledge entry should normally contain:

- technical explanation
- simple explanation
- example
- use case
- related concepts
- source notes, if relevant

For code files, create a matching `.md` documentation file with the same base name.

## Question workflow

Use:

```text
/new question [question text]
```

Question entries are saved in `questions/` and should keep the original question visible, then add a short answer, detailed answer, related concepts, and follow-up questions.
