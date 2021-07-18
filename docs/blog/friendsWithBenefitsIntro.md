---
title: Intro - Friends W Benfits Components
published: true
date: 2021-07-19
description: Intro to the SPA vs MPA approaches
tags: [Web Components, html, javascript, website, CMS, markdown, rich text]
cover_image: https://storage.googleapis.com/betterology-com.appspot.com/images/landscape/700/jonathan-borba-Azety72JJ54-unsplash.jpg
---

# SPA/MPA and Friends With Benefits

The single page app (SPA) solves some very obvious problems with developing a cohesive app. So much so that it's pretty much the only way we can even imagine developing a site that performs like an app.

`Alert: This article uses some jarring imagery to jog the psyche. Discretion advised.`

Once I accept the fact that the car needs a gasoline engine, I can put my energies into designing the rest of the car, where all the really important stuff is, like style and features.

## The Marriage Analogy

Where the car analogy makes sense, the marriage analogy takes it to an emotional level.

I'm not against marriage, but neither do I believe that it should be taken lightly. So this whole thing about getting married into an SPA just to - er uh - have relations with auth and a back end, yeah I've got issues with that.

## The Really Big Thing

The task of developing an app has had something in common with marriage for a couple of decades. "OMG, this is a really big deal!" Marriage is a lifetime commitment. 

Building a real app - something that can perform to expectations for thousands or even millions of people on a seemingly infinite array of devices can take a large team many months or years. That's a really big deal, too.

In that context, it is appropriate to simply assume that SPA is how we're going to do things. "We've got a lot work to do, let's get after it."

## What Happens When the Math Changes

Simple math has changed dramatically, even in the last couple of years.

- Exectations about the _**speed**_ of an app or site.
- Ability to knock out simple app functionality in _**minutes, not months**_
- [SSGs] make the content side of an app/site almost a trivial effort.

Reverting to the car analogy, all of a sudden I can watch videos of electric cars obliterating gasoline powered "muscle cars" on racetracks. Dude, wasn't but a few years ago that my son and I were swapping out gas engines on his truck, in our garage. WTF? Electric?

So what happens when the Multi Page App (MPA) becomes instantaneous, and dropping in components too?

## Friends With Benefits

Returning to the marriage analogy, all of a sudden relations between FE and BE become a ho-hum thing. It's can be a distasteful thought, on the human side, when intimate relations are so taken for granted. "I think I'll sleep with Suzy tonight."

But stacks aren't humans, and they don't have emotions. It's OK when stacks relate to each other in different ways, even when the humans who code them may have emotional commitments to specific stacks.

The shift comes when FE/BE relations can be a drop in widget - and only on that one page when and where they are needed. It's like "app-shell" of the SPA now becomes lots of mini-app-shells, dispersed throughout, with many duplicate functionalities.

My shopping site, which is 97% content, now becomes even faster, and in many ways, easier to maintain. It still has a cart, but that's a drop in widget on one page.

## Tradeoffs. Ugh

Like every shift in approaches, this one comes with some serious downsides.

Now my app repo is a mono-repo, with every little mini-app-shell becoming it's own package. Ugh.

Even worse, each mini-app-shell has it's own auth and other FE/BE connectivity, so I'm duplicating so much code in multiple places. That's enough to drive me back to SPAs all by itself.

And the links. Good gawd. No common routing mechanism, so now I'm maintaining all these links between pages and packages as onesies. What a horrible design.

## Specifics

Here are my known mini-app-shells, so far:

- [Login/auth](https://github.com/petecarapetyan/page-fb-rdx-auth)
- [Shopping cart](https://github.com/petecarapetyan/page-fb-rdx-cart)
- [Media uploads](https://github.com/petecarapetyan/page-fb-rdx-upload) for content authors
- [Security roles admin](https://github.com/petecarapetyan/page-fb-rdx-role-admin)

Additionally:

- [Back end callable functions module](https://github.com/petecarapetyan/functions-for-page-fb-rdx) to support all of the above

Each seems like it's going to have it's own permalink so that maybe I can simplify routing by at least having a set of string constants.

## A Commitment to Experiment

Tesla didn't beat all those muscle cars on it's first day.

Neither am I certain where this is going to go, but I can tell you what my objective is. I want my MPA to be as fast as it can possibly be. Period.

So if I can tinker with my mini-app-shells for a while, I should be able to measure the tradeoffs. Then I'll know if this _**Friends With Benefits**_ thing is worth the continued experimentation.
