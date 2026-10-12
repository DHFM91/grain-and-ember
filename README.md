# Grain & Ember

A falling-sand sandbox in the tradition of *Falling Sand* and *Noita*. Paint elements onto a black screen and watch them interact.

**Play:** https://dhfm91.github.io/grain-and-ember/

## Elements

| Element | Density | Behaviour |
|---|---|---|
| Earth | fixed | Stays where painted. Flowing water erodes it into mud. |
| Sand | 16 | Falls and piles. Sinks through water and oil. |
| Mud | 16 | Eroded earth. Falls like sand, dries back into earth when away from water. |
| Water | 10 | Falls and levels out. Puts out fire. Erodes earth while flowing. |
| Oil | 8 | Floats on water. Burns. |
| Fire | — | Burns where painted, spreads through oil, burns out into smoke. |
| Smoke | 0.4 | Rises, fades, despawns. |

Open **Rules** in the game for the full interaction list.

## Controls

- **1–6**: Earth, Sand, Water, Oil, Fire, Erase
- **Drag**: paint (the brush replaces whatever is underneath)
- **Space**: pause · **C**: clear · **R**: rules

Single `index.html`, plain JavaScript and Canvas, no build step.
