
# The Sweet Spot

<img class="bordered" src="/_merged_assets/_static/images/webSweetSpot.svg" alt="FiveThirtyEight.com screenshot" />

One piece at a time, here's how we may have reached the sweet spot, and why it's the _**last thing**_ in the world we might ever notice.

Weird, but wonderful. How to take advantage?

## What is a framework?

The "framework" or platform is a decades old idea to solve a decades old problem. The browser standard was immature, and the DOM - and even JS, a little bit, sucked. Enter the "framework" to solve the problem.

Except, it wasn't a problem. It was a big **set** of - ahem - _opportunities?_ Did I use the right word? Different frameworks evolved, year after year, to address each one, in different ways. Soon it became "I'm an Angular developer" or "I'm a React developer" or Drupal, or ....

A framework included all that stuff that the language and the browser standard didn't have. So now we get to work as a tribe, be buddies, share an ecosystem - go DX!

That's why "better" isn't better. Cowboys and Indians is a fun game, and _this vs that_ framework depends on - well - we keep our guns loaded and we stick together. Everything depends on the browser standard staying immature and JS and the DOM sucking, so we don stick with our framework's fixes tha we know and love.

Speed and efficiency comes from knowing the lingo of the tribe, not the relative merits of the platform. That's an important distinction.

So that's the first pattern we look for - providing whatever we need in a single ecosystem.

## But wait, there's more!

You might be eager to point out that all is not Cowboys and Indians - sometimes it's City vs Country or even East vs West. 

Goodness gracious, I spent decades coding everything on the dang back end, in Java servers. Or others did the same, in PHP or Python. In this world, there was no client side code, or at least not much of one.

I bring it up here only to illustrate a shared priority. If my first concern is about how to maintain a static approach to my work, rather than the better experience for my customer. Not concerned about keeping developers safe from learning new standards, not here. This site is all about the better experience for the customer as a baseline.

If that means I gotta learn something new, so be it. Tough luck. Life goes on.

As a side note only - standards are a finite set of things that I need to learn, if I want to keep up with the browser standard and JS/TS language. It only _feels_ infinite, sometimes.

So that's another feature of the sweet spot - it needs to live where it serves the customer best.

## Woops, somebody improved DOM and JS

Sigh. So much emotion gets in the way when I'm forced to do things differently. Perhaps I'll just resist?

Look, I'm just picking on React or Angular here as a point of comparison. But it could just as easily be Gatsby or VuePress or Laravel/PHP.

In the unfortunate case of the React ecosystem, VDOM and JSX taught the browser standard folks how to implement nearly identical functionality in the standard browser. But now, if I'm a React dev, now suddenly I'm writing legacy code? Is that really fair? Doesn't feel that way.

But it is that way. And it's not just React. Here's a modest sampling:

- css variables vs scss 
- file based SSGs vs SQL based Wordpress, Drupal, and the like
- fetch vs axios
- CSS grid vs Bootstrap or many other
- too many others to mention here

The resistance is palpable. You simply don't ask me to learn something new when I could already be done with familiar legacy stacks. But that's exactly what is happening, here.

So these improvements lead us to the next section: When to adopt the new standards?

## Conclusion: Tests to the rescue:

We need a quick set of tests to continue, in the face of what feels like an infinite array of options. Arguments or discussions between tribes isn't going to feed anything but my fragile ego.

1. **Substitutions:** _Have my favorite stacks/approaches/whatever become a legacy substitute for something that is now in the DOM or the JS/TS language?_ If so, migrate immediately, for that one piece, anyway. This is a pretty easy black/white test.
1. **Practices:** Already we get into the grey area of better practices. _Which is better? Webpack or Rollup?_ These tests are never definitive, because the answers differ depending on context, and even which version of which stack. So we still test for these, and we prepare ourselves for switching out stacks when that context demands same.
1. **CRO:** WUT? Since when is CRO even an issue for a dev? Isn't that on the business side? _CRO is about results._ In what other world do results not even enter into the discussion? To me, this shows how distracted we are by DX. Results is all that matters in a mature context. And almost never discussed in polite society of the dev world.

