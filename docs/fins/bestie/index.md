# Friendly Customization || 40

**TL;DR:** 

How to stay on friendly terms with your favorite SSG _when you start going deep_ into personalizing your theme? If you set yourself up properly, it's easy to stay best friends.

Then you can customize and personalize your chosen theme, to your heart's content.

The tips below are less important, if you're just doing shallow theme modifications like colors.

## Too Much Friendliness already?

You could say that SSGs are already _**too**_ friendly for their own good. [They are certainly friendlier than their UI driven predecessors](/blog/will-wordpress-go-way-of-dodos/)

SSGs use a **sequential overwrite based on inputs** pattern.

There are three _**very serious**_ side effects to this otherwise friendly pattern:

- the **overwrite** part
- the **sequence** part
- the **inputs** part

Since all of these are attempts to give you freedom, maybe that's why I never hear people talking about the side effects.

But I spend unwanted minutes(?) on the side effects - sometimes on a daily basis. Maybe that's because I'm autistic? Either way, here's how I compensate for all that freedom.

## The overwrite foot-gun

As an illustration only, let's compare strongly typed and weakly typed languages. In strongly typed, once you establish a structure it can't be overwritten. It is simply impossible. SSGs are more analogous to the weakly typed languages - overwrites are just taken for granted, for the most part.

Or CSS. You can set the same selector value in 10 different places in 7 different CSS files all referenced by a single HTML page. But only the last one has any effect, usually. Allowing that kind of freedom could be considered friendly, but it can also leave me searching for _which one?_

In this sense, templating systems are their own house of horrors, and they all tend to share this same foot gun. Pretty much by definition, a templating system loops over stuff and writes wherever and however it needs to, to get the job done. Overwrites aren't even discussed as an issue, they are just _writes_. If they also over-write, then it's just them trying to be friendly and let you write what you need to write.

What all this means is that SSGs can give you a lot of overwrite styled foot guns by trying to be super friendly. Like any foot-guns, some degree of extra care may be required if you like your feet.

## Strategy 1 - It's the sequence!

One remedy to all that freedom is spending a few seconds really grokking the sequences. If the overwrites are always in the correct sequence, it's never a problem, right? The last one was the one you wanted, anyway. Friendly!

So the first strategy is just make sure you're aware of these two specific types of sequences so you know where to apply any changes. Neither is hard to find and internalize, nor do you have to be a template coder to grasp the sequence.

- Which css files get applied in which sequence?
- Which template loops get run in which sequence?

Once you have these two things identified you can quickly resolve any otherwise time consuming sequenced overwrite problem. Or, as easily as possible.

Don't even get me started on the giant foot gun that is CSS. A topic for a different day.

## Strategy 2 - It's the inputs!

The whole point of your friendly SSG is to make sure you're not having to be some kind of hyperactive policeman watching out for the SSG's well meaning foot guns. Which brings us to the second strategy to dealing with your favorite friendly SSG. Understanding enough of 11ty, Rocket's backbone, to interject your own personalized changes into your site.

RTFM is mostly against the rules, for me. Not until everything else fails. So I'm not going to tell you here that RTFM is step 1. Instead, the friendlier thing to do is isolate those instances where you may have to resort to RTFM, and how to keep it friendly, when you do. RTFM in the service of watching out for our feet :)

Friendliness, in this particular instance, is 11ty's most notable trait. It does soooo very much for you, and with such _flexibility_. Template system? Pick from a dozen - and counting. Data sources? Use any of several types, any of seemingly infinite locations. And naming conventions keep it all straight, as does your chosen folder structure.

But here's what it doesn't keep straight - your brain. It offers flexibility to be friendly, but you have to RTFM to really understand what it just did. Fortunately, the docs are well written and widely regarded as easy to understand. Once you see it, it's like _'duh'_.

Then rocket adds even more layers of implicit behavior. Really neat stuff, but no way you're going to understand how to customize it fully without spending at least a few minutes in the guide or docs.

See [this section below](#top-n-11ty-and-rocket-features) for my _**top n 11ty and rocket features**_ that you might eventually have to break down and RTFM. A sad day for us all :(

## Strategy 3 - It's the workflow

So I'm just going to come out and say it. SSGs are a much different workflow than other coding workflows I have used.

If you ever got coached in woodworking, someone warned you "Measure twice, cut once." A lot of coding workflows are like that. I think about the design carefully, try stuff out, then refactor after the long coding session. That's just how the process works, for a lot of us.

By comparison, I find that SSGs are more like mowing the lawn. You just, well, mow the lawn. Thinking isn't so much a part of the process, and the best part is the instant gratification.

How long does it take to run an experiment in an SSG? Sometimes it's just saving a file, you don't even have to restart localhost. Worst case is 3 seconds to tab back to the shell and control C up arrow to restart localhost, such as if you renamed a file.

This changes the workflow quite a bit. So here are some guidelines that I use for SSGs, that may be different from other types of coding that you or I do.

- **Religiously stick to the only change one very small thing rule** and then check it out.
- **Commit much more frequently than normal** coding - then use your IDE to double check git diffs, before each commit.
- **dev tools** play more prominently in my SSG workflows than other types of coding that I do.

As a result of all these high velocity trivial commits, I end up with a hyperactive git log where all the commits are labeled `WIP` but since most were so trivial, I never seem to care. I still do the occassional rollback, but I'll just use dates and fast experiments rather than try to nail it on the first attempt.

## Top n 11ty and rocket features

As referenced above, I don't RTFM until all else fails. So if things fail for you on more complex theme personalizations, here's what you might have to RTFM first.

- Data cascade
- Menu
- How 11ty walks the directory

There are, of course, other things such as the Markdown plugin that you also might want to read about, but I didn't find them very likely to get in my way during the process of customization or personalization.


right about here is where i could insert a reference for a 10 minute video on standard customization workflow
