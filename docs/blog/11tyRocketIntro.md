---
title: 11ty Rocket Intro
published: true
date: 2021-07-17
description: Opinionated perspective on when to use Rocket, which is also 11ty
tags: [WordPress, html, javascript, website, CMS, markdown, rich text]
cover_image: https://storage.googleapis.com/betterology-com.appspot.com/images/landscape/700/rocket.jpg
---

# 11ty Rocket Intro

If you want to put something on the web and you're considering a static site generator (SSG) then 11ty comes out near the top of [this list of 330+ SSGs](https://jamstack.org/generators/)

11ty what I was going to use in 2020, until the [open-wc group](https://open-wc.org/) put [Rocket](https://rocket.modern-web.dev/) together. Essentially, 11ty - plus a little magic.

## Oh, sweet productivity!

Falling in love with Markdown was accidental, and happened years ago when I started using `README.md` files on github.

Holy smoke! I can write good-enough articles in minutes! And except for my writing talents, not bad results. Like this one. Just start typing in a darn text editor, 5 minutes later you're done.

Pull down Rocket from npm, drop in a few markdown files, `npm start` and my site is done. Didn't even build any menus, somehow they all just magically happened.

But that was last year. I wanted more. I wanted a site that didn't look like, well, _a Rocket site_.

## Enter, Themes

Hmmm. _**Customers are begging us to help migrate off of WordPress.**_ But I like the WordPress themes, mainly because I'm a developer, not a web designer, and otherwise my sites look like an engineer, not a designer, created them.

So, Jan 1, 2021 I set out to build [some themes for Rocket](https://webappwriter.com/fins/thumbnails/).

Here's the two takeaways from building 17 Rocket themes:

- Rocket is pretty easy to learn, and write themes in
- Whoa! My CSS skills sucked worse than I thought.

How did I deploy 17 sites to demo Rocket? Lorem Ipsum, mostly. And they still look like an engineer built them. No one will confuse me with a graphics designer. But the point is, we're talking about a very minimal investment in time - that's what Rocket offers. Get it done, make it fast. 

Rest is up to you, it's just HTML - mostly written in Markdwon.

## Why is Rocket Easy?

You would think that a static site generator just takes clumps of HMTL/CSS/JSS and loops through templates, creating pages as it goes.

You'd be right! And that is pretty nearly what you see happen before you, when you're working in Rocket.

There are some cool magic pieces - my favorites are menuing, search, and link checking. But the magic is pretty limited, and best of all pretty segregated into it's own modules.

Rocket uses nunjucks for it's templating, but guess what? Rocket is probably 85% 11ty at it's core, so like any 11ty, you can use any of a dozen or so template engines, not just nunjucks. 

You might care more about template engines than i do. The point is, you get to choose, if you do.

## Bonus Points for MPA Features

I'm not against marriage, but neither do I believe that it should be taken lightly. So this whole thing about getting married into an SPA just to have relations with auth and a back end, yeah I've got issues with that.

If you want you're mind blown for a few moments, [watch Rocket's creator use Rocket to replace a React SPA and then Lit SPA](https://www.youtube.com/watch?v=JEirUtE4k84&t=1576s) with Rocket's MPA design while live coding.

Dude. You can't do stuff like that without a really clean and super-dumb (as in simple) bolt up mechanism for wiring in Javascript without a fuss. Go Rocket.

I got so excited, I started working on my own _**Friends With Benefits**_ Web Components that lets me take little micro-functionality modules into Rocket pages with only the PRECISE MINIMUM of Firebase Auth, or Firestore Database, or other specialized functionality ONLY TO THAT PAGE that needs it. Obnoxious allcaps intentional, sorry - this is just too much fun.

## Opposite Approaches

Rocket's approach - no magic, just straightforward standards based HTML/CSS/JS - is not for everyone.

Compare it to the stated goals of more ambitious projects such as Astro or even Svelte, in it's own way, and if you like magic you may want to go into that direction instead. Astro promises "use any framework you want" and then it compiles it to HTML via SSR. Svelte offers it's own improved semantics using a live server to compile HTML via SSR - I think.

Or look at any of [the other 330+ SSGs](https://jamstack.org/generators/) lotta great options.

For me, less magic, more writing HTML/CSS/JS to a universal evergreen browswer standard - that's a win.

## Summary

Rocket is just enough magic on top of 11ty to make the jump worthwile and still simple.

How much time should you budget to try out Rocket? Pretty much any developer that uses npm every day will probably be done in 15 minutes.