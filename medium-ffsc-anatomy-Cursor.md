# Full-flow staged combustion, methalox: what the two preburners actually do

**Suggested Medium title:** Full-flow staged combustion, methalox: what the two preburners actually do

**Subtitle:** A 34-second anatomy jig, and the public cycle it is trying not to lie about.

**Tags:** rocketry, aerospace, engineering, methane, propulsion

**Meta description:** How a methalox full-flow staged combustion engine routes methane and oxygen through two preburners and two turbines before an all-gas main chamber. A reading guide to a 34-second schematic, with the numbers that are storyboard and the numbers that are not.

---

A full-flow staged combustion engine burns almost all of its fuel and almost all of its oxidizer in separate preburners, runs each stream through its own turbine, and only then injects both as gas into the main chamber. On methalox, the fuel is liquid methane and the oxidizer is liquid oxygen. The point of the split is mechanical: the fuel turbine never has to seal hot fuel-rich gas against liquid oxygen, and the oxidizer turbine never has to seal hot oxygen-rich gas against fuel.

That is the whole cycle. The rest of this piece is how to see it, what a public ground demo already established, and which numbers in the accompanying film are labels rather than measurements.

The film is a 34-second schematic, 1,020 frames at 30 frames per second:

https://mizcausevic-dev.github.io/methalox-ffsc-anatomy/

It is not a flight engine, not a manufacturing drawing, and not a Raptor model. The contour, the element count, and the blade count are illustrative. Where the picture uses 300 bar, 40,000 RPM, or 15 degrees, those are storyboard setpoints printed on the plate so they cannot be mistaken for test data.

## What "full-flow" changes

Staged combustion, in the ordinary sense, burns a fraction of the propellants in a preburner, drives a turbine with that gas, and dumps the turbine exhaust into the main chamber instead of overboard. Full-flow is the twin-shaft version of that idea. One preburner runs fuel-rich and drives the fuel turbopump. The other runs oxygen-rich and drives the oxidizer turbopump. Nearly all of the methane takes the fuel path. Nearly all of the oxygen takes the oxidizer path. A small oxidizer flow still has to reach the fuel-rich dome, and a small fuel flow still has to reach the oxygen-rich dome, or those preburners have nothing to burn.

The U.S. Integrated Powerhead Demonstration put that arrangement on a stand with liquid oxygen and liquid hydrogen, not methane. NASA's 2006 release on the 100 percent power test, and the Air Force write-up of the same July 12 run at Stennis, describe the cycle in the same words: a fuel-rich preburner drives the fuel turbopump, an oxidizer-rich preburner drives the oxygen turbopump, and because each turbine sees only its own propellant-rich gas, the pumps do not need the complex seal that keeps fuel and oxidizer from meeting on one shaft. The demonstrator was not a flown engine. The releases say so.

Methane does not change the topology. It changes the coolant, the mixture chemistry, and the materials problem on the oxygen-rich side. The jig uses methane because that is the propellant pair in the brief. It does not borrow a hydrogen engine's chamber pressure and relabel it.

## Why the seal is the point

On a single shaft that pumps both propellants, or on a turbine that ingests one propellant while the pump on the same shaft holds the other, something has to keep them apart. That something is the interpropellant seal. It is a small part with a large failure mode: mix fuel and oxidizer in the wrong cavity and you no longer have a turbopump, you have a reaction in the wrong place.

Full-flow moves the problem instead of deleting hardware in general. You now have two preburners, two turbines, and an oxygen-rich hot-gas path that has to survive its own chemistry. What you drop is the shaft that sees both. The fuel machine is fuel on both ends of the power train. The oxidizer machine is oxidizer on both ends. NASA's IPD language calls the result the elimination of a complex propellant seal and of inadvertent mixing at that seal. That is a reliability claim about a failure mode, not a claim that the engine got simpler everywhere else.

The film's middle seven seconds exist to make that split visible. The fuel turbine is one object. The oxidizer turbine is another. They are not geared together on screen, and they should not be.

## How to read the 34 seconds

The player is one HTML file. Space starts and stops it. Keys 1 through 5 jump the cuts. The cuts sit on the clock, not on a loose frame count: 5.0, 10.0, 17.0, 25.0, and 34.0 seconds.

**0.0 to 5.0 seconds. The skirt.** The camera is low and off to the side, looking up the bell. The dark metal is the jacket. The copper-colored wall inside the opened wedge is the liner. Methane and oxygen feed lines travel outward on radial axes, and so do the gimbal actuators. That move is an anatomy explode. It is not a claim about how far the flight hardware strokes during start.

**5.0 to 10.0 seconds. The preburners.** The frame splits. Left is the fuel-rich dome: mostly methane, a little oxygen, drawn in cryo cyan with a thin oxygen-white tap. Right is the oxygen-rich dome: mostly oxygen, a little methane. The dots inside the domes are a visual for vapor, not a droplet-size simulation. Each dome's job is to leave hot gas for its own turbine.

**10.0 to 17.0 seconds. The turbopumps.** The camera visits the fuel stack, pulls back until both stacks read, then visits the oxidizer stack. The plate says 40,000 RPM because the brief did. The blades on screen turn at about six revolutions per second. At 30 frames per second, a true 40,000 RPM strobe is about 22 revolutions per frame, which is a disk. A directional smear is more honest than a slowly spinning cartoon labeled as real time. Discharge is marked "300 bar class" for the same reason. 300 bar is about 296 standard atmospheres. The brief also said "over 300 atmospheres." Those are the same order of magnitude, not two measurements.

