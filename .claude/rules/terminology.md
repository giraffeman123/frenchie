# Vocabulary Parsing Rule

## File Structure
The file `vocabulary.txt` follows a specific key-value format:
- Individual entries are separated by a pipe `|`.
- Each entry follows the pattern: `word - definition`.

## Required Action
1. **Fetch**: At the start of any task involving text generation or naming, use the `Read` tool on `vocabulary.txt`.
2. **Parse**: Treat the content as a dictionary where:
   - Key: The string before the hyphen (`-`).
   - Value: The definition after the hyphen.
3. **Apply**: 
   - Use the exact "word" from the file when describing the corresponding "definition".
   - If the user uses a synonym, correct it to match the vocabulary in the file.

## Reference
@vocabulary.txt
