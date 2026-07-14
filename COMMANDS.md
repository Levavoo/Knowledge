# Commands

This file is the short command reference. The detailed command/modifier documentation lives in `Commands/`.

## Core syntax

```text
/new <term> [modifiers]
```

If no modifier is provided, the assistant decides which supporting entries are useful.

## Most used commands

| Command | Purpose | Example |
|---|---|---|
| `/new <term>` | Create a new knowledge entry and choose useful support files. | `/new variance` |
| `/new <term> --formula` | Force a formula entry. | `/new variance --formula` |
| `/new <term> --code` | Force a code-focused entry. | `/new gradient descent --code` |
| `/new <term> --example` | Force a worked example entry. | `/new cosine similarity --example` |
| `/new <term> --rus` | Add vocabulary with Russian translation and definition. | `/new likelihood --rus` |
| `/new question "..."` | Save a learning question. | `/new question "Why use n - 1 in sample variance?"` |

## Available modifiers

```text
--minimal
--full
--formula
--code
--example
--flashcards
--vocabulary
--rus
--book
--source
```

## Assistant decision rule

For every `/new <term>` request, decide whether the term needs:

- `Concepts/` entry: almost always
- `Formulas/` entry: if there is important math notation or calculation logic
- `Code/` entry: if implementation matters or from-scratch code helps understanding
- `Examples/` entry: if the concept becomes clearer with a worked example
- `Flashcards/` entry: if it is exam-relevant or easy to forget
- `Vocabulary/` entry: if English/German/Russian terminology matters

## File naming

Use lowercase snake case:

```text
variance.md
cosine_similarity.md
gaussian_distribution.md
gradient_descent_from_scratch.md
```

## Folder names

Use the capitalized folders defined in `README.md`:

```text
Concepts/
Formulas/
Code/
Examples/
Flashcards/
Vocabulary/
Templates/
Books/
Commands/
```
