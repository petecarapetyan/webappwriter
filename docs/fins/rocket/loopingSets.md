# Rocket >> Looping Sets || 20


## TL;DR:

Rocket uses a pretty obvious approach to aggregating chunks of stuff to write on any given page. If you look at the files in the `_merged_includes` directories, it practically jumps out at you.

Read more only if you want someone to review the high-level view of that approach.

## Rocket Docs

The [Rocket docs for this](https://rocket.modern-web.dev/guides/presets/using-templates/) also describe much of what I explain below, perhaps more succinctly.

## What Writes on a Page?

Hey, this is 11ty! So pretty much by design, the contents of a page can come from any number of places!

But in Rocket, 2 primary conventions:

1. Write it straight into the `_includes/something-layout.njk` as HTML.
2. Follow the -layout > partials > joining blocks hierarchy - see below

## 1. Writing straight HTML instead of all that nunjucks

One of the _**best impulses you will ever have**_ is also one of the most inevitable. Then you might not do it, anyway.

In my very first day of Rocket, first there was confusion, but after that the light goes off in my brain. "Hey I don't have to do all this multilayer nunjucks template stuff! I can just write straight HTML and be done in 15 seconds!"

And so you should.

But then as you write it, you may or may not have all the same impulses that we all have to refactor, share elements, eliminate copy-pasting, etc. One at a time, nunjucks templates slip in, and pretty soon the new page looks just like the rest of Rocket nunjucks pages. 

So goes life. This is good.

## 2. What is the layout > partials > joiningBlocks hierarchy?

This outline:

- layout file
  - partials file
    - joiningBlocks file

I could put up pictures here but it is actually just easier to go into the codebase and look at the actual files in the `docs/_merged_includes` directory.

Then, look at the above outline, and you will say "Ahah! Now I see how layout files reference partials as children, which in turn reference joining blocks as children. Seems so simple." It is.

I could probably never get the nunjucks syntax correct, on my own, but I don't have to. I just copy the same syntax already used. Or mostly, I just replace different joiningBlocks files with my own.

So that's pretty easy, eh?

## Introducing data into the mix

Thankfully for me, I was able to go for weeks before I started thinking in terms of consuming or even creating structural data on my pages.

yada

---
everything below is probably gone

2. Write chunks into separate files under `includes/joiningBlocks/something/20-something.njk`. These separate files _**then get aggregated into the above!**_

The language I am using above is oversimplified and doesn't catch every use case, but it will get you through almost all typical Rocket pages.

## How to joiningBlocks get aggregated?

Leaving out the nunjucks syntax, and instead focusing on the high level

- `something-layout.njk` includes a looping chunk of nunjucks code.
- Inside that loop above loop, `partials/something.njk`
- That in turn 

## What if I need to make a small adjustment?

Glad you asked!

Maybe this should be obvious but it wasn't to me.

If you have any kind of adjustment on 10-something.njk you have to replace the entire file!

## How does all this relate to me?