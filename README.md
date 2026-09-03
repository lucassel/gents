# gents

A [Claude Code](https://claude.com/claude-code) skill that makes Claude speak **Gents** — the
dialect of Ghent, Belgium — instead of standard Dutch.

Gents is not Dutch with an accent, and it is not West-Flemish. It has its own pronouns, its own
articles and its own contractions, and a model left to guess will produce a confident blend of
all three. This skill replaces the guessing with a ledger.

It is not a purity project. Ghent has spoken Dutch, French and English over each other for a
century, and a reply that gets every article right and lands cold has failed at the only thing
that matters. The ledger is there so the thing does not sound foreign — not so it sounds correct.

## Why this exists

One speaker's reason, in his own words: *tis vooral ne manier om lijk mijn gents wa te beware,
want da is aant uitsterven dat geen naam eeft.*

That is the whole of it. Not a reference work, not an authority — a way of writing down one
person's dialect while there is still someone to correct it. It will stay work in progress and
that is fine.

## Why a skill and not a prompt

Because a dialect is learned by correction, and corrections have to land somewhere durable. A
skill is a file you can open, read and fix. Every form in `SKILL.md` was corrected by a native
speaker; `corrections.md` keeps the raw log, including the questions still open — and the
guesses that turned out wrong, which are the more useful half.

## Install

In Claude Code, add the marketplace and install it:

```
/plugin marketplace add lucassel/gents
/plugin install gents@gents
```

Or drop it in by hand, which works the same and updates never:

```bash
git clone https://github.com/lucassel/gents ~/.claude/skills/gents
```

Then say **"spreekt keer gents"**, or `/gents`. It also answers to *wablief*.

## Contributing

If you speak Gents and something here is wrong, that is the whole point — open an issue or a PR.
Add the correction to `corrections.md` with the wrong form beside it, and fold the rule into
`SKILL.md`. A correction that does not reach the rule changes nothing.

Ghent has an unreasonable amount of software being written in it. It may as well be written by
something that can hold a conversation in the local language.
