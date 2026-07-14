# Knowledge

Personal atomic knowledge base for data analytics, machine learning, statistics, programming, mathematics, exam preparation, and multilingual technical vocabulary.

The repository is organized around small reusable entries. Each entry should explain one term, concept, formula, code implementation, worked example, flashcard set, or vocabulary item.

## Repository structure

```text
Knowledge/
├── README.md
├── COMMANDS.md
├── TAG_INDEX.md
├── .gitignore
│
├── Books/
│   └── README.md
├── Concepts/
├── Formulas/
├── Code/
├── Examples/
├── Flashcards/
├── Vocabulary/
├── Commands/
│   ├── README.md
│   └── modifiers.md
└── Templates/
    ├── concept_entry.md
    ├── formula_entry.md
    ├── code_entry.md
    ├── example_entry.md
    └── vocabulary_entry.md
```

## Folder purpose

| Folder | Purpose |
|---|---|
| `Books/` | Local book storage and reading context. Do not commit copyrighted PDFs. |
| `Concepts/` | Main explanations for terms, concepts, and theories. |
| `Formulas/` | Mathematical formulas, symbols, derivations, and calculation logic. |
| `Code/` | Code-focused learning entries and from-scratch implementations. |
| `Examples/` | Worked examples, practical situations, and use cases. |
| `Flashcards/` | Review questions and Anki-style learning cards. |
| `Vocabulary/` | English/German/Russian vocabulary entries and terminology tables. |
| `Commands/` | Defined assistant commands and allowed modifiers. |
| `Templates/` | Reusable Markdown templates for new entries. |

## Core workflow

Use this chat with commands like:

```text
/new variance
/new variance --formula --example
/new cosine similarity --formula --code --example
/new likelihood --rus
/new gradient descent --code --formula
/new question Why does gradient descent need a learning rate?
```

If no modifier is provided, the assistant decides which supporting files are useful.

## Entry standard

Every normal concept entry should include:

- short definition
- simple explanation in English
- technical explanation in English
- example
- use case
- common mistakes, if useful
- related entries
- tags
- source reference, if relevant

Formula-heavy concepts may also receive `Formulas/` entries. Code-heavy concepts may also receive `Code/` entries. Practical concepts may also receive `Examples/` entries.

## Source rule

When a note comes from a book, course, video, school task, or documentation page, add a source reference in the front matter. For copyrighted books, write your own explanation and page/chapter reference instead of copying long passages.

## Book storage rule

`Books/` may be used locally for PDFs and other book files, but the repository should not commit copyrighted PDFs. The `.gitignore` blocks common book formats by default.
