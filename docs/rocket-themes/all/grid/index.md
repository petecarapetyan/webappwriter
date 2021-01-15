# All >> Grid Based || 50

These themes are all built around CSS grid, or more specifically CSS grid areas.

## 2018 New

If you're a grid enthusiast like the infamous [Jen Simmons](https://en.wikipedia.org/wiki/Jen_Simmons) you might be surprised how many otherwise strong devs **think it's necessary to stay away from CSS Grid** because of lack of browser support.

If grid scares you, check it out on [caniuse.com](https://caniuse.com/?search=grid) but you might find support for CSS grid much stronger in 2021 than you might have suspected.

## Why Grid

Again, referring you back to real experts such as [Rachel Andrew](https://www.smashingmagazine.com/understanding-css-grid-template-areas/) or [Jen Simmons](https://labs.jensimmons.com/) would be greatly preferrable to my own opinions, but here's an analogy that I go by.

_**CSS grid is like painting by numbers, compared to previous css approaches.**_ It gives you nice little 2 dimensionally prescribed boxes, you do your work inside these little boxes, and the world stays clean.

If you're unfamiliar with grid, you might find it shockingly straightforward. What used to require heroic or external CSS just kinda happens automagically. _This can be upsetting, especially if you are already accustomed to using dazzling media queries, convoluted CSS, or third party layout libraries._ I empathize.

## Media Queries still remain an issue

- Rocket already has media queries that have not yet been reconciled against any themes
- Even theming with grid areas requires _**some**_ amount of media queries, [which haven't been done yet](/rocket-themes/all/issues/#yikes-media-waiting)

Something that has not yet been resolved is the issue of media queries.

`_assets/layout.css` has a number of media queries which have not yet been reconciled against either of these situations:

- media queries moved to `_assets/grid-area-layout.css`
- media queries which are no longer necessary, due to migration to grid areas which often supplants media queries

Resolving this issue in code is probably pretty fast but I haven't implented yet.

What is NOT resolved in my mind is whether this will fight whatever code is currently in `_assets/layout.css`

## Separate CSS

Ut sint eiusmod minim id consequat. Aliquip nisi ipsum ea officia ut commodo velit ullamco aliqua ipsum irure dolor nisi aliqua qui. Veniam exercitation laboris minim est aliqua quis enim esse sint esse elit. Duis amet sunt velit ea qui. Cillum aute nostrud eu. Enim officia culpa est esse est in quis labore. Qui dolor voluptate culpa et pariatur culpa voluptate amet eu culpa. Mollit fugiat reprehenderit sunt voluptate aute ullamco excepteur veniam eiusmod irure incididunt sunt id do.