# 1.2 Typography

So we're going to continue off from where [Hello World](chapter-1/hello-world/) left off and talk about text. I'm not going to go into [every single text based tag in HTML](http://baselinecss.com/typography.html), but instead I'll cover the basics:

- Headings
- Paragraphs
- Quotes
- Lists

## Headings

1. let's begin by opening the `index.html` file and we're going to change our text `Hello World and Hello Mum!` into a heading; to do this we need to *wrap* a heading tag around our text, so let's begin by adding the start of the heading tag before our text, so write `<h1>` at the start of that line
2. now we need to close the tag to complete the *wrapping* so we write `</h1>` (the closing tag), at the end of the line
3. save the file and open it in your favourite web browser and you should see something like [this](http://ahmednuaman.github.io/coding-for-my-sister/chapter-1/typography/headings.html)
4. finally make sure you commit this to git by opening your terminal and writing `git commit -v -m 'added a heading to my file' index.html`
4. we're just using 'Heading 1' here but [there are a few more that you can use](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements)

## Paragraphs

1. now we're gonna add a paragraph, this is pretty simple, create a new line and we'll begin by adding the opening tag of our paragraph, so write this `<p>`
2. we need to add some text to so let's go with this `You're the greatest mum ever!`
3. then close the tag by writing `</p>`
4. save the file and open it to check that the paragraph is there, it ought to look like [this](http://ahmednuaman.github.io/coding-for-my-sister/chapter-1/typography/paragraphs.html)
5. don't forget to commit it

## Quotes

1. now you may not use quotes straight away but they're a good thing to understand them so let's start by writing the opening quote tag on a new line `<blockquote>`
2. on a new line we add our quote, so let's use `Look ma, I'm coding!`
3. then on a new line we need to cite ourselves so we place that in a footer of the quote by using the `<footer>` tag
4. we then fill the tag with our name and title, in this case let's use `Me, a developer`
5. and finally we close the footer tag by writing `</footer>` and on the following line we close the quote by writing `</blockquote>`
6. save the file, preview it and it ought to look something like [this](http://ahmednuaman.github.io/coding-for-my-sister/chapter-1/typography/quotes.html)
7. and now commit it

## Lists

We're going to look at two types of list tags in HTML: the ordered and the unordered list. One creates bulleted lists and one creates numbered lists (respectively).

### Unordered Lists

1. on a new line open the tag by writing `<ul>` (`ul` stands for **u**nordered **l**ist)
2. on the next line write `<li>` (`li` stands for **l**ist **i**tem) and within write whatever you want your list to contain, in this case let's go with `This is an unordered list item!` and close the list item by writing `</li>`
3. make as many list items as you want, close the list tag by writing `</ul>`, save the file, preview it and it ought to look something like [this](http://ahmednuaman.github.io/coding-for-my-sister/chapter-1/typography/ul.html)

### Ordered Lists

1. this is gonna be quick and dirty: copy and paste the unordered list and change the `<ul>` tags to `<ol>`, that'll change the list to an ordered one, so save, preview it and check it looks like [this](http://ahmednuaman.github.io/coding-for-my-sister/chapter-1/typography/ol.html)

Don't forget to commit your file! 