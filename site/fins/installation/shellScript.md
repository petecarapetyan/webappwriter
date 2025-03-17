---
layout: layout-sidebar
title: shellScript
eleventyNavigation:
  key: shellScript
  title: shellScript
  parent: installation
  # order: 42
# FIXME - Values shown above are currently derived from the file path only, except order which is also commented out because it is optional. Correct as desired and delete comment(s).
---

# Installation >> Shell Script || 30

**TL;DR:**

**This shell script is destructive!** Always `git commit` before running on an existing folder!

`./try.sh mysite not-five38 seed start` 

- writes or overwrites ../mysite with a new `not-five38` theme
- also adds Lorem Ipsum content and random images
- starts it up in localhost

`./try.sh mysite not-slashdot keep start` 

- to swap in `not-slashdot` theme
- and keep any content changes you made

## try.sh is for new or git projects only!

[More discussion on why shell scripts are not always fashionable](/fins/installation/whyShell/)

Don't use the `try.sh` script _**unless:**_

- You're making a new project and so you don't care about deletions/overwrites yet.
- You have forced yourself to be cautious, and always at minimum, run `git commit` before you run `./try.sh` against an existing project.

I created [an issue](https://github.com/petecarapetyan/fins-rocket-themes/issues/1) to provide some automated safeguards for the destructive overwrites below, but they are not on the schedule yet.

## Pre-reqs:

> The fine print: <br>_Be sure to consult [I ♥ HTML req](/fins/html/) before committing to a Fins - Rocket Theme_ <br> All themes are always considered incomplete, unlike WordPress themes, where the owner is not expected to jump in and adjust the HTML/CSS manually

- same pre-reqs as necessary to install and run rocket
  - you're running node 14+
  - same basic skillsets HTML/CSS git npm etc 
- you have git cloned [fins-rocket-themes](https://github.com/petecarapetyan/rocket-themes) into the same folder that you intend to create a new `mysite` to try out one of the rocket themes

It is suggested, but perhaps not required - that you may be happiest if you have already installed and played with a default rocket install, enough to get a feel for the basics.

## Usage

`./try.sh mysite not-five38 [seed,keep], [start,not]` is the fuller explanation.

- `chmod a+x try.sh` one time only, if required to make it executable
- **`./try.sh mysite not-five38 seed start`**
  - installs into `../mysite` **DESTRUCTIVE OVERWRITE!**
  - installs the `not-five38` theme
  - `seed`s the project with Lorem Ipsum content and random images
  - `start`s the project in localhost

30 seconds to npm install, and you're live on localhost with your new theme!

- **`./try.sh mysite not-apnews keep start`** 
  - installs into `../mysite` **DESTRUCTIVE OVERWRITE!**
  - Swaps out `not-apnews` for the theme
  - `keep` leaves your existing data in case you have started on the content
  - `start` starts up localhost

That is how you swap in a theme, any time you want to try a different one.

- **`./try.sh mysite not-reddit keep start`** 
  - installs into `../mysite` **DESTRUCTIVE OVERWRITE!**
  - Swaps out `not-reddit` for the theme
  - `keep` leaves your existing data in case you have started on the content
  - `not` does NOT start up localhost

That is an example without starting up localhost
