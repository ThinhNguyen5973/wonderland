# WONDERLAND


**Play:** [Wonderland](https://thinhnguyen5973.github.io/wonderland/)

Desktop browser recommended. Sound on.

A garden-world, with the soil runs Conway's *Game of
Life*; six biomes each bend its rules. Creatures are dreamed live, part
by part, by three small neural networks trained on John Tenniel's
original 1865 Alice illustrations, dreamed by an early
machine. They are born, eat, grow, pair, strike, and die into terrain:
the past stays visible on the map and can never be revisited. You are
the gardener. You hold four tools and one pen. Sign the creature you
want to keep — a signed death becomes a page in the Book of the Dead,
and the Book is the only thing that persists between worlds.

## The design system

The piece was built by writing eight laws first, then refusing to break them:

1. **Scale changes what a thing means.** The same creature is prey when small and weather when huge. Small deaths become flowers; huge deaths become named mountains.
2. **The gardener obeys the garden.** Seeds wait for living soil, hands hold one thing, and the world does not pause while you draw.
3. **Only what is marked remembers.** Unmarked deaths leave terrain. Marked deaths leave a page.
4. **The place acts.** One automaton, six dialects: the Tea Garden freezes time, the Croquet Ground decrees order, the Pool of Tears shrinks, the Wood overgrows.
5. **The garden makes more than play.** Every season ends in a paper — a downloadable PNG of the census and the book, closing with a page about the gardener: you.
6. **Time moves one way.** No pause exists. No undo exists. Refreshing the page begins a new world; the Book survives alone.
7. **Creatures are made of their worlds, not their files.** Parts are dreamed from the place of birth; behavior is environment, not stats; the specimen card collects everything and comprehends nothing.
8. **The constraint dreams.** Every body comes from a small early model, at 64 pixels, and nothing is corrected.

## How to play

| Input | Action |
|---|---|
| **[1]** hold left mouse | pour water — water brings dead soil to life |
| **[2]** click living soil | plant a patch of seeds; the garden decides what sprouts |
| **[3]** click a creature | draw your sigil in red ink, freehand, while the world keeps running |
| **[4]** click | carry one small creature or egg; click again to set it down |
| right-click | kneel — inspect one cell of ground |
| **[A]** / **[B]** / **[H]** / **[L]** / **[K]** | atlas view / the Book / the Chronicle / the Lab / every key |
| **[M]** | sound on / off |
| **[P]** | press the paper — export the season as a PNG poster |

Food is Alice's objects: mushrooms cause molts, eat-me cakes grow,
drink-me bottles shrink (taken while small, they vanish), tea restores.
Creatures have twelve natures — wanderlust, lovers who pair and lay
eggs, aggressors who sometimes fall in their own charge, phoenixes who
leave an egg behind, cheshires who vanish and are elsewhere.

## The dream engine

At boot the game probes `model/heads`, `model/bodies`, `model/limbs`
and reports `ENGINE n/3 DREAMED`. Every part type that loads is dreamed
live from the network; every type that fails is **photocopied** —
procedural ink parts drawn from seeds, the oldest collage machine. The
game runs either way fully.

All sound is synthesized live — wind that breathes, birds by day,
crickets by night, rain when showers pass, a trickling pour, hatches
that chord by head-count, a soft knell for every death. No audio files
exist in this repository.

