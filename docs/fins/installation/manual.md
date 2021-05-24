# Installation >> Manual Install || 60

**TL;DR;**<br>Permanent daim bramage could result from attempting to follow the instructions on this page :)

One option would be to return to [shell script installation](/fins/installation/shellScript/) as a more positive experience.

## High Level

Setting aside the attempt at humor above, manual installs are a rather tedious and error prone process. If you miss one file or even leave an older previous version of a file without realizing it, debugging any SSG install can be a less rewarding use of time.

So that's why I recommend against manual installs, even though I proved that it worked many times, back in December 2020 - the last time I did one.

So, here goes, if you still want to go that route. 

- Install the basic 5(?) required files into your new rocket project, just like you would any other rocket project.
- Seed some extra folders of markdown files so you'll have some actual content to navigate to when you try out the new theme.
- _**Copy paste the fins-community files from the `fins-rocket-themes/community/docs` into `[mysite]/docs`**_
- _**Copy paste the theme files themselves from the `fins-rocket-themes/[not-something]/src/docs` into `[mysite]/docs`**_
- run `npm i`
- run `npm start`

The part in bold above, is the only thing different from a normal rocket project.

Next, let's look at doing all of this manually, in case you never installed rocket before. For all you rocket newbies.

## Manual, all the way

### Follow the rocket guide

Go to [rocket guide](https://rocket.modern-web.dev/guides/first-pages/getting-started/) and set up your new project, exactly as it instructs.

Once you get it all running and you're satisfied that you understand it, you are ready to add a theme from `fins-rocket-themes`, as below.

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

- copy everything in `fins-rocket-themes/[not-something]/src/docs` into `[mysite]/docs`

That's it. Your new theme is "installed"

Your source docs should look like this:

<img class="bordered" src="https://storage.googleapis.com/betterology-com.appspot.com/webappwriter/img/my-project-theme-vscode.jpg" alt="my project theme vscode" />

Enjoy! You're done. Run `npm start` in your new project and you're looking at your new site in localhost.
