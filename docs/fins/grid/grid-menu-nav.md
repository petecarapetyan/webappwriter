# Grid Based >> Grid Section Menu and Sidebar || 60

**TL;DR:**

Every fins theme has a grid.css with 3 mandatory areas. Except the home page only includes the first.

1) Horizontal **section** menu.
2) Vertical **navigation** sidebar.
3) Markdown content block.

The grid layout surrounds these other blocks with any other styling

 And then there is the rest of the content, which can be any kind of HMTL content. 

## The 3 Rocket Specific Grid Areas

The content below attempts to document the three areas, but it might be easier to scan the [grid-thumbs page](/fins/grid/gridThumbs/) to get a **color coded mental picture.**

Central to any rocket theme is the interaction of these 3 _**rocket specific**_ grid areas.

Meaning _**these grid areas coordinate closely with rocket code**_, all other areas belong solely to the theme itself.

_"Area"_ here denotes those [grid-areas](/fins/grid/) within the `_assets/grid-area-layout.css`

Repeating for emphasis, your theme is entirely fresh and original. Nothing to do with rocket, specifically. _**Except**_ those 3 rocket grid areas.

## Rocket Header: \<div class="header-grid-area"\>

_Grey in the blocking view_

Separation of responsibilities:

### Rocket code in the header

Rocket specifically furnishes the following links for the header:

- Content **section** links
- Rocket managed **search** link
- Rocket managed **light/dark theme** link

You or the theme may also put whatever you wish in the header

### Theme code in the header

- The theme doesn't provide the rocket links, but it does tell the header how to display the rocket links
- Anything else that the header needs such as how to display non-rocket links

## Rocket Sidebar: \<div class="sidebar-grid-area"\>

_Salmon in the blocking view_

### Different links

In rocket, automagically provided links are split between the header and the sidebar. How this split works is not documented here.

Most of the above descriptions of the header also describe how the sidebar works in a theme.

- Rocket manages the rocket provided links in a sidebar, just as the header
- Theme manages everything else in the sidebar, just as the header.

Benny Powers has teased how a [little customization to the sidebar](https://apolloelements.dev/blog/todo-app/#the-end-result) can make a differnce in making it look nifty, but so far I've just taken the implementation straight from rocket in the themes on this site.

## Rocket Content: \<div class="content-grid-area"\>

_White in the blocking view_

The rocket implementation itself shows how you can mix your own HTML/CSS content in with the markdown content section, in very creative ways.

So far I've mostly tried to just blast through this and make sure at least the markdown copy is showing. But you can add HTML/CSS to that.

## Everything else

_Blue in the blocking view_

Anything goes in this area - go wild! Or be conservative. It's yours.

- your own html/css and even js, in
  - home.njk
  - sidebar.njk
  - theme.css
- your own content in
  - _assets/_static ...
  - _data ...

## Careful deliniation of theme vs rocket files

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
- [something footer here]

### Files specifically off limits to a theme

- `assets/style.css`
- `assets/layout.css`
- `includes/partials/*` except as noted above

## The Nuclear Option

This:

_Copypasting in `_assets/style.css` and `_assets/layout.css` can be like "You break it, you buy it"_

You, as a consumer, can always take the nuclear option, even if the theme author should never resort to this. [Per section above.]

Since your theme is always a fork anyway, you can simply fork anything that is normally off-limits to theme developers, such as `_assets/style.css` and `_assets/layout.css`

Why is it OK for you and not OK for a theme developer? For the same reason that you might not want to do that, yourself. As soon as you fork it, you own it, and you have to keep up with the changes on your own.

For example, if rocket improves it's search or dark mode after you fork, you won't be able to get those improvements except through line by line manual code imports. So, just know what you're getting into if you take this approach.

## What about my theme vs light/dark theme?

Yeah, some cross cutting concerns there. Speaking for myself only here's what I wouldn't want in any theme I had on a site that I maintain:

- Having to _**maintain my own light/dark theming**_ just because I have my own theme
- Having to _**give up on a light/dark theming**_ just because I have my own theme
- Having to  _**wrangle with difficult light/dark theme interaction**_ just because I have my own theme

At the time of this writing it still wasn't worked out how a theme and the light/dark theme integrate with each other.

## Subjugation to Rocket

If any terminology on this page is perceived as an expression of taking charge of, or making decisions for, rocket - then that is an error and strictly my fault.

In every instance with no exception these themes exist in subjugation to the rocket codebase, and it's maintainers. Rocket leads, themes follow. End of story.
