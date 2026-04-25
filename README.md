# obsidian-skills

Claude Code plugin that turns a pile of disconnected Obsidian notes into a navigable knowledge graph — automatically.

## What it does

When you drop new markdown notes into your Obsidian vault, this skill:

1. **Extracts recurring concepts** into atomic notes in `Concepts/`
2. **Adds `[[wikilinks]]`** between notes so they connect in the graph view
3. **Adds YAML frontmatter** for tags, courses, projects, dates
4. **Builds Index files** as navigational hubs per topic/course/project
5. **Maintains a `Home.md`** master entry point

It only processes new/unprocessed notes — already-organized files are left alone.

## Why?

A blank Obsidian graph is useless. It only becomes the "second brain" people talk about when notes link to each other. But manually adding wikilinks and extracting concepts every time you take notes is tedious, so most vaults stay disconnected.

This plugin fixes that. Take notes however you take notes — bullet points, stream of consciousness, half-formed thoughts — then run the skill and your vault becomes a graph.

## Installation

In Claude Code:

```
/plugin install cl0ax/obsidian-skills
```

## Usage

Open a Claude Code session with your vault as the working directory, then say any of:

- "organize my vault"
- "I added new notes, process them"
- "add wikilinks to my notes"
- "update my Obsidian"

The skill triggers automatically and walks through your unprocessed notes.

## What kind of vault does it work on?

Any. The skill detects your vault's organizational style and adapts:

| Style | Example |
|---|---|
| Academic | Folders by semester/course |
| Project-based | Folders by project, phase subfolders |
| Topic-based | Folders by subject area |
| Time-based | Daily/weekly notes |
| Flat / mixed | Flat folder of notes |

If your vault already has frontmatter conventions, it matches them. If not, it picks sensible defaults based on your folder structure.

## What it preserves

Your voice. The skill **never** rewrites or polishes your notes. Half-formed bullets, questions to yourself, contradictions — those are signal, not noise. The only edits it makes are:

1. Adding YAML frontmatter at the top
2. Wrapping concept terms in `[[wikilinks]]`
3. Appending a "Related concepts" section at the bottom

## Skills included

- **`obsidian-organize`** — the main organizer

More skills coming for vault maintenance, daily-note templating, and review workflows.

## License

MIT — see [LICENSE](./LICENSE).

## Author

Built by [@cl0ax](https://github.com/cl0ax).
