> **This repository is archived as of 2026-06-01.** The playbook has moved into my personal knowledge base, where the ideas continue to evolve. A curated, web-native version will be published at [99rabbits.com/ai-context](https://www.99rabbits.com/ai-context) (coming soon). The files here are frozen at their last state — kept public for anyone who linked to them or wants to read the original snapshot.

---

# Context Composer Playbook

**What should the interface for human knowledge look like in the AI era?**

This is an open design playbook exploring a single problem: the hard part of using AI isn't the models — it's assembling the right context. You copy-paste, re-explain, search for old threads, and lose track of what the AI actually knows. The vocabulary is shifting from "prompt engineering" to "context engineering," but the user-facing tools haven't caught up.

This playbook contains the problem diagnosis, design principles, interaction patterns, and product concepts for solving it.

## Browse the playbook

**[Read the full playbook on Obsidian Publish](https://publish.obsidian.md/ai-ui/Playbook+Map)** — the best way to explore. Notes are interconnected with wiki links, and you can navigate freely between concepts.

Start with:
- **[Start Here](https://publish.obsidian.md/ai-ui/Start+Here)** — a jargon-free introduction for anyone who uses AI chat
- **[Playbook Map](https://publish.obsidian.md/ai-ui/Playbook+Map)** — the full structure: problems, principles, solutions, architecture

## What's in here

The playbook is organized as atomic, interconnected notes:

- **Problems** — why current AI tools fail at context ([context assembly is the new bottleneck](https://publish.obsidian.md/ai-ui/context-assembly-is-the-new-bottleneck), [context rot](https://publish.obsidian.md/ai-ui/context-rot), [manual context curation is hidden labor](https://publish.obsidian.md/ai-ui/manual-context-curation-is-hidden-labor))
- **Principles** — design beliefs that guide the solution ([context is curation, not search](https://publish.obsidian.md/ai-ui/context-is-curation-not-search), [memory is governance, not storage](https://publish.obsidian.md/ai-ui/memory-is-governance-not-storage))
- **Patterns** — concrete UX approaches ([Propose → Adjust → Send](https://publish.obsidian.md/ai-ui/propose-adjust-send), [Context Chips](https://publish.obsidian.md/ai-ui/context-chips), [Context Strength Slider](https://publish.obsidian.md/ai-ui/context-strength-slider))
- **Concepts** — the product vision ([Context Composer](https://publish.obsidian.md/ai-ui/context-composer), [Trusted Knowledge Layer](https://publish.obsidian.md/ai-ui/trusted-knowledge-layer), [Four-Layer Architecture](https://publish.obsidian.md/ai-ui/four-layer-architecture))

## The core idea

Most AI tools today treat context as either fully manual (copy-paste) or fully automatic (RAG, memory). A few Chrome extensions are starting to explore the middle ground, but none have nailed it yet: **human-guided context composition**.

The Context Composer is a pre-flight interface where you see, adjust, and send context before every AI interaction. The AI proposes what context might be relevant. You confirm, remove, or add items in under 5 seconds. Then the prompt sends with exactly the right context.

Think of it as the difference between dumping your entire filing cabinet on someone's desk vs. handing them a carefully assembled briefing folder.

## The gap this addresses

Research across ~30 GitHub repos, Chrome Web Store extensions (~22,400 installs), Hacker News threads, and Reddit discussions shows strong builder convergence on context management as the AI bottleneck. But everything being built clusters into three camps:

1. **Developer tools** — CLI, IDE extensions, YAML configs (for developers, not regular users)
2. **Memory engines** — store everything, retrieve later (passive, no curation)
3. **Standalone chat UIs** — requires switching interfaces (high adoption barrier)

A handful of Chrome extensions (MemoryPlugin, Context Compass, AI Context Flow) are experimenting in this direction, but none yet offer a complete visual, non-technical, pre-flight context layer that works *inside* existing AI tools. That's the gap.

## Contributing

This playbook is a living document. If you're thinking about these problems, I'd love your input.

**How to contribute:**

- **Open an issue** to share a reaction, challenge an assumption, point out something we're missing, or suggest a new angle. Issues are great for discussion.
- **Submit a pull request** if you want to propose a specific change — a new note, an edit to an existing one, a correction, or a link to relevant research.
- **Start a discussion** in Issues if you're working on something adjacent and want to compare notes.

**What's most useful right now:**
- Critiques of the problem framing — are we describing the right pain?
- Evidence from your own AI workflow — how do *you* handle context assembly?
- Pointers to tools, research, or communities we should know about
- UX feedback on the interaction patterns (Propose → Adjust → Send, Context Chips)

**Note structure:** Every note has a `type` (concept, problem, principle, pattern, question, action), a `status` (seed, growing, mature), and links to related notes. See [CLAUDE.md](CLAUDE.md) for the full conventions if you want to contribute a note.

## What's not in this repo

This repo contains the open design playbook — the problem diagnosis, principles, and interaction patterns. The project roadmap, competitive research, and source documents are kept separately. The playbook explains *why* something should exist; the product itself will be built separately.

## About

This playbook was created by someone who uses AI every day and got frustrated with the hidden labor of context assembly. It's an attempt to articulate the problem clearly and design a solution worth building.

If this resonates, the best thing you can do is [open an issue](../../issues) and tell me about your experience with AI context.

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). You're free to share and adapt the material for any purpose, including commercial, as long as you give appropriate credit and link back to this repository.
