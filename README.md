# Grain & Ember

A falling-sand sandbox in the tradition of *Falling Sand* and *Noita*. Paint elements onto a black screen and watch them interact.

**Play:** https://dhfm91.github.io/grain-and-ember/

## Elements

| Element | Density | Behaviour |
|---|---|---|
| Earth | fixed | Stays where painted. Flowing water erodes it into mud. |
| Wax | fixed | Stays where painted. Fire melts it into molten wax and burns longer for it. |
| Sand | 16 | Falls and piles. Sinks through water and oil. |
| Mud | 16 | Eroded earth. Falls like sand, dries back into earth when away from water. |
| Water | 10 | Falls and levels out. Turns to steam when it puts out fire. Erodes earth while flowing. |
| Molten wax | 9 | Thick liquid. Floats on water, sinks under oil. Hardens away from fire; water freezes it instantly. |
| Oil | 8 | Floats on water. Burns. |
| Fire | — | Burns where painted, spreads through oil, feeds on wax, burns out into smoke. |
| Steam | 0.5 | Rises, never fades, condenses back into water and rains down. |
| Smoke | 0.4 | Rises, fades, despawns. |

The bottom of the screen is a drain: anything that falls off it is gone. Paint earth or wax along the bottom to hold things in.

Open **Rules** in the game for the full interaction list.

## Controls

- **1–7**: Earth, Sand, Water, Oil, Fire, Wax, Erase
- **Drag**: paint (the brush replaces whatever is underneath)
- **Space**: pause · **C**: clear · **R**: rules
- Hover over any pixel to see what it is.

Single `index.html`, plain JavaScript and Canvas, no build step.