The proposal here is that these 3 tests give us instantaneous answers, even if they are always changing.

So now we still have some grey areas in the form of contextual switches, but Goldilocks now has a map to grandma's house, and it's not just "which tribe am I in?" any more.

## Downstream takeaway: OWC

If you were autistic like me, you might be exasperated by that human need to work as a group. I don't read a group's social signals well, so I tend to rely less on feelings, more on inadequate versions of pattern matching, like the above 3 tests.

So let's first assume that humans(devs) need to feel they are a part of a group, first. 

You might ask "Which group or framework?" rather than "Which stacks?".

For this I would tell you that there is a somewhat loosely connected group of devs which pretty much sticks with the first two tests and builds what you might think of as "frameworks" for same. Even if they themselves would never ever use that term - because they are nominally anti-framework.

So that is the main takeaway of this site. If I do it right, it will even look easy - thanks to [11ty](https://www.11ty.dev/) and now, [rocket](https://rocket.modern-web.dev/)

## Downstream takeaway: Yax

As if to demonstrate that framework free comes in multiple flavors and perspectives, yax seems to begin with the **quite literal** interpretation of framework free.

If cowboys and indians was the metaphor, Daniel Kehoe was a leader in previous tribes - er uh, frameworks - and observes that current toolsets allow for absolute freedom from build tools, because of advancments in three specific areas. 

Lifting these directly from [this article](https://thenewstack.io/case-against-web-frameworks/):

1. **ES6 Modules:** JavaScript ES6 can support import modules, which are also supported by browsers.
1. **Module CDNs:** JavaScript modules can now be downloaded from third-party content delivery networks (CDNs)
1. **Custom HTML elements:** Developers can now create custom HTML tags, via Web Components.


I offer this here only as a marker of how far things have gone. Nobody in the dev world I travel with would ever make it past their first day without getting into the weeds of WCs and the necessary build tools et al.

I'll even go one further. Rocket lets you build a site without any of this. git, npm, Markdown - that should be enough. But I digress.

So the fact that you could develop in [Daniel's approach](https://yax.com/) says it all. Shows how far things have gone, in the direction away from static-stack developer tribalism.

## About letting Rocket get you started

What you might like about Rocket, when it is released, is that it's built from browser-standard dumb stuff by hard-core practitioners of building from browser-standard dumb stuff. And it's built from standard parts like 11ty by devs who are creative about not re-inventing or using a legacy tool once a standard matures and is easily adopted.

Much as I'd like to drag you through a word salad extolling the 100 ways to illustrate where Rocket does that for you, how about not? Yes, Rocket lets you focus on the your content (or your app) the way the React or other ecosystems do. To validate , instead search for your area of interest around 11ty, Markup, buildless web, Web Components, Lit, and all the other pieces that Rocket does for you. Or, just browse through the code for yourself.

## CRO vs Good Feelings

It does feel good to be creative and put out helpful content. But, as developers - should we stop there?

If good feelings are enough for you, then the above Sweet Spot diagram doesn't apply to you. 2 out of 3 is fine.

But I've been doing the good feelings thing for a couple decades, and all that content hasn't served a commercial purpose. Now it's time for me to learn the results part, as well.

[CRO](https://en.wikipedia.org/wiki/Conversion_rate_optimization) is well worn path, the tools are popular and free, and Rocket integrates them easily. 

So I'm going to document some of that progress here, to compare notes with others and invite future contracts.

If it slows me down, then I'm doing something wrong. More will be revealed.

## Fins - Rocket Themes

When Rocket releases later this year, you might conclude that it's a bit like what Henry Ford "Any color you want, as long as it's black". 

You don customize it, sure, but it's not a trivial affair like WordPress or Drupal themes would be.

So I started coding up 18 or so rocket themes. [Fins](/rocket-themes/) They aren't very far along, but it at least exercises the process and helps us get started.