# Installation >> The Parts

**TL;DR:**<br>The information on this page is not helpful unless you have decided to personalize/customize a theme in production.

## Why Think In Parts?

You might do yourself a disservice by thinking of a theme installation as a single thing. It very definitely IS, or can be, a single process.

But what gets installed is multiple sets of files, and seeing those sets distinctly can save you some amount of heartache later, even though they are all jumbled up in the same install directories.

In reverse order of layering:

- seed content (optional)
- theme specific code
- fins-community code
- rocket provided code

The achilles heel of SSGs may very well be that all these types of files become aggregated at deploy time in a manner that the SSG author imagines as understood and transparent to the consumer of the SSG.

This assumption was questionable in the CMS world (think WordPress), and it is questionable in the SSG world. Consumers of an SSG just do not have that kind of contextual information loaded into their brain, so expecting someone to simply know how to make adjustments in the files in a way that follows their best interests? That expectation is not realistic.

By taking just a little bit of care to load up that contextual information, you can save yourself some heartache. An illustration follows:

## Example - Future Update Goes Well

Susan Developerish deploys and then slightly modifies the `not-ibm` theme for her new site. Her entire team is delighted with the new web presence, and team members begin adding content immediately, in a surge of creativity and excitement.

Then Billy Designerish contributes an elegant graphic design update to the `not-ibm` theme. Meanwhile Thomas Allmer contributes some improvements to Rocket, and Pete Carapetyan integrates Thomas's contribution and some miscellaneous improvements to Fins community code.

Susan Developerish does a new git branch, loads up all the latest changes using the standard script, and quickly determines which of her own changes need to override the incoming. Half hour later, she has deployed all of the external changes, and then one or two of her own, and presto-changeo she has a great new deployment!

It wasn't immediate, there were still some style sheet fixes she needed to make in a couple of places, but all in all it worked as well as possible.

Imagine how good it felt for the entire team to see their site suddenly improve dramatically, as the elegant graphics improvements from Billy Designerish suddenly appeared on Susan's site!

## Same Example - Gone Sour

In this scenario, imagine all of the above, except instead of a relatively painless process, it was actually kind of painful for Susan. Not only this one time, but in future updates, as well.

What happened to make things painful for Susan?

The important thing here is that Susan didn't do anything "wrong," but instead just didn't have the full context loaded in her brain about how the layering of files worked.

So instead of installing her changes in the theme.css file, she put her changes in the layout.css which maintained at the fins community level. And that, in turn, is reconciled against Rocket changes by Thomas Allmer or someone else.

So now Susan has to go through every incoming change at the `layout.css` file, and perhaps even the affected `.njk` files, because that's where her one or two changes are also made. And well, those files can get pretty hairy to reconcile, because subsequent files overwrite them when it all gets layered in. Confusing!

## Not All Doom and Gloom

You're going to know almost instantly when things are right - that's the beauty of an SSG. So Susan's problems in the second scenario above are not horrible, just more difficult than necessary.

- She can still get her work done, it just might take more time
- Or, she doesn't have to grab incoming updates at all!

But we all feel a little bit protective of Susan, so we want her experience with the `not-ibm` theme to be as positive as possible.

Better yet, the fast feedback of testing a site is so visual and straightforward, that even if Susan does everything the hard way, she can still slog through it and make it all work perfectly before deploying to the CDN/server.

## Defining The Parts

Again from above, in reverse order of layering:

- content
- theme specific code
- fins-community code
- rocket provided code



### Content

Content is defined in the docs folder as anything under any folder that doesn't start with an underscore.

### Theme specific code

Ew boy, manual check required, here. Theme specific code is anything in these three folders that originate from these three folders from 

fins-rocket-themes/[my-theme]/src/docs/_assets
fins-rocket-themes/[my-theme]/src/docs/_data
fins-rocket-themes/[my-theme]/src/docs/_includes

As tedious as it is to have to check these folders to know which ones you want to be adjusting first, it can save you some time on incoming updates, later.

It is especially helpful to prefer style.css and theme.css, and avoid themes.css, layout.css and markdown.css at all costs. This is the order in which css files are layered in:

variables.css [yours]
layout.css [fins-community]
markdown.css [fins-community]
grid.css [fins-theme]
themes.css [fins-community]
theme.css [fins-theme]
style.css [yours]

## fins-community code

These folders are:


- rocket provided code