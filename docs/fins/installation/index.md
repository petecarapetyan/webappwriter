# Installation || 20

## Finished themes? Or starter/customizeable?

Finished themes could eventually be installed [as rocket presets, like this](https://www.npmjs.com/package/@webappwriter/not-alphabet-rocket-theme). The install process works perfectly, but the theme itself is more of a [POC](https://en.wikipedia.org/wiki/Proof_of_concept), because as themes go, it's pretty useless in it's current status.

None of the above preset really applies to what is below, because all current themes are unfinished at the moment, and would require you to jump in and complete the HTML/CSS to suit your needs.

Read on, if you're still interested in pursuing, as is.

## Pre-reqs:

- same pre-reqs as necessary to install and run rocket
  - you're running node 14+
  - same basic skillsets HTML/CSS git npm etc 
- you've cloned [rocket-themes](https://github.com/petecarapetyan/rocket-themes) into the same folder that you intend to create a new `my-project` to try out one of the rocket themes

## High Level

First, for rocket newbies, the high-level on what we're going to do. 

_[There's an 30 second way to do it below](/fins/installation/#one-cli-command-instead), but this is for when you want to know what it's doing, before you skip to the automated script._

- Install the basic 5 required files into your new rocket project, just like you would any other rocket project.
- Install some extra folders of markdown files so you'll have some actual content to navigate to when you try out the new theme. Again, same as you would do with any rocket project.
- _**Copy paste the theme files themselves from the `rocket-themes/[some-theme]/src/docs` into `[my-new-project]/docs`**_
- run `npm i`
- run `npm start`

The part in bold above, is the only thing different from a normal rocket project.

Next, let's look at doing all of this manually, in case you never installed rocket before. For all you rocket newbies.

## Manual, all the way

### Follow the rocket guide

Go to [rocket guide](https://rocket.modern-web.dev/guides/first-pages/getting-started/) and set up your new project, exactly as it instructs.

Once you get it all running and you're satisfied that you understand it, you are ready to add a theme from `rocket-themes`, as below.

Your running project files should now look like this, if you're in vscode:

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-initial-vscode.jpg" alt="my project initial vscode" />

### [Sorta optional] Seed some markdown copy

This is optional, only in the sense that everything else will still work, if you don't do this step.

But if you don't do this, you won't have any content to navigate to.

Either [follow this guide for adding content](https://rocket.modern-web.dev/guides/first-pages/adding-pages/) or just copy in Lorem Ipsum markdown content from `rocket-themes/seed-markdown/docs` if you are too lazy to seed the content manually.

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-lorem-vscode.jpg" alt="my project initial vscode" />

### You can now launch your site

_You haven't installed your new theme yet - but not required._

Again, follow the rocket guide or else just run these two commands:

- run `npm i` from the shell
- run `npm start` from the shell

You should see a boilerplate rocket project launch in your browser.

### Manually install a theme

- copy everything in `rocket-themes/[some-theme]/src/docs` into `[my-new-project]/docs`

That's it. Your new theme is "installed"

Your source docs should look like this:

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-theme-vscode.jpg" alt="my project theme vscode" />

Enjoy! You're done. Run `npm start` in your new project and you're looking at your new site in localhost.

## One CLI command, instead

There be dragons here, for shell scripting newbies. So if you're _**not a shell noob**_, and you took a few seconds to inspect `try.sh` for  anything not OK (**such as over-writing an existing project**), then run as below:

- `chmod +x try.sh`
- **`./try.sh my-project not-five38`** That's it!

That creates (or over-writes) `my-project` as a sibling to `rocket-themes` and installs the `not-five38` theme in it, and then runs npm and launches it in your browser.

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-five38-vscode.jpg" alt="my project five38 vscode" />

30 seconds, and you're live on localhost with your new theme.

Now you can re-run with different themes and the same project, to try out different themes in seconds. Though you might need to un-comment the `rm -rf ../$1/docs` line in `try.sh` first, to avoid some unpredictable results if file structures are not identical between themes.

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-two-vscode.jpg" alt="my project two vscode" />

Now you're looking at a new theme in your browser:

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-ibm-vscode.jpg" alt="my project not ibm vscode" />
