# Command Modifiers

Modifiers control what supporting files should be created for a `/new` command.

## Main modifiers

| Modifier | Purpose | Typical output |
|---|---|---|
| `--minimal` | Create only the most essential entry. | `Concepts/<term>.md` or vocabulary row |
| `--full` | Create all useful supporting entries. | Concept + formula/code/example/flashcards/vocabulary if useful |
| `--formula` | Force formula-focused entry. | `Formulas/<term>.md` |
| `--code` | Force code-focused entry. | `Code/<term>.md` |
| `--example` | Force worked example. | `Examples/<term>_example.md` |
| `--flashcards` | Force review cards. | `Flashcards/<term>.md` |
| `--vocabulary` | Force vocabulary entry. | `Vocabulary/<topic>_terms.md` row or file |
| `--rus` | Translate to Russian and define. | Vocabulary row with English, German, Russian, meaning, tags |
| `--book` | Use active book/source context. | Source front matter with book details |
| `--source` | Use provided source text or reference. | Source front matter with source details |

## Modifier combinations

Modifiers can be combined:

```text
/new variance --formula --example
/new cosine similarity --formula --code --example
/new gaussian distribution --full
/new likelihood --rus
/new gradient descent --code --formula
```

## Decision rules

### Use `--formula` when

- the concept has a mathematical formula
- symbols and notation matter
- calculation steps matter
- the formula is likely to be reused

Examples: variance, standard deviation, Gaussian distribution, cosine similarity, gradient descent update rule.

### Use `--code` when

- implementation helps understanding
- from-scratch code is useful
- the concept is common in Python, SQL, or data workflows

Examples: linear regression, gradient descent, cosine similarity, train-test split.

### Use `--example` when

- the concept is abstract
- numbers, a scenario, or a small dataset make it clearer
- the entry should be usable for exam/project revision

Examples: variance, SQL JOIN, decision tree classification, API request-response cycle.

### Use `--rus` when

- the user wants vocabulary support
- the word is English or German and should be translated to Russian
- the term belongs to technical vocabulary

Example output format:

```md
| English | German | Russian | Simple Meaning | Tags |
|---|---|---|---|---|
| likelihood | Likelihood / Plausibilität | правдоподобие | How plausible data is under a model | statistics, machine-learning |
```

## Default rule

If no modifier is given, the assistant chooses the useful set of entries and explains why.
