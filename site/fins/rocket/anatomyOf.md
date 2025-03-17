---
layout: layout-sidebar
title: anatomyOf
eleventyNavigation:
  key: anatomyOf
  title: anatomyOf
  parent: rocket
  # order: 42
# FIXME - Values shown above are currently derived from the file path only, except order which is also commented out because it is optional. Correct as desired and delete comment(s).
---

# Rocket >> Anatomy of || 10

## TL;DR:

**[Automatic menus/navigation](https://rocket.modern-web.dev/guides/first-pages/manage-sidebar/)** is critical to understanding how these themes work. If you understand how that works, the rest of this page may be TL;DR

Rocket has a long list of great features, but **three features** make Rocket my default JAMstack SSG. **1)** Automatic Markdown driven menus/navigation, **2)** MDJS, and **3)** default service worker.

All themes ship with search and blog enabled. Some theme demo sites disable blogs.

## JAMstack, SSG

JAMstack and SSG are not covered here. 

It is assumed that the reader knows both of those terms, and is at least aware of the enthusiasm that some of us have for them.

I also drone on endlessly [on my blog](/blog/) about the benefits of moving off of WordPress and the like, and onto JAMstack/SSGs.

## Outline View

_Rocket is an SSG based on 11ty, which in turn is a JAMstack, and then rocket contributes it's own additional functionality sets._ **Oh my.** What a mouthful!

If we wanted to take this apart a bit, so we can understand which piece is contributed by which other piece, how would we do this?

First, let's try an outline form. Note that _even this_ is already TMI, or too much information:

- Rocket
  - 11ty
    - JAMstack
      - SSG
  - Modern web server
  - javascript imports
  - Markdown plugin
  - Rocket Navigation
    - urls via 11ty
    - menuing via Rocket
  - Rocket Drawer
    - Lion Drawer
    - automatic sidebar
  - Links checking
  - Search
  - Blog
  - default Rocket HTML theme
  - Image preset config
- Fins-rocket-themes
  - [ insert here ] HTML theme

How can we make this more digestible?

One approach is to simply ask _"Why not just use 11ty?"_

## The rocket value proposition

_"Why not just use 11ty?"_ 

As you can see above, Rocket integrates a ton of stuff for you that you could do yourself with 11ty, if you wanted to work that hard.

- Search
- Blog
- Local server
- Link checker
- Image presets
- more

So let's focus on the 3 _critical_ wins, instead:

- **[Markdown driven default menus!!!](https://rocket.modern-web.dev/guides/first-pages/manage-sidebar/)**
- [MDJS](https://rocket.modern-web.dev/docs/markdown-javascript/overview/)
- [default Service Worker](https://rocket.modern-web.dev/docs/configuration/service-worker/)

In eleventy, and even in super-admin-ish WordPress, I found the task of establishing and maintaining menus more time consuming than I wished. With Rocket, you just write your Markdown files, and Rocket takes care of **all the navigation & menus from Markdown headings. _Huge win!_** You can still customize to your heart's content, but most of the time, I don't have to.

The second thing is JS. Why? I love composing content in Markdown - it's super fast and easy. Like this page, for example - I'm writing in a frkn text editor. Can't get much snappier than that! But I'm not building a web site, I'm building a dynamic web presence! That's just fancy talk for JS and Web Components, for the most part.

MJDS lets me do _anything dynamic_ by staying in Markdown and still having **all the JS and Web Components I want. Another big win.**

The last critical piece that Rocket gives me is a **default Service Worker maintained by someone other than myself.** Don't even get me started on how much I don't enjoy jacking with a service worker, Workbox or not.
