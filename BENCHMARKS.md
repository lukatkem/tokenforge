# Tokenizer compression benchmarks

Measured on the embedded demo corpus (deterministic, reproducible):

| vocab | bytes → tokens | bytes/token |
|---|---|---|
| 300 | 555 → 285 | 1.95 |
| 400 | 555 → 195 | 2.85 |
| 512 | 555 → 195 | 2.85 |

The plateau between 400 and 512 is the corpus exhausting distinct merges — documented behavior.
