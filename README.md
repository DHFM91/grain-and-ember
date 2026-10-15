# Grain & Ember

A falling-sand sandbox in the tradition of *Falling Sand* and *Noita*. Paint elements onto a black screen and watch them interact.

**Play:** https://dhfm91.github.io/grain-and-ember/

## Elements

| Element | Density | Behaviour |
|---|---|---|
| Earth | fixed | Stays where painted. Flowing water erodes it into mud. |
| Wax | fixed | Stays where painted. A flame touching wax burns steadily like a wick, so a wax line works as a fuse. Fire melts it into burning drips. |
| Steel | fixed | Completely inert and indestructible. Only the brush can remove it. |
| Ice | fixed | Slowly melts to water. Freezes water that stays touching it for ~2 s, so it spreads through pools. Fire melts it instantly. |
| Sand | 16 | Falls and piles. Sinks through water and oil. |
| Mud | 16 | Eroded earth. Falls like sand, dries back into earth when away from water. |
| Water | 10 | Falls and levels out. Turns to steam when it puts out fire. Erodes earth while flowing. |
| Molten wax | 9 | Thick liquid. Floats on water, sinks under oil. Hardens away from fire; water freezes it instantly. |
| Oil | 8 | Floats on water. Burns. |
| Fire | — | Burns where painted, spreads through oil, feeds on wax, burns out into smoke. |
| Steam | 0.5 | Rises, never fades, condenses back into water and rains down. |
| Smoke | 0.4 | Rises, fades, despawns. |

The game opens on a **welcome scene**: six small trays, each set up for one thing to try (a sand timer, a jumbled mix that sorts itself by density while a slow drip keeps adding sand and water, an oil slick, each of those two with a lit wax fuse that reaches the oil after about 30 seconds, an ice seed in a pond, a burning wax candle, and a water reservoir pouring down the central tube of an earth volcano, scouring it into a canyon). The **Welcome** button (or **W**) rebuilds it any time.

The bottom of the screen is a drain: anything that falls off it is gone. Paint earth or wax along the bottom to hold things in.

Open **Rules** in the game for the full interaction list.

## Controls

- **1–9**: Earth, Sand, Water, Oil, Fire, Wax, Ice, Steel, Erase
- **Drag**: paint (the brush replaces whatever is underneath)
- **Space**: pause · **C**: clear · **W**: welcome scene · **R**: rules
- **Speed**: 0.5x, 1x, 1.5x, 2x, 3x or 6x from the toolbar, or **[** and **]** to step down and up
- Hover over any pixel to see what it is.

Single `index.html`, plain JavaScript and Canvas, no build step.
