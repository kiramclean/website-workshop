# HTML

Now we'll get started writing some code.

## What is HTML?

HTML is a markup language used to semantically describe content. It's used to annotate normal text, like what we just wrote, so that browsers can display it in a way that makes sense.

HTML wraps pieces of content in "tags", which give browsers information about how render the text. A tag starts with `<` or `</` and ends with `>`. When we say something is "wrapped" in a tag, that means there's an "opening tag", which is one that starts with `<` before it, and a closing tag, which is one that starts with `</`, after it. 

Don't worry if that doesn't make sense yet, we'll see what it looks like in context next.

## Plain text to html

All HTML pages have a few things in common. The first thing at the beginning of an html document is a message to the browser about what kind of document it is, which looks like this: `<!DOCTYPE html>`. This is really a historical artifact from the early days of the internet when we had to give browsers information about what kind of content to expect, because there multiple different versions of HTML in use. These days all you really need to know is that valid HTML documents start with that tag at the very top, which is sometimes called a "doctype declaration".

The second thing all HTML documents have in common is that _all_ the content is wrapped in an `<html></html>` tag. This is called the "root" element, and it tells the browser that this is the beginning of our html content.

Turn your plain text document into an HTML document by adding a doctype declaration to the top and wrapping the rest of the content in the `<html></html>` tag, like [this](https://github.com/kiramclean/website-workshop/blob/3-text-to-html/site/index.html):

```html
<!DOCTYPE html>
<html>
  Kira McLean

  About
  Hi! Thanks for visiting my site. I'm a Software developer in Montreal, Canada.
  Check out some of my projects below.

  Projects
  - Profile website (right here!)
  - Blog
  - Blackjack
  - Tic tac toe

  Follow me on github or twitter
</html>
```

### Formatting

You'll notice that I indented all the content one level so that it's clear that it's _inside_ the `<html></html>` tag. This is how HTML should be structured in a file, so it's a good practice to pick up right now. It makes our code much easier to read once there are more tags.

Remember that the spacing of the content inside your text file doesn't affect how the browser renders it. We'll learn more about how to change the way your content looks in a bit. 

## HTML `head`

The next thing all HTML documents have in common is that the next piece of information the browser gets after the doctype declaration is the `<head></head>` tag. This part of an HTML document contains metadata about the page you're looking at. In this case metadata means information that the browser needs in order to render the page properly, but that doesn't need to be rendered for users to see.

There are loads of possible things you can put in the `<head></head>` of an HTML document, but there are at least two that you should always include.

### Title

This will be show up as the title of the browser tab and is what your web page will be called if someone bookmarks your web page. It looks like this: `<title>This is my title</title>`.

### Character set

You should always include a `<meta>` tag with a `charset` attribute. HTML tags can have attributes, which are extra information that's relevant to that particular tag. A valid meta tag to put in the `<head></head>` of your HTML document looks like this: `<meta charset="utf-8">`.

This is there to tell the browser which character set to use. It's not super important to understand what that means, but it has to do with telling the browser how to render the text that it finds in your file. 

In the early days of programming not everybody translated the letters we understand into the numbers that computers understand the same way, and "character encoding" is a whole topic around sorting that out. It won't come up again for us, we just need to make sure to include this tag in our pages. 

Pretty much all web pages use "utf-8" encoding now because it supports the widest range of characters.

### Valid HTML `head`

All of this adds up to a valid HTML `head` tag, and our document should look like [this](https://github.com/kiramclean/website-workshop/blob/4-add-head/site/index.html) now:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Kira McLean</title>
  </head>
  Kira McLean

  About
  Hi! Thanks for visiting my site. I'm a Software developer in Montreal, Canada.
  Check out some of my projects below.

  Projects
  - Profile website (right here!)
  - Blog
  - Blackjack
  - Tic tac toe

  Follow me on github or twitter
</html>
```

If you refresh your page in the browser, you'll see it looks the same. There is one different you can notice now, though, which is the title of the page in the browser tab. That's the title we set.

## Closing HTML tags

You might have noticed that some HTML tags (like `<html></html>` itself, `<head></head><head>`, and `<title></title>`) have both an opening tag and a closing tag, while others (like `<meta>`) only have the opening part. Tags like the `<meta>` tag that don't have anything after them are called "self-closing" tags. They don't need to be closed because they don't have any content.

We'll see more examples of self-closing tags later. As a general rule, if a tag as any content inside of it, it needs to be closed, otherwise you only need the opening part.

## Semantic markup

Our project is starting to look a little more like code and a little less like plain text. We use HTML to semantically describe the structure of our content, which allows browsers to interpret it. We saw earlier that when our file only contained plain content, the browser rendered it all in one line. It didn't know what to make of our text and just dumped it all on the screen.

This is really the point of HTML. It allows browsers to interpret the structure of our content so it can be rendered in a way that looks good. It's much easier for users to read a document that's well structured and laid out than it is to read a big blob of text.

There are other benefits of using semantic HTML markup, too. It allows search engines to understand what's on our web page and add them to their indexes. People who browse the internet using assistive technologies like screen readers also benefit from well laid out documents. And it also allows us to target certain tags with CSS or JavaScript to augment the appearance or behaviour of our page. We'll learn about these languages later.

### Markup our content

Looking at the content we have, we can see it has some structure, it's just ambiguous right now because it all looks the same. We have a page header, some sub headings, a list of things, and some loose text.

#### Header tags

HTML supports 6 levels of headers, starting with  `<h1></h1>` up to `<h6></h6>`  They signify the beginning of a section of content. Add some headers to your content to show what the title of each section is, like [this](https://github.com/kiramclean/website-workshop/blob/5-add-headers/site/index.html):

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Kira McLean</title>
  </head>
  <h1>Kira McLean</h1>

  <h2>About</h2>
  Hi! Thanks for visiting my site. I'm a Software developer in Montreal, Canada.
  Check out some of my projects below.

  <h2>Projects</h2>
  - Profile website (right here!)
  - Blog
  - Blackjack
  - Tic tac toe

  Follow me on github or twitter
</html>
```

## Structural markup

HTML is also used to add structure to our page. There are several tags that describe the _location_ of an element on the page, more than it's _meaning_, but these are HTML tags, too. We 



























