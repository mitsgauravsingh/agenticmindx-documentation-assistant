# AgenticMindX Documentation Assistant

A local-first documentation assistant prototype. It indexes Markdown and text files, retrieves relevant passages with a transparent keyword score, and displays source filenames so answers can be checked.

## Quick start
Requires Python 3.10 or newer.

```bash
python src/main.py --docs ./sample_docs --question "How do I add a tool?"
```

## Features
- Reads `.md` and `.txt` files from a folder.
- Splits documents into small passages.
- Uses a simple term-overlap ranking method.
- Shows source filenames and excerpts rather than inventing citations.

## Limitations
This is retrieval, not a language model. It does not generate authoritative answers and may miss semantic matches. Verify important information in the cited source files.

## Next steps
Add embeddings, a vector database, an LLM answer layer, evaluation questions, and access controls.
