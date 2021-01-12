# All >> 3 rocket areas || 20

## The 3 Rocket Specific Grid Areas

The fundamental idea behind all of these themes is the 3 _**rocket specific**_ grid areas.

Meaning _**these grid areas are reserved for rocket**_ all other areas belong to the theme,

The word "area" is used because it corresponds to those 3 grid-areas within the `_assets/grid-area-layout.css`

Thus, your theme is entirely fresh and original. Nothing to do with rocket. _**Except**_ the 3 rocket grid areas.

- Rocket header area - or _'header-grid-area'_ in css class lingo.
- Rocket sidebar area - or _'sidebar-grid-area'_ in css class lingo.
- Rocket content area - or _'content-grid-area'_ in css class lingo

So the name of the game with all themes here is to be totally creative, _**excepting that portion of the work which is handled by the three areas,**_ which you are still creative with, but in a more constrained manner, because each area is also rocket code that you are interacting with.

## Rocket Header - class="header-grid-area"

_Also keyed as grey in the blocking view_

Elit sit nisi magna consequat laboris incididunt id enim. Fugiat incididunt incididunt velit. Cillum exercitation velit eiusmod culpa culpa ullamco aute.

## Rocket Sidebar - class="sidebar-grid-area"

_Also keyed as salmon in the blocking view_

Ut sint eiusmod minim id consequat. Aliquip nisi ipsum ea officia ut commodo velit ullamco aliqua ipsum irure dolor nisi aliqua qui. Veniam exercitation laboris minim est aliqua quis enim esse sint esse elit. Duis amet sunt velit ea qui. Cillum aute nostrud eu. Enim officia culpa est esse est in quis labore. Qui dolor voluptate culpa et pariatur culpa voluptate amet eu culpa. Mollit fugiat reprehenderit sunt voluptate aute ullamco excepteur veniam eiusmod irure incididunt sunt id do.

## Rocket Content - class="content-grid-area"

_Also keyed as white in the blocking view_

yada

## Everything else

_Also keyed as blue in the blocking view_

Anything goes in this area - go wild!

- your own html/css and even js, in
  - home.njk
  - sidebar.njk
  - theme.css
- your own content in
  - _assets/_static ...
  - _data ...

## Grid Area Layout - Designed to be left alone

At least in terms of daily development, the `_assets/grid-area-layout.css` file is intended to remain relatively static.

The idea is that your basic page layout is defined here and mostly remains untouched. 

Then you improve your fork of the theme in  `_assets/theme.css`, html and njk files, or other related files.

The basic idea isn't that it's specifically wrong to change the  `_assets/grid-area-layout.css` file, but rather that CSS gets really messy, really fast, and there is a benefit to keeping the grid layout css clean and segregated for your own ease of layout maintenance.

Grid area code is just weird enough to benefit from that extra segregation.

## The Nuclear Option

_You break it, you buy it_

You, as a consumer, can always take the nuclear option, even if the theme author should never resort to this. [See section below.]

Since your theme is always a fork anyway, you can simply fork anything that is normally off-limits to theme developers, such as `_assets/style.css` and `_assets/layout.css`

Why is it OK for you and not OK for a theme developer? For the same reason that you might not want to do that, yourself. As soon as you fork it, you own it, and you have to keep up with the changes on your own.

For example, if rocket improves it's search or dark mode after you fork, you won't be able to get those improvements except through line by line manual code imports. So, just know what you're getting into if you take this approach.

## Careful delination of theme vs rocket files

Everything discussed on this page assumes a very careful and agreed upon deliniation of what files are in themes, and what files are not in themes by default.

This is a [so far] a fantasy. It really hasn't happened yet.

So far, it looks like it would be like this, if it happened:

### Files OK or expected in themes

- `assets/_static/*`
- `assets/grid-area-layout.css`
- `assets/theme.css`
- `includes/home.njk`
- `includes/with-sidebar.njk`
- `includes/partials/head.njk`
- `includes/partials/header.njk` probably??

### Files specifically off limits to a theme

- `assets/style.css`
- `assets/layout.css`
- `includes/partials/*` except as noted above

## What about my theme vs light/dark theme?

Yeah, some cross cutting concerns there. Speaking for myself only here's what I wouldn't want in any theme I had on a site that I maintain:

- Having to _**maintain my own light/dark theming**_ just because I have my own theme
- Having to _**give up on a light/dark theming**_ just because I have my own theme
- Having to  _**wrangle with difficult light/dark theme interaction**_ just because I have my own theme

So we gotta negotiate that, eventually.

## Subjugation to Rocket

If any terminology on this page is perceived as an expression of taking charge, or making decisions, for rocket - then that is an error and strictly the fault of this page author.

In every instance with no exception these themes exist in subjugation to the rocket codebase, and it's maintainers.