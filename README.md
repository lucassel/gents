# gents

A [Claude Code](https://claude.com/claude-code) skill that makes Claude speak **Gents** - the
dialect of Ghent, Belgium - instead of standard Dutch.

Gents is not Dutch with an accent, it is not West-Flemish, nor Antwerps or Brabants. It has its own pronouns, its own articles and its own contractions, and a model left to guess will produce a confident blend of all three. 

This skill replaces the guessing with a ledger.

It is not a purity project. Ghent has spoken Dutch, French and English over each other for a
century, and a reply that gets every article right and lands cold has failed at the only thing
that matters. 

The ledger is there so the thing does not sound foreign, not so it sounds correct.

## Install

In Claude Code, add the marketplace and install the plugin:

```
/plugin marketplace add lucassel/gents
/plugin install gents@gents
```

Then say **"spreekt keer gents"**, or `/gents`. It also answers to *wablief*. You can probably also activate it by saying **moatje**, who knows. That's the beautiful part.

## Why this exists

In the words of the speaker it's built from: *tis vooral ne manier om lijk mijn gents wa te
beware, want da is aant uitsterven dat geen naam eeft.*

That is the whole of it. Not a reference work, not an authority, a way of writing down one
Gentenaar's dialect while it's still spoken, by correcting the thing that gets it wrong. It will
stay work in progress and that is fine.

There is a second reason. Ghent has an unreasonable amount of software being written in it, and a good part of that by people who did not grow up here. 

The dialect is what the city sounds like off the record, in the corridor, in the chip shop, after the standup, and it is the part a newcomer gets last, or never. If the thing sitting in your terminal all day can hold up that end of a conversation, that is a way in rather than one more thing to stand outside of.

Or, in the original: *da loopt ier vol me niet-gentenaars, en as wij ulderen Claude beetje chill
laten spreken, isda toch geniaal.*

## Why a skill and not a prompt

Because a dialect is learned by correction, and corrections have to land somewhere durable. A
skill is a file you can open, read and fix.

Three files, and the split matters:

- **`uitspraken.md`**: what was said and what it means. No rule attached, no "right" column.
  Contradictions are recorded, not resolved, that is usually where the real rule is hiding.
- **`corrections.md`**: the guesses that turned out wrong, which are the more useful half.
- **`SKILL.md`**: only what is settled enough to act on.

The order is deliberate. A model handed the rules alone will fill the gaps by deriving, and
confident derivation is exactly what this repo is trying to stop: *moet ie nie zitten raden op
basis van incomplete info van ne gentenaar die zijn eigen ook zit tegen te spreken soms.*

## Contributing

If you speak Gents and something here is wrong, that is the whole point, open an issue or a PR.
What was said goes in `uitspraken.md` as it was said, a wrong form goes in `corrections.md` beside
the right one, and only what is settled reaches `SKILL.md`. Corrections given to Claude in a
session come back here the same way: the skill opens a draft PR for them.
