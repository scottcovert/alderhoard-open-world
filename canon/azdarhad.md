# AZDARHAD

**Status:** open canon. Free to use in your game.
**Added:** August 2026.

---

> **Renamed 2026-09-10.** This page went up in August 2026 as GRISHNAK and the
> canon on it has not changed by a word — same nine points, same rule, same
> being. Only the name is different, and it is different for a dull reason: the
> old one sat one letter away from a Tolkien orc and the game it came out of had
> already been renamed off it. If you built against the old page, nothing you
> built is wrong. `canon/grishnak.md` still resolves and points here.


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

Azdarhad is defined as an **arrangement of nine points**. Wherever nine things sit in
that arrangement, Azdarhad is present. There is no skin to draw, so it can be rendered by
anything able to place nine of something — bricks, trees, dead-ends in a maze, lamps,
stars, pilings, chairs, holes in a floor, names on a list, words on a page.

That means it works in your game whatever your game is. An 8-bit platformer, a parser
game with no graphics at all, an FPS, a spreadsheet — all of them can place nine things.

## The signature

Nine points on a 9-wide by 11-tall grid. Scale however you like. **Never rotate it and
never mirror it** — a mirrored Azdarhad is a different thing, and it is not canon.

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
const AZDARHAD = [
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
Azdarhad in a sentence, the implementation went wrong.

The rule a player can actually learn, across any game, with no exposition at all:
**look for the ninth thing that does not belong.**

## What it is

**Azdarhad is what a place looks like while it is being forgotten.**

It does not hunt, want, or intend anything. It is a symptom with a shape. Where something
is being erased from the world's memory, the matter left behind settles into the nine-point
arrangement, because that is the shape of the hole. The forgetting comes first. Azdarhad
is only how you can tell.

This is not a new law bolted onto the setting — it is the visible face of one already in
the world guide:

> *THE TURNING is the slow rotation that carries souls and objects between rooms. When
> something is forgotten in one world, a light dims somewhere in another.*

Forgetting was already a physical force here. It simply never had a face.

It also explains the **nine** thread, which the guide describes as recurring quietly and
never being remarked upon — nine steps, gate 9, nine years, a clock stopped at nine.
Azdarhad is why. Every nine already written into every game becomes foreshadowing, and
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

**Azdarhad is the Hollow King.** Not a relative — the same thing under two names.

The Hollow King is "a mourning given shape, put to sleep so it would stop trying to
remember what it lost." **A mourning given shape and a forgetting given shape are the same
object seen from either side.** One is the thing losing; the other is the loss.

The Keepers, who studied it, called it the Hollow King. That name is speakable and appears
in shipped games. The name the valley used is *Azdarhad*, and the meaning is gone — which
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
  he took it. Azdarhad is the weather that let the villain happen, not a bigger villain
  standing behind him.
- **Not explained.** See below.

## The one hard rule

> **Azdarhad is never named inside a game, and never explained in one.**
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

## ⭐ WHERE IT SHOWS UP, AND HOW (Scott, 2026-09-10)

> *"he can show up in different visual, clue or auditory ways in space, moon,
> mars, modern times, main township areas which take place at an unspecified
> time, and even places like prehistoric australia."*

This is the part most likely to be useful to you, so it is worth being exact
about what it licenses.

**AZDARHAD is not tied to a period, a planet, or a genre.** It has no body, only
an arrangement, so there is nowhere it cannot be — anywhere able to place nine
of something can hold it. The list above is not a list of places it has been. It
is a demonstration that the question "would it fit in my game" has already been
answered YES, whatever your game is.

### The three channels

An appearance reaches the player through one of three, and the choice matters
more than the setting does:

1. **VISUAL** — the nine points are simply there, in whatever the place is made
   of. Lamps, pilings, dead ends, chairs, craters, holes in a floor, names on a
   list. The most common and the easiest to overdo.
2. **A CLUE** — the arrangement is in a record rather than in the room. A
   survey, a seating plan, a shipping manifest, a scoreboard, nine entries in a
   log with the last one out of place. The player finds it the way a person
   finds things: by reading something boring.
3. **AUDITORY** — nine of something heard and never seen. Nine drips, nine
   clicks of a relay, nine notes with the last one flat and far away. ⚠ The
   ninth point is *always at least three units from every other* — in sound
   that means the ninth event comes late, or from the wrong direction, or at the
   wrong pitch. **A sound version that puts the ninth beat on time is not the
   signature; it is a rhythm.**

Mix channels across a game and never within one appearance. Two channels at once
is a nudge, and a nudge is a kind of explaining.

### Surfaces, and what each one is good for

| Where | What it gives you that the others do not |
|---|---|
| **Deep space** | Nothing to anchor scale against, so the arrangement is the only structure in frame. |
| **The Moon** | Instruments. Somebody was measuring, and the last reading is still on the panel. |
| **Mars** | A habitat and a horizon: the first place with people who arrived, built, and might still be there. |
| **Modern times** | Records, cameras, and paperwork — the channel-2 setting. Bureaucracy makes the best clue. |
| **The township, undated** | Nobody can date it, so nobody can say the arrangement is old *or* new. That ambiguity is free here and expensive everywhere else. |
| **Prehistory** | ⭐ The only surface where somebody CARVED it. Everywhere else the nine points happen to be there; here a hand put them. See below. |

### ⭐ The oldest surface is the coldest one

Every other place has a witness who could have written it down. Prehistory has
none, and that is exactly why it is the strongest: **a glyph is a message with
no author left to ask.** The entity's law is that it is never explained, and
here there is nobody who *could* explain it — in the fiction or out of it. The
silence stops being a design choice you have to defend and becomes the setting.

It is also the only surface where the nine points were *placed* rather than
found, which is a different and colder fact.

⚠ **And it is the surface most likely to break the lore law by accident.**
Nothing here is a real culture's art, and nothing here is a real mythology. The
rock, the ochre, the megafauna and the size of the sky are the setting; what is
carved into it is invented and belongs to the entity alone.


## Using it

You do not need permission and you do not need to tell anyone. If you want your game
listed alongside the others, open a pull request against `games/` — see
[CONTRIBUTING.md](../CONTRIBUTING.md).
