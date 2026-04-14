# Project Context: French Language Coaching

## Primary Agent
- **Agent Name:** `frenchie`
- **Usage:** Always invoke the `frenchie` agent for coaching, feedback, and exercise generation.

## Core Resources
- **Vocabulary:** `./vocabulary.txt` (Structure: `{word - definition | ...}`)
- **Exercises:** All writing tasks and feedback are stored in `./exercises/`.
- **Rules:** Logic for parsing vocabulary is in `.claude/rules/terminology.md`.

## Project-Specific Instructions
1. **Context Initialization:** Before starting, `frenchie` must read `vocabulary.txt` to sync target words and scan the `./exercises/` folder to understand the user's recent progress and recurring errors.
2. **Exercise Management:** 
   - When generating a new "High-Structure Creative Writing" prompt, save it as a new file in `./exercises/` using a descriptive name (e.g., `exercises/prompt_la_nostalgie.txt`).
   - When providing feedback, read the user's latest file in `./exercises/` and save the corrected version in the same file. Don't overwrite anything inside, just append the corrected version in a new paragraph, add a title to it such as "frenchie corrected version".
3. **Vocabulary Enforcement:** 
   - Prioritize words from `vocabulary.txt` in the "12-Element Grid".
   - Cross-reference writing in `/exercises` against `vocabulary.txt` to ensure target terms are being used correctly.

## Reference
@vocabulary.txt
@exercises/
