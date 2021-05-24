# Friendly Customization || 50

**TL;DR:** 

How to stay on friendly terms with your favorite SSG _when you start going deep_ into personalizing your theme? If you set yourself up properly, _**it can be easy to stay best friends.**_

Then you can customize and personalize your chosen theme, to your heart's content.

The tips below are less important, if you're just doing shallow theme modifications like colors.

## Too Much Friendliness already?

You could say that SSGs are already _**too**_ friendly for their own good. [They are certainly friendlier than their UI driven predecessors](/blog/will-wordpress-go-way-of-dodos/)

SSGs use a **sequential overwrite based on inputs** pattern.

There are three _**very serious**_ side effects to this otherwise friendly pattern:

- the **overwrite** part
- the **sequence** part
- the **inputs** part

Since all of these _**are attempts to give you freedom,**_ maybe that's why I never hear people talking about the side effects. Freedom is supposed to feel positive, not overwhelming.

But I spend unwanted minutes(?) on the side effects - sometimes on a daily basis. Maybe that's because I'm autistic so I don't shift contexts as nimbly as others? Either way, here's how I compensate for all that freedom.

## The overwrite foot-gun

To illustrate, let's compare strongly typed and weakly typed languages. In strongly typed, once you establish a structure it can't be overwritten. It is simply impossible. _**SSGs are more analogous to the weakly typed languages**_ - overwrites are just taken for granted, for the most part. Freedom.

Or CSS. You can set the same selector value in 10 different places in 7 different CSS files all referenced by a single HTML page. But _**only one has any effect,**_ usually. Allowing that kind of freedom could be considered friendly, but it can also leave me searching dev tools for _which one?_

In this sense, templating systems are their own house of horrors, and they all tend to share this same foot gun. Pretty much by definition, a templating system loops over stuff and _**writes wherever and however it needs to,**_ to get the job done. Overwrites aren't even discussed as an issue, they are just _writes_. If they also over-write, then it's just them trying to be friendly and let you write what you need to write.

What all this means is that SSGs can give you a lot of overwrite styled foot guns by trying to be super friendly. Like any foot-guns, some degree of extra care may be required if you like your feet.

## Strategy 1 - It's the sequence!

How to learn what sequence the SSG overwrites?

One remedy to all that freedom is spending a few seconds really grokking the sequences that a page is written in, or CSS is applied in. If the overwrites are always in the correct sequence, it's never a problem, right? The last one was the one you wanted, anyway. Friendly!

So the first strategy is just make sure you're aware of these two specific types of sequences so you know where to apply any changes. Neither is hard to find and internalize, nor do you have to be a template coder to grasp the sequence.

- Which css files get applied in which sequence?
- Which template loops get run in which sequence?

Once you have these two things identified you can quickly resolve any otherwise time consuming sequenced overwrite problem. Or, as easily as possible.

Don't even get me started on the giant foot gun that CSS is.

## Strategy 2 - It's the inputs!

Here's a fun twist - _**11ty's best feature can break your flow**_ - if you have what seems to be the "normal" approach to time management.

1. 11ty is _**way flexible**_. Lots-o-different ways to do the data thing.
1. Normal human time management means RTFM is _**not even**_ the first order of the day.

#2 above works as the default, for me. Except in the presence of #1 above. That's when I wish I had forced myself to RTFM. So here's my RTFM list, in case you want travel deep into the land of customizing an 11ty site:

- [The Data Cascade](https://www.11ty.dev/docs/data-cascade/) - holy smoke I never thought I'd see so many great ways to collect structured input in one platform! And Rocket seems to use them all.
- [Collections](https://www.11ty.dev/docs/collections/), of what?
- [Rocket Navigation](https://rocket.modern-web.dev/guides/first-pages/manage-sidebar/) is totally intuitive when you see it in action, if not yet at the docs level.

By this time you're beginning to maybe not wonder what "frontmatter" is, and other contextually defined words from the 11ty world.

Recapping, for emphasis: SSGs in general, and 11ty/Rocket specifically, might be easier to personalize/customize after a specific chunk of RTFM, first. Or at least that's true when it comes to **taking in data structures as inputs.**

Don't forget, the structured input data provided by these files is replacing an entire structured database and admin-UI for a CMS such as WordPress. There's a reason why that data is so important to the process.

## Strategy 3 - It's the workflow

So I'm just going to come out and say it. SSGs are a much different workflow than other coding workflows I have used.

If you ever got coached in woodworking, someone warned you "Measure twice, cut once." A lot of coding workflows are like that. I think about the design carefully, try stuff out, then refactor after the long coding session. That's just how the process works, for a lot of us.

By comparison, I find that SSGs are more like mowing the lawn. You just, well, mow the lawn. Thinking isn't so much a part of the process, and the best part is the instant gratification.

How long does it take to run an experiment in an SSG? Sometimes it's just saving a file, you don't even have to restart localhost. Worst case is 3 seconds to tab back to the shell and control C up arrow to restart localhost, such as if you renamed a file.

So here are some guidelines that I use for SSGs, that may be different from more typical coding that you or I do as software developers.

- **Religiously stick to the only change one very small thing rule** and then check it out.
- **Commit much more frequently than normal** coding - then use your IDE to double check git diffs, before each commit.
- **dev tools** play more prominently in my SSG workflows than other types of coding that I do.

As a result of all these high velocity trivial commits, I end up with a hyperactive git log where all the commits are labeled `WIP` but since most were so trivial, I never seem to care. I still do the occassional rollback, but I'll just use commit dates and fast experiments rather than try to nail the rigtht rollback on the first attempt. YMMV.

## Other Rocket features you may need to RTFM

You may find [these Rocket explorations](/fins/rocket/anatomyOf/) handy for understanding how the various parts of every Rocket page work together.

There are, of course, other things such as the Markdown plugin that you also might want to read about, but I didn't find them very likely to get in my way during the process of customization or personalization.