**17.0 to 25.0 seconds. The injector.** Both propellants are gas by the time they reach the face. The pattern is a schematic coaxial element: oxygen-rich core, fuel-rich annulus. Count the rings if you want. The count is not from a drawing release. Below the face, the chamber is mach blue, `#1A8CFF`. Methane-oxygen flames are not that color. The blue is a code so the chamber reaction cannot be confused with the coolant. The coolant is the cyan moving up the copper wall, from the exit manifold toward the injector. That is the regenerative circuit in one sentence: liquid methane in the liner, heat into the methane, wall kept inside its material limit. The film does not solve the heat flux.

**25.0 to 34.0 seconds. The bell and the gimbal.** The camera spirals back out. Past a throat, a choked chamber flow is supersonic in a diverging nozzle. That is gas dynamics, and it does not require an exit Mach number, so none is printed. The mount pitches to 15 degrees. A fixed dashed axis stays put. A cyan axis moves with the engine. The color bar in the corner is an ordinal sketch: cold methane in the wall, a peak at the throat, mach blue in the gas. It is not a contour plot from a solver.

## What the colors are doing

Five colors, and none of them are decoration for its own sake.

| Color | Hex | Job in the film |
| --- | --- | --- |
| Jacket | `#16181D` | Cast structural shell. Dark on purpose. |
| Liner | `#3D271D` | Copper-alloy wall in the opened section. |
| Methane | `#00E5FF` | Liquid methane and fuel-rich gas paths. |
| Oxygen | `#E0F7FA` | Liquid oxygen and oxygen-rich gas paths. |
| Chamber | `#1A8CFF` | Main-chamber reaction, as a code. |

If a later version mixes those meanings, the picture gets worse even if the rendering gets prettier. Cyan that sometimes means methane and sometimes means "hot" will teach the wrong pipe.

## What this will not pretend to know

A schematic can be accurate about topology and still be useless as a design record. This one is in that category on purpose.

It does not know a real nozzle contour, a real injector element pattern, or a real turbine blade count. It does not know wall temperature. The throat "peak" is the usual qualitative fact that chamber heat flux concentrates at the throat, drawn as a gradient so the eye has somewhere to land. It is not a British thermal unit per square inch per second.

It does not know the mixture ratio in either preburner. Published studies of methalox full-flow concepts do pick very different mixture ratios for the two domes, fuel-rich well below stoichiometric and oxygen-rich far above it, because turbine inlet temperature has to stay inside the metal. Those ratios are design choices. They are not printed here, because this film did not run that trade.

It does not claim a specific vehicle. Public writing treats SpaceX Raptor as a flown methalox engine on this cycle. Wikipedia's full-flow section is one of the places that identification shows up. Using the name as a pointer is fair. Tracing its ducts from a marketing render and calling the result a drawing is not. The jig does not do that.

## Where the cycle was demonstrated, and where methane enters

The clean primary source for the cycle logic is the IPD test campaign, oxygen and hydrogen, ground only. The NASA release on the Stennis 100 percent power test, and the Wright-Patterson Air Force version of that note, are the ones to read if you want the seal sentence in the program's own words. A NASA technical report on the Stennis facility work, "Facility Activation and Characterization for IPD Turbopump Testing," describes the same demonstrator as a 250,000-pound-thrust liquid-oxygen / liquid-hydrogen full-flow staged combustion article. Use the 2006 releases for what reached mainstage. The earlier component papers describe the path into that test, not the 100 percent result itself.

Methane full-flow is a later application of the same flow path. The teaching value of the jig is the path: two domes, two shafts, gas at the face, methane in the wall. Anyone who needs a number for a vehicle should get it from that vehicle's data, not from a 34-second player.

## How to use the page

The live player is the Pages URL above. The repository is [mizcausevic-dev/methalox-ffsc-anatomy](https://github.com/mizcausevic-dev/methalox-ffsc-anatomy). `?frame=510` opens the injector shot paused. `?frame=0&play=1` plays from the start. If the browser asks for reduced motion, the film stays parked until you press play.

There is no account, no form, and no analytics tag on the page. A form would need a purpose, a disclosure, a retention rule, and an owner. This page's job is the mechanism.

If you only have a minute, watch 5.0 to 17.0 seconds twice. The first pass is the two domes. The second is the two shafts. Everything else in the film is there so those two shots have a nozzle under them and a chamber after them.

## Sources

- NASA, "New Rocket Engine Combustion Cycle Technology Testing Reaches 100% Power Level," on the Integrated Powerhead Demonstration's 100 percent power test at Stennis. Oxygen/hydrogen, ground demonstrator. https://www.nasa.gov/news-release/new-rocket-engine-combustion-cycle-technology-testing-reaches-100-power-level/
- Wright-Patterson Air Force Base, "New Rocket Engine Combustion Cycle Technology Testing Reaches 100% Power Level," the Air Force account of the same July 12 test, including the seal sentence. https://www.wpafb.af.mil/News/Article-Display/Article/401448/new-rocket-engine-combustion-cycle-technology-testing-reaches-100-power-level/
- NASA Technical Reports Server, "Facility Activation and Characterization for IPD Turbopump Testing at NASA Stennis Space Center," record 20050041816. States the 250,000-pound-thrust LOX/LH2 full-flow description and the 2003 component tests. https://ntrs.nasa.gov/citations/20050041816
- Wikipedia, "Staged combustion cycle," full-flow section, for the twin-shaft definition and the public methalox flight example. https://en.wikipedia.org/wiki/Staged_combustion_cycle

The player itself is the primary source for what the film shows. If the plate and this article ever disagree, the plate is the picture and this article should be corrected.

---

*Draft for Medium. Byline: Miz Causevic. Status: explainer, 22 October 2026. Not a certified propulsion analysis.*
