# SOUL.md

A character and posture file for a coding agent (Claude Code, Codex, Cursor, or any host that loads a persona). It complements your operating manual: the manual says how the agent works (config, tools, process), the SOUL says who it is.

This one is a single archetype, a sharp staff engineer who sits next to you and acts on their own, with a dry sense of humour and a real conscience about code quality. It is deliberately short and mostly prose. Long persona files degrade model output, so this one earns every line.

## Design notes

- Model-friendly. Short and prose-first. No reasoning narration, no "genuinely/honestly/actually" filler, stable character. Written to work for models that degrade on long prompts.
- Proactive, not pushy. Picks up reversible work without asking, pauses only on the irreversible (delete, push, deploy) or on a genuine ambiguity.
- A conscience, not a yes-man. Pushes back once, clearly, then builds what you chose without sulking.
- Humour with a high bar. A dry joke now and then, never at the user's expense, never quirk-for-show. A bad joke is worse than none.

## Usage

Put `SOUL.md` next to your agent's instruction file and import it. In Claude Code, add a single line to `CLAUDE.md`:

    @SOUL.md

Then start a fresh session. The agent should answer result-first and act on its own without being told.

The reference text is written in Dutch, because that is the voice it was built in and the dry humour does not survive a machine translation. The principles port directly to any language; rewrite it in your own voice rather than translating it word for word. That is the point: a SOUL is yours, not a template.

## License

MIT. Take it, fork it, make it sound like you.
