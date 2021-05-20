# Installation >> Manual Install || 60

**TL;DR;**<br>Permanent daim bramage could result from attempting to follow the instructions on this page.

You are advised to return to [shell script installation](/fins/installation/shellScript/), immediately.

## High Level

First, for rocket newbies, the high-level on what we're going to do. Just reading this confusing sequence should be enough to convince you of the benefits of automating it with a script, instead.

- Install the basic 5(?) required files into your new rocket project, just like you would any other rocket project.
- Seed some extra folders of markdown files so you'll have some actual content to navigate to when you try out the new theme.
- _**Copy paste the fins-community files from the `fins-rocket-themes/[some-theme]/src/docs` into `[mysite]/docs`**_
- _**Copy paste the theme files themselves from the `fins-rocket-themes/[some-theme]/src/docs` into `[mysite]/docs`**_
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

- copy everything in `rocket-themes/[some-theme]/src/docs` into `[mysite]/docs`

That's it. Your new theme is "installed"

Your source docs should look like this:

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-theme-vscode.jpg" alt="my project theme vscode" />

Enjoy! You're done. Run `npm start` in your new project and you're looking at your new site in localhost.

