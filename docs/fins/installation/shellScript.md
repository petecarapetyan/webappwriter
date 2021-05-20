# Installation >> Shell Script || 30

**TL;DR:**


**This shell script is destructive!**, always `git commit` before running on an existing folder!

`./try.sh mysite not-five38 seed start` 

- writes or overwrites ../mysite with a new 'not-five38' theme
- also adds Lorem Ipsum content
- starts it up in localhost

`./try.sh mysite not-slashdot keep start` 

- to swap to not-slashdot theme
- and keep any content changes you made

## try.sh shell script is destructive!

Everything on this page assumes that you are super-cautious and wise. Hah!
If only I could count on myself, in that respect!

So just don't use this `try.sh` script _**unless:**_

- You're making a bran new project and so you don't care
- You have forced yourself to be cautious and always at minimum, run `git commit` before you run `./try.sh` against an existing project.

I created an issue to provide some automated safeguards, but they are not on the schedule yet.

## Pre-reqs:

> The fine print: <br>_Be sure to consult [I ♥ HTML req](/fins/html/) before committing to a Fins - Rocket Theme_ <br> All themes are always considered incomplete, unlike WordPress themes, where the owner is not expected to jump in and adjust the HTML/CSS manually

- same pre-reqs as necessary to install and run rocket
  - you're running node 14+
  - same basic skillsets HTML/CSS git npm etc 
- you have git cloned [fins-rocket-themes](https://github.com/petecarapetyan/rocket-themes) into the same folder that you intend to create a new `mysite` to try out one of the rocket themes

It is suggested, but perhaps not required - that you may be happiest if you have already installed and played with a default rocket install, enough to get a feel for the basics.

## One CLI command

There are reasons to not like shell scripting for this, but I put them [here] so you wouldn't have to read them.

- `chmod +x try.sh` one time only
- **`./try.sh my-project not-five38`** That's it!

That creates (or over-writes) `my-project` as a sibling to `rocket-themes` and installs the `not-five38` theme in it, and then runs npm and launches it in your browser.

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-five38-vscode.jpg" alt="my project five38 vscode" />

30 seconds, and you're live on localhost with your new theme.

Now you can re-run with different themes and the same project, to try out different themes in seconds. Though you might need to un-comment the `rm -rf ../$1/docs` line in `try.sh` first, to avoid some unpredictable results if file structures are not identical between themes.

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-two-vscode.jpg" alt="my project two vscode" />

Now you're looking at a new theme in your browser:

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-ibm-vscode.jpg" alt="my project not ibm vscode" />
