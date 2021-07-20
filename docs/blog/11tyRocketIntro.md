---
title: 11ty Rocket Intro
published: true
date: 2021-07-17
description: Opinionated perspective on when to use Rocket, which is also 11ty
tags: [WordPress, html, javascript, website, CMS, markdown, rich text]
cover_image: https://storage.googleapis.com/betterology-com.appspot.com/images/landscape/700/rocket.jpg
---

# 11ty Rocket Intro

If you want to put something on the web and you're considering a static site generator (SSG), [11ty](https://www.11ty.dev/) comes out near the top of [this list of 330+ SSGs](https://jamstack.org/generators/).

[Rocket](https://rocket.modern-web.dev/) is 11ty, plus some artfully spare magic added by the [open-wc group](https://open-wc.org/).

## Oh, Sweet Productivity w Markdown

Falling in love with Markdown was accidental, and happened years ago when I started using `README.md` files on github.

Holy smoke! I can write good-enough articles in minutes! And except for my writing talents, not bad results. Like this one. Just start typing in a darn text editor, 5 minutes later you're done.

I also deploy straight `*.html` files, when appropriate. Rocket doesn't flinch. It's 11ty!

Pull down Rocket from npm, drop in a few markdown files, `npm start` and my site is done. _**Didn't even build any menus,**_ somehow they all just magically happened.

But that was last year. I wanted more. I wanted a site that didn't look like, well, _a Rocket site_.

## Enter, Themes

Hmmm. _**Customers are begging us to help migrate off of WordPress.**_ But I actually like the WordPress themes, mainly because otherwise my sites look like an engineer created them. Personal problem, sure. But also typical.

So, Jan 1, 2021 I set out to Proof-of-Concept [some themes for Rocket](https://webappwriter.com/fins/thumbnails/).

Here are my two takeaways from building 17 Rocket themes:

- Rocket is pretty easy to learn, and decent to write themes in
- Whoa! My CSS skills sucked worse than I thought.

How did I deploy [17 sites to demo Rocket?](https://github.com/petecarapetyan/fins-rocket-themes#running-examples-of-these-themes) Lorem Ipsum, mostly. No one will confuse me with a graphics designer. But the point is, we're talking about a very minimal investment in time - that's what Rocket offers. Get the work done easily, make the site fast.

The rest is up to you, it's just HTML - even if optionally written in Markdwon.

## Why is Rocket Easy?

You would think that a static site generator just takes clumps of HMTL/CSS/JS and loops through templates, creating pages as it goes.

You'd be right! And that is pretty nearly what you see happen before you, when you're working in Rocket. The simplicity is helpful.

There is some cool magic - my own favorites are _menuing, search, and link checking._ But the magic is pretty limited, and best most importantly, it is mostly segregated into modules.

Rocket uses nunjucks for it's templating, but guess what? Rocket is 11ty at it's core, so like any 11ty, you can use any of a dozen or so template engines, not just nunjucks.

You might care more about template engines than me. The point is, you get to choose.

## Bonus Points for MPA Features

The SPA is such a dominant structural feature in web based app design, most developers have never had an opportunity to even imagine the approach as optional. How else would you even accomplish something as fundamental as a shared auth and/or back end connection?

If you want your mind blown for a few minutes, [watch Rocket's creator, Thomas Allmer, use Rocket to replace both a React SPA and a Lit SPA](https://www.youtube.com/watch?v=JEirUtE4k84&t=1576s) with Rocket's MPA design - while coding.

Rocket makes this possible with a really clean and super simple bolt up mechanism for wiring in Javascript without a fuss.

This blog is not the place to detail such a [fundamental shift as SPA to MPA](/blog/friendsWithBenefitsIntro/). Once there, however, your brain might imagine new opportunities to speed up your user's experience with an MPA. Shopping cart? Single widget on a single page. The other 150 product pages don't even know that the cart exists, nor do they require auth/login. Hmmm.

## Opposite Approaches

Rocket's approach - spare on the magic, just straightforward standards based HTML/CSS/JS - is not for everyone.

Compare it to the stated goals of more ambitious projects such as Astro or even Svelte. If you like magic on steroids, you may want to go in that direction instead. Astro promises "use any framework you want" and then it compiles it to HTML via SSR. Svelte offers it's own improved semantics using a live server to compile HTML via SSR - at least, I think that is what it does.

Either approach is way too much magic for my tastes. Keep it simple. I want to dump legacy frameworks, not provide more magical processes to unwind already too much magic. Personal preference, no judgement intended.

If _your_ preferences still aren't fulfilled, you can look at any of [the other 330+ SSGs](https://jamstack.org/generators/) - lotta great options.

## Summary

Rocket is just enough magic on top of 11ty to make the jump worthwile and still keep it simple.

Straight HTML/CSS/JS to a universal evergreen browser standard - that's a win.

How much time should you budget to try out Rocket? Pretty much any developer that uses npm every day will probably be done in 15 minutes.
