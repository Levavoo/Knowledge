# Defined Commands

This folder defines the fixed commands and modifiers used for the Knowledge repository.

## Main command

```text
/new <term> [modifiers]
```

The `/new` command creates a new atomic entry. If the user does not specify modifiers, the assistant decides which entry types are useful.

## Supported command forms

| Command | Meaning | Example |
|---|---|---|
| `/new <term>` | Create the best default set of entries. | `/new variance` |
| `/new <term> --minimal` | Create only the essential entry. | `/new API --minimal` |
| `/new <term> --full` | Create concept plus all useful supporting entries. | `/new gaussian distribution --full` |
| `/new <term> --formula` | Force a formula entry. | `/new cosine similarity --formula` |
| `/new <term> --code` | Force a code entry. | `/new gradient descent --code` |
| `/new <term> --example` | Force an example entry. | `/new variance --example` |
| `/new <term> --flashcards` | Force flashcards. | `/new decision tree --flashcards` |
| `/new <term> --vocabulary` | Force a vocabulary entry. | `/new regression --vocabulary` |
| `/new <term> --rus` | Translate to Russian and add vocabulary. | `/new likelihood --rus` |
| `/new <term> --book` | Mark the active book as source context. | `/new derivative --book` |
| `/new <term> --source` | Use provided source text, page, course, or documentation. | `/new API endpoint --source` |
| `/new question "..."` | Create a question entry. | `/new question "Why use n - 1?"` |

## Default assistant behavior

For `/new <term>`, decide whether to create:

1. `Concepts/<term>.md`
2. `Formulas/<term>.md`
3. `Code/<term>.md`
4. `Examples/<term>_example.md`
5. `Flashcards/<term>.md`
6. `Vocabulary/<topic>_terms.md` or a vocabulary row

Do not create unnecessary files. For example, `API` probably does not need `Formulas/api.md`, but `variance` probably does need `Formulas/variance.md`.

## Output rule

When creating entries, first state the planned files, then create or update them.
