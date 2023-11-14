# MPIDR LaTeX Beamer-template-21

LaTeX Beamer template based upon the 2021 Powerpoint templates of the Max-Planck-Institute for demographic research.

Feel free to open issues or propose changes.

The most up-to-date version will (probably) be on GitHub: https://github.com/tomthe/mpidr-beamer-template-21

## Try it on Overleaf

Viewing only:

https://www.overleaf.com/read/rtnzcychznbd

Editing the template:

https://www.overleaf.com/2115745887cygrppdbnbzf

# The `stork` color theme
The stork color theme is a `beamer` color theme based on the corporate design of 
the MPIDR (see the 2021 Powerpoint template). Using this color theme allows you
to pick your preferred `beamer` (outer) theme (i.e. the general layout of your 
slides) and have titles, sidebars, list items etc. use MPIDR colors.

## How to use the color theme
Add the file `beamercolorthemestork.sty` to the directory of your `beamer` 
presentation or to the directory where your other `beamer` themes live.

Add `\usecolortheme{stork}` to your preamble to activate it.

## Does it matter where in the preamble I load the color theme?
In `beamer`, changes to themes are cumulative. This means that themes that are
loaded later in the preamble add to or override themes loaded earlier. If you
would like to change a specific element of your presentation to a specific
color, you can load another color theme in which that that color is defined
first and load the `stork` color theme afterwards. Or you can define the color
and the element in the `sty` file. Look through some of the color themes that
come with `beamer` to get an idea of which elements can be changed. 

## How did you pick the colors?
This color theme uses the colors from the Powerpoint template (2021).
 
We do not give any guarantees that all colors defined by all themes are covered
in this themes or that they work together harmoniously. We defined the major
colors (`structure`, `palette {primary,secondary,tertiary,quaternary}`, 
`sidebar`, `palette sidebar {primary,secondary,tertiary,quaternary}`, `alerted
text`) but there are many more specific ones and we only did some cursory checks
against the default theme, one theme with a footer (Boadilla), one theme with a
sidebar (Bergen), and one theme with a sidebar talk outline (Berkeley).

## Why `stork`?
Till Landau named his color themes after flying animals. We follow his example. 
The symbol of the Max Planck Society is the owl, but we wanted something more 
specific to our institute. Our first idea was "seagull" but sadly that was 
already taken. Then we thought about demography's themes: mortality, fertility, 
and migration. Mortality seemed a bit morbid. Everyone knows that babies are 
delivered by storks. Job done. There is also the 
[Rostocker Pfeilstorch](https://en.wikipedia.org/wiki/Pfeilstorch) which 
provides a nice link between fertility, migration, and Rostock.

# Can I get a nice logo in my beamer presentation?
If you're lucky, adding this line to the preamble adds a logo:
`\logo{\includegraphics[<options>]{<path_to_the_logo_file>}}`

Not all themes define a place for the logo. The logo placement is defined in the 
outer theme. If the logo does not show up, use a different (outer) theme. 		

See section 8.2.5 of the `beamer` user guide (p. 72) for more information.
