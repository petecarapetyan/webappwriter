# Friendlier than WordPress? WUT?

Can't beat that satisfied smile you see when WordPress helps someone launch a beautiful and original site - sometimes even in minutes. With 38m sites and climbing, and a massive number of plugins, it's the frienliest way to launch an impressively capable site.

Or, at least until SSGs started to appear and JAMstack became a thing. Don't expect WordPress to take notice, but it may be losing it's "friendliest" reputation with younger or more evolved content producers, in coming years.

## TL;DR
By cutting out the complex WP UI we can dump the server . That in turn allows us to use simple familiar files instead of a DB, which allows us to do everything locally, which lets us do it with whatever codebase is simplest and most familiar to us.

The net result is that super complex WP system becomes a simple dumb, and super fast assembly program that's really easy to maintain.

## LAMP Stack giveth, then taketh away

The bounty that is WordPress comes from it's underlying 2003 era engine - the LAMP stack.

Servers used to be how you did serious things, back in 2003 when WordPress was invented. That's how WordPress got it's friendly reputation, because the LAMP stack let "script kiddies" set up servers in minutes on any random web host back when being a server admin was a super serious corporate role. These PHP "script kiddies" were the heroes of the internet, making things possible that were previosly not even thinkable without massive corporate budgets.

But then millenials+ and shops like google and facebook took over the javascript space after 2010, and now all that LAMP stuff is actually way harder than the latest stacks allow for, and more to the point, we're not really even using servers much any more. 

What was the easiest, is now, well, harder. Lots harder. Especially if you're doing anything even remotely customized and/or complex. How did this happen?

## Very specific differences

WordPress improves every year, so to understand how another system improved faster, we really need to look at specific technical aspects.

This article will still only hit the high points - but if you're one of the few who are actually suffering from the difficulties that come with WordPress, you might at least get a glimpse at the new "friendliest" stacks.

## HTML/CSS/JS vs HTML/CSS/JS

OK, I'm being a smart aleck here, but WordPress is just HTML/CSS/JS, delivered to the browser by a complex server.

So the distinction is never on the HTML/CSS/JS side, it's only on the server that assembles it. Using the LAMP stack for that job doesn't have much of anything to do with what is delivered down the pipe.

Which means if you're doing anything on the customization side like my customers require, you're always going to have to know HTML/CSS/JS. Sorry, no win there for WordPress.

## Files vs SQL

JAMstack/SSGs - or at least the ones I know about - don't store things in SQL databases. Seems heretical - but the simple computer file system really works great for everything that builds into even the most complex site. Shocking, I know. 

This means there's a whole set of layers and databae schema that simply evaporate. Both SQL and schema can get very complex. To learn an SSG even at it's most complex, you just - shockingly - look at the files.


## CLI vs UI

After you put stuff in files, there's not a lot of complexity left. [Based on the idea that everyone in the content producer target market already knows how to do computer files.]

In 2003, that wasn't the case. The ethos then was to wrap a UI around every important operation, so you had to build a complex UI that made for handling all of the hundreds of pieces that make up a site in a complex and specialized set of forms. And then there are config files to manage the forms and interaction between the SQL engine.

SSGs don't have all that UI, but neither do they need it. Not that much complexity to manage - it's all just dumb files, and since there is no UI or DB to manage, considerably fewer, to boot.

## PHP vs [random template engine]

Any code that is required to build a site has to be maintained, so the less there is, the friendlier it is to customize and add features to.

Now that we have no database or UI to manage, it's already a lot friendlier codebase to maintain. Pretty much all that is left is to assemble all the little pieces in files into bigger pieces in the final files that go down the pipe as HTML/CSS/JS

There isn't much code left, but the nice thing is that the code that IS left can be anything. There are 232 SSGs and counting, and nobody even cares what you use to assemble your templates. Favorites come and go, but you're not stuck with PHP or really anything. Simple and whatever is familiar does the trick.

## Plugins vs JS/REST

When WordPress was invented, the LAMP stack served us well because there was no such thing as a REST API, or at least not in common usage.

So the LAMP stack was the whole important thing - and external data was a critical piece of the puzzle.

But the other 2/3s fo the internet that is not WP kept evolving beyond the LAMP stack, getting simpler and dumber. More and more functionality arrived in a-la-carte pieces - many by the same vendors like Shopify that also created WP plugins.

So now we have this odd situation where you can get stuff in either lightweight JS/REST packages and APIs, or in complex harder to maintain WP plugins. Interesting!

Who is friendliest? In this case, it's usually the simpler, easier to maintain and evolve JS libraries and REST APIs.

## Markup vs Rich Text

Rich text, in 2003, was a critical piece of the puzzle.  And people had much better things to do with their time than learn how to write that in HTML!

WordPress and others evolved as a critical alternative, allowing people to use the WordPress UI to write rich text! That editor made the process super friendly, and still does, today.

But then Wikis showed up, and millions of us began doing most of our writing in text editors, just because, frankly, we didn't have the patience to mess with rich text. Many cute languages evolved to serve this fast shorthand, and Markup ended up being the standard, now 20 years later.

This article was written in a text editor. It may appear, to you, as rich text. But like I said, I really don't have the patience for writing in rich text, and I can do anything with Markup that I need to do.

JAMstack uses regular old markup. No rich text to make formatting decisions about. No complex processes. Dumb, super fast, and I can use CSS to force all the pages to look the same. Perfect.

Friendliest, in this case, goes to SSG/JAMstack, at least for the millions of us like myself that already write in Markup for almost everything we do anyway.

## UI v Git

OK this one is tricky, on the friendly scale.

WordPress comes with it's own UI, so that makes it friendliest, especially if you compare that to a newbie learning command line git and saving those same files to git.

So for Billy Designer or Mary Content Creator who doesn't work in git every day, there's your line in the sand.

But wait! The waters get muddy fast, for a couple reasons.

1. There are now git UI