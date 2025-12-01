# English Vocabulary Trainer

Claude Code Plugin for English vocabulary learning. Manage words, practice with flashcard-style quizzes, and improve speaking skills through roleplay conversations.

## Installation

```bash
/plugin install https://github.com/namtoki/english-vocabulary-trainer
```

## Commands

| Command | Description |
|---------|-------------|
| `/evt:words [n\|word]` | Add vocabulary words (by count or specific word) |
| `/evt:cliche [n\|phrase]` | Add cliche/fixed expressions |
| `/evt:framework [n\|pattern]` | Add sentence framework patterns |
| `/evt:anki [n]` | Start a flashcard quiz with n questions |
| `/evt:rollplay start` | Start an English conversation roleplay |
| `/evt:rollplay end` | End roleplay and save conversation log |


## Word Format

Words are stored in markdown files with the following format:

```markdown
## Category Name
- `word` /pronunciation/ ([Register] Japanese meaning) Example sentence.
  - `synonym1` /pronunciation/ ([Register] meaning) Example.
  - `synonym2` /pronunciation/ ([Register] meaning) Example.
```

**Registers:**
- `[Formal]` - Formal/business contexts
- `[Neutral]` - General use
- `[Casual]` - Informal/spoken contexts

## Features

### Vocabulary Management (`/evt:words`, `/evt:cliche`, `/evt:framework`)
- Add words from major word lists (NGSL, GSL, AWL, COCA, SVL 12000)
- Categorize by part of speech and semantic field
- Include pronunciation, register, meaning, and example sentences
- Search YouGlish for real-world usage videos

### Flashcard Quiz (`/evt:anki`)
- Random selection from your vocabulary
- Interactive quiz format with reveal
- Track which file each word came from

### Conversation Roleplay (`/evt:rollplay`)
- Practice speaking with current news topics
- Get feedback on your expressions
- Learn more natural ways to say things
- Save conversation logs for review

## License

MIT
