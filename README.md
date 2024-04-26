# \[b\]exli's \[b\]log \[g\]enerator

## the goal
- create a python module I run that generates a blog-like site skeleton
- leverage vanilla gh pages + jeykll themeing

## Project structure
### `bbg/`
The actual site generator
- Copies blog folder verbatim to docs/
- Read front matter and (Maybe with some Jinja magic ✨) add footers for index pages, single pages that serve as big toc for all articles of a particular category or tag
- Adds recent articles to index.md

### `blog/`
Where content is written, and is used by `bbg` to generate the full blog

### `docs/`
The actual site that served by Pages