# The AEC Verge

**AI-empowered crafts on the verge of AEC.**

AECVerge builds open-source AI tooling for the architecture, engineering, and
construction industry. We are on the frontier where structured building data
meets agentic intelligence.

## Projects

### pygments-step

[Repository](https://github.com/AECVerge/pygments-step) | 
[Docs](https://AECVerge.github.io/pygments-step) | 
[PyPI](https://pypi.org/project/pygments-step)

**Pygments lexers for EXPRESS (ISO 10303-11) and STEP Part 21 (ISO 10303-21).**

Syntax highlighting for the two ISO languages behind BIM and STEP exchange
files — schema-agnostic, dependency-light, and installed in one line. Works out
of the box with MkDocs, Sphinx, `pygmentize` and any other Pygments-backed
renderer, so `express` and `step21` code fences read cleanly whether the reader
is a human or an agent.

### mmap-cursor

[Repository](https://github.com/AECVerge/mmap-cursor) | 
[Docs](https://docs.rs/mmap-cursor) | 
[crates.io](https://crates.io/crates/mmap-cursor)

**A zero-copy byte-position reader for parsers and lexers of large files.**

Byte positions, zero-copy slices and `(line, column)` lookups over a read-only
memory map — format-agnostic, dependency-light, and no copy of the file. Pairs
with any hand-written lexer or parser, so an EXPRESS schema or a STEP Part 21
exchange file is walked by byte position rather than loaded into a buffer;
positions outlive the snapshot, so a diagnostic still renders after the file
itself has been let go.

## Philosophy

- **Open-source first.** The industry runs on shared standards; the tools
  should be shared too.
- **AI-native, not AI-wrapped.** Every tool is designed from the ground up
  for agentic workflows, not retrofitted with an API.
- **Speed matters.** Gigabyte-scale project files demand zero-copy parsing and
  sub-millisecond rule evaluation. We borrow from the best in developer
  tooling to make BIM tooling feel fast.
