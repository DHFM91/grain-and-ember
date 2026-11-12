# Grain & Ember

A falling-sand sandbox in the tradition of *Falling Sand* and *Noita*. Paint elements onto a black screen and watch them interact.

**Play:** https://dhfm91.github.io/grain-and-ember/

## Elements

38 elements, every one with its own brush. They're sorted into five groups in the toolbar: **Solids, Powders, Liquids, Fire & gas, Gadgets**.

| Element | Density | Behaviour |
|---|---|---|
| Earth | fixed | Stays where painted. Flowing water erodes it into mud. |
| Wax | fixed | Stays where painted. A flame touching wax burns steadily like a wick, so a wax line works as a fuse. Fire melts it into burning drips. |
| Steel | fixed | Inert to fire, water, acid and blasts. Only burning thermite can melt it (into slag). Bounces shrapnel. |
| Ice | fixed | Slowly melts to water. Freezes water that stays touching it for ~2 s, so it spreads through pools. Fire melts it instantly. |
| Stone | fixed | Cooled lava. Acid eats it slowly; burning thermite melts it back into lava. |
| Glass | fixed | Sand fused by lava, slag, thermite or long fires. Acid can't touch it; a blast shatters it back into flying sand. |
| Wood | fixed | Catches slowly and burns as embers, leaving ash. Soaks up water; wet wood won't light until it dries. |
| Copper | fixed | Wire. Carries sparks one cell per tick and holds the charge forever: sparks bounce back from dead ends and from each other until earth, mud or water grounds them out. |
| Vine | fixed | Grows from seeds. Drinks water and grows thin tendrils upward or toward water. Dry vine burns easily. |
| Spout | fixed | Copies the first loose material, flame or spark that touches it, then keeps pouring it out. |
| Void | fixed | Deletes anything touching it except steel. A drain you can put anywhere. |
| Ember | fixed | Burning wood. Throws flames, spreads to nearby wood, crumbles into ash. Water puts it out. |
| Mercury | 22 | Heaviest of all: sinks through everything, and sand floats on it. Acid can't eat it. |
| Slag | 20 | Molten steel from thermite. Lights things, fuses sand, cools back into steel (instantly in water). |
| Sand | 16 | Falls and piles. Sinks through water and oil. |
| Gunpowder | 16 | Piles like sand. Fire, a blast, a spark or shrapnel lights it, and a pile goes off like a string of firecrackers: small pops on short random fuses, each setting off the next. A blast destroys everything but steel at its core, throws loose pixels clear, and sprays shrapnel that cuts through anything but steel and bounces off steel. |
| Mud | 16 | Eroded earth. Falls like sand, dries back into earth when away from water. Under water it slowly bubbles out marsh gas. |
| Thermite | 16 | Ordinary fire can't light it; a blast, lava or slag can. Lit, it burns white-hot even underwater and melts steel. |
| Salt | 15 | Dissolves into water, turning it into brine. Melts ice and snow. |
| Lava | 14 | Thick and slow. Lights almost everything, melts ice, fuses sand into glass. Water sets it into stone. |
| Lye | 14 | Cancels acid: the two become water and foam. Soaked ash turns into lye. |
| Seed | 14 | Sprouts into a vine on mud, or on earth with water nearby. |
| Nitro | 13 | Stable while still. Dropped more than 8 cells onto something hard, or touched by flame, spark or shrapnel, the whole pool goes off in one big blast. Dropping it into a liquid is safe. |
| Brine | 12 | Salt water. Sinks under fresh water, never freezes, melts ice. Boiled by fire it leaves salt behind. |
| Slime | 12 | Gloopy. Clings to walls and ceilings and creeps down them; grains barely move inside it. |
| Acid | 11 | Dissolves anything it touches except steel, glass and mercury, one for one: every pixel it eats uses up a pixel of acid. Never eats other acid. |
| Water | 10 | Falls and levels out. Turns to steam when it puts out fire. Erodes earth while flowing. Grounds electricity. |
| Molten wax | 9 | Thick liquid. Floats on water, sinks under oil. Hardens away from fire; water, brine, snow and ice set it instantly. |
| Oil | 8 | Floats on water. Burns. |
| Ash | 6 | Light powder left by burnt wood. Floats on water, then soaks into lye and sinks. |
| Snow | 4 | Light: piles softly and floats on liquids. Melts to water; a deep pile packs into ice. |
| Foam | 2 | Froth from acid meeting lye. Rises through liquids, heaps on top, pops after a few seconds. |
| Fire | — | Burns where painted, spreads through oil, feeds on wax, lights wood and gas, burns out into smoke. |
| Lit thermite | 16 | Burning thermite: melts steel into slag and stone or glass into lava. |
| Spark | — | Runs along copper forever until grounded by earth, mud or water. Water it grounds into gets a jolt that sets off explosives. Lights explosives, oil, wax, wood and gas. |
| Steam | 0.5 | Rises, never fades, condenses back into water and rains down. |
| Marsh gas | 0.6 | Rises and pools under ceilings. A flame sets the whole pocket burning in a quick flash. |
| Smoke | 0.4 | Rises, fades, despawns. |

The game opens on a **welcome scene**: six small trays, each set up for one thing to try (a sand timer, a jumbled mix that sorts itself by density while a slow drip keeps adding sand and water, an oil slick, each of those two with a lit wax fuse that reaches the oil after about 30 seconds, an ice seed in a pond, a burning wax candle, and a water reservoir pouring down the central tube of an earth volcano, scouring it into a canyon). They all stand inside one big, thin steel sink: whatever spills or washes out runs along its floor to a single drain in the middle and down a pipe off the screen. Sand or mud that reaches the drain piles up in the pipe and clogs it, and then the sink starts to fill. The **Welcome** button (or **W**) rebuilds it any time.

The bottom of the screen is a drain: anything that falls off it is gone. Paint earth or wax along the bottom to hold things in.

Open **Rules** in the game for the full interaction list.

## Controls

- **1–9, G, 0**: Earth, Sand, Water, Oil, Fire, Wax, Ice, Steel, Acid, Gunpowder, Erase
- Every other element: pick its group in the toolbar (Solids, Powders, Liquids, Fire & gas, Gadgets), then the element. Hover a brush to read what it does.
- **Drag**: paint (the brush replaces whatever is underneath). Fire painted on wood lights it; sparks only paint onto copper or into empty space.
- **Space**: pause · **C**: clear · **W**: welcome scene · **R**: rules
- **Speed**: 0.5x, 1x, 1.5x, 2x, 3x or 6x from the toolbar, or **[** and **]** to step down and up
- Hover over any pixel to see what it is.

Single `index.html`, plain JavaScript and Canvas, no build step.
