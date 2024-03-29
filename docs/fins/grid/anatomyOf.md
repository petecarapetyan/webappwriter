# Grid Based >> Anatomy of a Theme || 50

## Based on CSS Grid

These themes are all built around CSS grid, or more specifically CSS grid areas.

I was anything but religious in my attempts to mimic the original site _accurately_. Close enough...

## 2018 New

If you're not a grid enthusiast like the infamous [Jen Simmons](https://en.wikipedia.org/wiki/Jen_Simmons), you might be surprised how many capable devs **think it's necessary to stay away from CSS Grid** because of lack of browser support.

If grid scares you, check it out on [caniuse.com](https://caniuse.com/?search=grid) but you might find support for CSS grid much stronger in 2021 than you might have suspected.

## Why Grid

Again, referring you back to real experts such as [Rachel Andrew](https://www.smashingmagazine.com/understanding-css-grid-template-areas/) or [Jen Simmons](https://labs.jensimmons.com/) would be greatly preferrable to my own opinions, but here's an analogy that I go by.

_**CSS grid is like painting by numbers, compared to previous css approaches.**_ It gives you nice little 2 dimensionally prescribed boxes, you do your work inside these little boxes, and the world stays clean and simple.

If you're unfamiliar with grid, you might find it shockingly straightforward. What used to require heroic or external CSS just kinda happens automagically. _This can be upsetting, especially if you are already accustomed to using dazzling media queries, convoluted CSS, or third party layout libraries._ I empathize.

## Grid Area Layout - Designed to be left alone

In the context of these themes, at least in terms of daily development, a theme's `_assets/grid.css` file is intended to remain relatively static.

The idea is that your basic page layout is defined here and mostly remains untouched. 

Then you improve your fork of the theme in  `_assets/theme.css`, html and njk files, or other related files.

Not that it's specifically wrong to change the  `_assets/grid.css` file, but rather that CSS gets really messy, really fast, and there is a benefit to keeping the grid layout css clean and segregated for your own ease of layout maintenance.

Grid area code is just weird enough to benefit from that extra segregation. My 2c only, not intended as fact.

## Media Queries still remain an issue

- Rocket already has media queries that have not yet been reconciled against any themes
- Even theming with grid areas requires _**some**_ amount of media queries, which haven't been done yet.

Specifics:

- `_assets/layout.css` has a number of media queries which have not yet been reconciled against either of these situations:
- media queries moved to `_assets/grid.css`
- media queries which are no longer necessary, due to migration to grid areas which often supplants media queries

Resolving these issues in code is probably pretty fast, but neither has it been started.

## Separate CSS

FIXME gotta explain which css is community, which is intended for customization, etc.