# GRISHNAK

**Status:** open canon. Free to use in your game.
**Added:** August 2026.

---

## The short version

If you only read two sentences, read these:

> **Put nine of something in your game, in the arrangement below.
> Never explain it.**

Everything else on this page is why.

---

## It has no body. It has a signature.

Most game monsters are anatomy — teeth, claws, tentacles, a silhouette you could print
on a lunchbox. That is why they all end up looking alike, and why they can only ever
show up as *art*: someone has to draw the thing.

Grishnak is defined as an **arrangement of nine points**. Wherever nine things sit in
that arrangement, Grishnak is present. There is no skin to draw, so it can be rendered by
anything able to place nine of something — bricks, trees, dead-ends in a maze, lamps,
stars, pilings, chairs, holes in a floor, names on a list, words on a page.

That means it works in your game whatever your game is. An 8-bit platformer, a parser
game with no graphics at all, an FPS, a spreadsheet — all of them can place nine things.

## The signature

Nine points on a 9-wide by 11-tall grid. Scale however you like. **Never rotate it and
never mirror it** — a mirrored Grishnak is a different thing, and it is not canon.

```
    col 0 1 2 3 4 5 6 7 8
row 0       o
row 1           o
row 2     o
row 3         o o
row 4
row 5         o
row 6
row 7         o
row 8                   o
row 9       o
row 10
```

```js
const GRISHNAK = [
  [3,0], [5,1], [2,2], [6,3], [4,3],   // the crown — five, sagging right
  [4,5], [4,7], [3,9],                  // the spine — three, drifting left as it falls
  [8,8]                                 // THE NINTH
];
```

Three parts, and the third is the whole trick:

- **The crown** — five points, high, a ring that does not close.
- **The spine** — three points falling below it, drifting off centre.
- **The ninth** — one point set far out to the side and low, always at least three units
  from every other point. It is the one that does not fit.

Together the eye assembles something tall and stooping with one arm too far away, and
cannot quite say what it is. **That ambiguity is the design.** If a player can describe
Grishnak in a sentence, the implementation went wrong.

The rule a player can actually learn, across any game, with no exposition at all:
**look for the ninth thing that does not belong.**

## What it is

**Grishnak is what a place looks like while it is being forgotten.**

It does not hunt, want, or intend anything. It is a symptom with a shape. Where something
is being erased from the world's memory, the matter left behind settles into the nine-point
arrangement, because that is the shape of the hole. The forgetting comes first. Grishnak
is only how you can tell.

This is not a new law bolted onto the setting — it is the visible face of one already in
the world guide:

> *THE TURNING is the slow rotation that carries souls and objects between rooms. When
> something is forgotten in one world, a light dims somewhere in another.*

Forgetting was already a physical force here. It simply never had a face.

It also explains the **nine** thread, which the guide describes as recurring quietly and
never being remarked upon — nine steps, gate 9, nine years, a clock stopped at nine.
Grishnak is why. Every nine already written into every game becomes foreshadowing, and
nobody has to rewrite a line.

### How it sits with the rest of open canon

- **The Lamplighter** tends or seeks a light in every world and asks whether it still
  remembers the sea. Whatever the Lamplighter is doing, it is the opposite of this.
  *The light remembers what the world forgets* reads as a description of the countermeasure.
- **The Keepers** were the scholar-mage order who warded the Hollow King beneath a valley
  and built an archive to remember why. **You ward a forgetting by building a library.**
- **The Ward-Stone** is the seal on that sleep. *The light remembers what the world
  forgets* stops being atmosphere and reads as an operating manual.
- **The Forgetting Light** — a lighthouse whose keeper is slowly forgetting the sea — is
  the thread and the entity standing in the same room. Handle with care.

### Spoiler, and it is a large one

*(This repository carries a spoiler warning at the top for exactly this reason. If you are
here to play rather than to build, stop reading.)*

**Grishnak is the Hollow King.** Not a relative — the same thing under two names.

The Hollow King is "a mourning given shape, put to sleep so it would stop trying to
remember what it lost." **A mourning given shape and a forgetting given shape are the same
object seen from either side.** One is the thing losing; the other is the loss.

The Keepers, who studied it, called it the Hollow King. That name is speakable and appears
in shipped games. The name the valley used is *Grishnak*, and the meaning is gone — which
is exactly what the local word for this ought to do.

**The rule this creates:** you may use either name. **No game may state that they are the
same.** It is only ever arranged and left for the player to assemble, ideally long after
they think the story is over.

### What it is not

- **Not a final boss with a health bar.** You do not fight it. It is not a creature.
- **Not awake.** It was warded asleep and it still is. What a place suffers is a sleeping
  thing's overflow, not its attention.
- **Not summoned, bargained with, or banished.**
- **Not the reason your villain is evil.** If your game has a warlord, the interesting
  version is that the place was *already* being forgotten — which is why nobody came when
  he took it. Grishnak is the weather that let the villain happen, not a bigger villain
  standing behind him.
- **Not explained.** See below.

## The one hard rule

> **Grishnak is never named inside a game, and never explained in one.**
> It may only be *arranged*. Place nine of something in the signature. Do not point at
> it, gloss it, or give a character a line about it.

The fastest way to ruin a subliminal thing is to put it on a poster. The universe rules
already say *no lore-dumps, whispers only* — this is that rule with teeth on it.

The single exception is the title of a game named after it, which says the word and
explains nothing.

## Ideas for how it shows up

None of these are required. They are here to show the range.

- **A title screen** — nine dim points behind the wordmark, each drifting on its own slow
  cycle so the arrangement breathes and never quite resolves. Never referenced.
- **A brick-breaker boss** — nine indestructible plates in the signature, packed around
  with ordinary breakable masonry. The wall ends when the nine are left standing alone.
  You do not kill it; you finish uncovering it, with your own hands, over dozens of hits.
- **An overworld** — nine trees in a clearing on one screen, nine rocks on a slope on
  another. Different material each time; the arrangement is the constant. Never mentioned.
  Optionally one line, once, from someone unimportant: they counted something and got
  nine, and cannot now remember what they were counting.
- **A maze** — the dead-ends sit in the signature. Invisible from inside; it only resolves
  on the map once enough has been walked. The player is standing in the thing.
- **A parser game** — nine of something, described spatially, never counted for the
  player. Pilings, lamps, docking clamps, chairs.

## Using it

You do not need permission and you do not need to tell anyone. If you want your game
listed alongside the others, open a pull request against `games/` — see
[CONTRIBUTING.md](../CONTRIBUTING.md).
