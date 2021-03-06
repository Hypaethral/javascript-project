# Part One - Acquiring The Tools

## The IDE
[Download VSCode](https://code.visualstudio.com/Download) (or don't if you already have an IDE you like for JavaScript or wanna try something else.)

If the IDE you're using is new to you, get comfy! Try the walkthrough.  You can fiddle with color themes and keybindings from your favorite editors.  Autosaving and integrated terminal are big ones for me personally!

## Node.js ([Download](https://nodejs.org/en/))
Unfortunately I could make three repositories worth of tutorials on Node alone.  For now, just think of nodeJS as another language entirely run on servers instead of in the browser, which is a means to sweet advanced javascript features on the frontend (confusing, I realize).  It also comes bundled with a package manager, NPM, which we'll use to keep track of all of these things.  More on that later.

There are installation guides all over the place for Node if you get stuck.  Verify that you can run
`node -v` and `npm -v` successfully in your shell of choice before moving on.


## Webpack
So remember how we installed Node and I was all, "yo this server-side language is going to give you language features on the frontend" and you were all "dude that doesn't make any sense"?  Well, prepare for some tiny fragments of sense!  Enter webpack [(outsourcing the explanation!)](https://webpack.js.org/concepts/).

You can install webpack globally by running

`npm i -g webpack`

We'll worry about configuring this later.

## Yarn
So we installed and ran an npm command, but what exactly *is* npm?

NPM stands for ~~nyarlathotep propagates mythos~~ node package manager, and it's used to manage libraries of code and those libraries' libraries and those libraries' libraries and...  All right, here's a picture to get us started:

![unable to load pic](https://github.com/Hypaethral/javascript-projects/blob/master/environment-setup/images/package_managers.png "Worst analogy ever...")

Think of it like a program that manages a shopping list for code libraries. Instead of sharing the code groceries, we share and update the shopping list, because our needs are very, very specific, and certain groceries depend on other factors that we don't have to worry about. The package manager manages these dependencies and specifications based on what our shopping list tells it (in a file called `package.json` for us). 

So why is this section about package managers called Yarn instead of NPM?  Yarn is a cool alternative to NPM which locks down versions for you so you never have to worry about production environments installing the wrong version of a package or its dependencies.

In this way, the grocery analogy only got us so far... It may be more helpful to think of managing all the atoms in each grocery item: the task is more complex than what it seems, because each package (a grocery item) is comprised of many smaller pieces (atoms vs dependencies).


Install yarn with

`npm i -g yarn`

and have a look at these resource links if you'd like:
* [Good write-up on yarn](https://code.facebook.com/posts/1840075619545360) by Facebook devs.
* [yarn docs](https://yarnpkg.com/lang/en/docs/)



*[continued in part two](https://github.com/Hypaethral/javascript-projects/blob/master/environment-setup/02-create-a-project.md)*
