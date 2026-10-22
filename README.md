# Methalox full-flow staged combustion, anatomy jig

A 34-second, 1,020-frame schematic of a methane / liquid-oxygen full-flow staged combustion engine. The clock is the frame index. The jacket stays dark metal. Cyan, oxygen-white, and mach blue are diagram colors, not measured spectra.

Open `index.html`. Space plays and pauses. Keys 1 through 5 jump to frames 0, 150, 300, 510, and 750. Comma and period step one frame.

`index.html` and `README.md` keep the names GitHub Pages and GitHub expect. The brief locks the stage colors, so this film does not carry a theme picker.

## What the film shows

| Frames | Time | What changes |
| --- | --- | --- |
| 0-149 | 0.0-5.0s | Low pass up the bell. Jacket section opens. Feeds and gimbal actuators travel out. |
| 150-299 | 5.0-10.0s | Split view of the fuel-rich and oxygen-rich preburners. |
| 300-509 | 10.0-17.0s | Fuel turbine, then both shafts, then the oxidizer turbine. |
| 510-749 | 17.0-25.0s | Schematic coaxial injector. Methane runs up the copper liner. |
| 750-1019 | 25.0-34.0s | Reverse orbit, 15 degree gimbal, ordinal heat sketch, schematic plume. |

## What it refuses to invent

- A manufacturer contour, blade count, or element count. Those are illustrative.
- 40,000 RPM and 300 bar as test data. They are storyboard callouts. The on-screen turbine smear is about 6 revolutions per second so the direction stays readable.
- An exit Mach number. The bell is diverging, so a choked chamber flow is supersonic past the throat. That is the claim.
- A CFD temperature field. The color bar is an ordinal heat-flux sketch that peaks at the throat.
- A flame spectrum. Mach blue is a code for the chamber reaction.

Review status: working explainer, not a certified engineering drawing. Check subject-specific details before treating any number as a design value.

## Run

Any static server, or open the file directly. `?frame=400` opens that frame paused. `?frame=0&play=1` plays from the start. Reduced motion does not autoplay.

No build step. No dependencies. No analytics tag. No form.

## GitHub

About: Frame-driven schematic anatomy of a methalox full-flow staged combustion engine.

Topics: `rocket-engine` `methalox` `full-flow-staged-combustion` `propulsion` `anatomy` `explainer` `visualization` `education` `motion-design` `github-pages`

Pages: the live branch is `gh-pages`.

The Medium draft lives in `medium-ffsc-anatomy-Cursor.md`.
