# French Writing Exercises

A personal French language learning project using structured creative writing to acquire and reinforce vocabulary.

## How It Works

Each session follows a **High-Structure Creative Writing** format:

1. A scenario prompt is generated based on target vocabulary from `vocabulary.txt`
2. A **12-Element Grid** constrains the writing: specific words, moods, characters, and narrative devices that must appear
3. The learner writes a short piece in French incorporating the grid elements
4. `frenchie`, the AI coaching agent, reads the attempt, cross-references vocabulary usage, and appends a corrected version with feedback

## Project Structure

```
.
├── vocabulary.txt        # Master word list (format: word - definition | ...)
├── exercises/            # All writing prompts, attempts, and corrected versions
│   ├── amitié fêlé.txt
│   ├── la bassine.txt
│   ├── la béquille.txt
│   ├── la détresse du travail.txt
│   ├── la haine.txt
│   ├── la montre.txt
│   ├── la neige et la faim.txt
│   ├── le café.txt
│   ├── le conflit.txt
│   ├── le forêt.txt
│   ├── le miroir rafistolé.txt
│   ├── le navire.txt
│   ├── le portrait.txt
│   ├── lâcher prise.txt
│   └── travail, quelle galère.txt
└── CLAUDE.md             # Agent instructions and project rules
```

## Vocabulary

`vocabulary.txt` holds the full target word list. Each entry follows the format:

```
word - definition | word - definition | ...
```

Words span a range of registers — from literary (*tire-d'aile*, *bée*, *courroucé*) to everyday colloquial (*galère*, *être crevé*, *chialer*) — with an emphasis on verbs and expressions that are hard to acquire passively.

## The `frenchie` Agent

The `frenchie` coaching agent:

- Reads `vocabulary.txt` at the start of each session to load target words
- Scans `exercises/` to understand recent progress and recurring errors
- Generates new scenario prompts that prioritize unused or misused vocabulary
- Appends corrected versions directly into exercise files (never overwrites the learner's attempt)

## Progress Snapshot

After 15 exercises, recurring strengths and patterns include:

- **Reliable words:** *gargouillement*, *galère*, *courroucé*, *nouer*, *fêlé*, *lueur* (concept correct, gender consistently wrong: *un* → *une lueur*)
- **Persistent errors:** reflexive pronoun agreement (*je pouvais s'en sortir* → *je pourrais m'en sortir*), feminine noun gender (*le forêt* → *la forêt*), infinitive used where conjugated form needed
- **Untouched vocabulary:** ~150+ words from the list have never appeared in any exercise — prime targets for upcoming sessions
