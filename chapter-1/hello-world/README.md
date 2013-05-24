# 1.1 Hello World

So what we're going to cover here is how to write and deploy a simple HTML page to the web. We're going to use [git](http://git-scm.org) to version the files, Sublime Text (or your favourite text editor) to write the files and github.com to host the files.

1. go to github.com
2. create a new repository (repo for short) and call it `hello-world`
3. go to your terminal and run the command `cd ~`
4. make a folder from your terminal called `Coding Tests` by running the command `mkdir ~/Coding\ Tests`
5. navigate into that folder from your terminal by running `cd ~/Coding\ Tests`
6. back on the github page you'll notice that it'll give you some instructions titled '*Create a new repository on the command line*', follow them
7. now we're ready to write some code so in your terminal run the command `touch index.html`
8. open your desired text editor/Sublime Text and open the `index.html` file that was created in the previous step
9. we're now going to begin writing some HTML code, if you want to cheat then you can [just copy and paste from one that's been prepared](index.html); if you don't want to cheat then let's go through it step by step:
	a. first we have to declare the document type for our HTML page (the 'doctype'); nowadays people generally only care about HTML5 so we'll stick with that and write `<!DOCTYPE html>` on the first line
	b. on the next line we begin our HTML [tag](https://www.google.co.uk/search?q=what+is+a+html+tag) by writing `<html>`
	c. now we begin to code the header portion of our HTML page (the bit that's *usually* hidden from view, it's generally reserved for holding any [meta data](http://en.wikipedia.org/wiki/Meta_element) and [styles](https://developer.mozilla.org/en-US/docs/Web/CSS) for the page) so we write `<head>` (opening the tag)
	d. we now define the character set for our HTML page by writing `<meta charset="utf-8" />` on a new line (notice the `/>` at the end of the tag: this means the tag closes itself; it's *self closing*)
	e. we *could* add some more tags but we're going to skip ahead and add a title to our page, we do this by writing on a new line `<title>Hello World</title>`; here the title is 'Hello World' (everything within the tag) and notice how we open and close the tag
	f. we're now at the end of our header portion for now so we close it by writing `</head>` on a new line
	g. now we're getting into the body portion of our HTML page (the bit where everything visibile is placed) so we begin by writing `<body>` on a new line
	h. within our body we're simply going to write a phrase, in this case it's `Hello World`, so stick this on another new line
	i. now that's probably enough for our body so we need to close the tag by writing `</body>` on a new line
	j. and finally you'll (hopefully) notice that we've still got our `<html>` tag open so we need to close that too to complete the document, therefore we write `</html>` on the following line

10. Hopefully you should now have a document that looks simular to this:

		<!DOCTYPE html>
		<html class="no-js">
		<head>
		<meta charset="utf-8" />
		<title>Hello World</title>
		</head>
		<body>
		Hello World
		</body>
		</html>

	Now as a *nice to have* we usually tend add an indent whenever we are inside a tag, this then creates a more legible document:

		<!DOCTYPE html>
		<html class="no-js">
		  <head>
		    <meta charset="utf-8" />
		    <title>Hello World</title>
		  </head>
		  <body>
		    Hello World
		  </body>
		</html>

11. now we need to add this file to git, this'll then allow git to track any changes to the file that we choose to commit, we begin by returning to our terminal and writing `git add index.html`
12. now we need to commit the file to git so we write `git commit -v -m 'my first commit' index.html`; here's a little explaination of the arguments for this command:
	a. the arguments that begin with a hyphen/dash (-) are called [flags](http://en.wikipedia.org/wiki/Command-line_interface) and we're using two:
		1. `-v` makes our commit verbose
		2. `-m` specifies our message with whatever string we provide, in this case it's `'my first commit'`
	b. at the end we specify the file(s) we want to commit, we can write a file, a list of files, a directory, etc… (it depends on what your terminal can support)
13. now we're ready to send our commit up to github.com so we write `git push`
14. go back to your browser where you've (hopefully) still on your github.com repo and refresh, you *should* see your `index.html` file you've just committed
15. committing isn't enough, we should push this live and *run* our file in a browser; to do this we're going to use [github.com's `gh-pages` system](http://pages.github.com/) so we do this by creating a new [branch](http://git-scm.com/book/ch3-1.html) in our git repo called `gh-pages`, so in your terminal write `git branch gh-pages`; git automatically takes the state of our current branch and duplicates it into a new branch when we create a new branch
16. now we want to edit our file so open `index.html` in your favourite text editor and change `Hello World` to `Hello World and Hello Mum!` (or whoever you want to say hello to)
17. save the file and now we're ready to commit it, so in our terminal we write `git commit -v -m 'dedicating this to my mum'`
18. and now we're going to push this commit and this new branch up to github.com, so we write `git push origin gh-pages`
19. when that's done we need to wait a few minutes for github.com's servers to have a think about it and then in your web browser visit `http://[YOUR GITHUB USERNAME].github.io/[YOUR GITHUB REPO NAME]/index.html` ([example](http://ahmednuaman.github.io/coding-for-my-sister/chapter-1/hello-world/index.html)) and you should see your HTML page all rendering and glorious!

Good work!