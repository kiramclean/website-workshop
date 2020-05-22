# Intro

This is a tutorial to walk you through building your first website. We'll walk through building a simple personal profile page together, where you can showcase all the projects you complete as you learn to code, this being your first one! You can see a summary of exactly how this tutorial is structured in its outline.

## Who is this for?

This tutorial is meant for people who have no background or experience with programming or web development. It was originally developed to give at a learnathon  for high school and recently-graduated-from-high-school students.

It will assume absolutely no knowledge of the internet, web development, or any of the topics, languages, or concepts contained in this tutorial.

If you already know how to code or how to make websites, you might find this pretty boring. That being said, if you are used to building complicated web apps or non-web-based software, you might find it interesting to follow along at a faster pace to see what the minimum requirements and basic principles are for making a simple, minimalist static website.

## Following along

Throughout the tutorial you'll see links to tagged commits on GitHub that say something like "See example here" [TODO: put whatever standard thing I came up with here]. Don't worry if you don't know what git or GitHub or commits are, just know that those are links to an example online of what your project should look like at that point. 

If something isn't working the way you expect it to or if you're having trouble getting through a particular step, have a look at the link.

It's not cheating to look at good examples of how something is done. It's completely ok if that's how you learn best. The example website included with this tutorial is meant to be a helpful guide to keep you on track and help you get unstuck. You won't learn much if you just copy it, but the goal here isn't to have something to submit at the end of the tutorial, it's to _learn_ how to make a website. How much effort you put into learning  and how honest you are about trying to learn vs. just copying the answer is completely up to you.

## Feedback and suggestions

If you have feedback or suggestions for how to improve this tutorial, I would love to know about them! My goal is for it to be a useful resource for people who are brand new to web development. I've been making websites for a while now and it's easy for me to forget what was and wasn't obvious when I was first learning. If there's something you think could be made more clear, I would love to hear your feedback and use it to improve future versions of this for others. 

You can reach me on twitter as [@kiraemclean](https://twitter.com/kiraemclean) for quick comments, or make an issue [TODO: link this] in the GitHub repository for this tutorial to share your feedback.

Let's get started!

# Setup

A website is really just some files on someone else's computer that you can access over the internet. We'll worry about how to put our files on the internet later, for now we'll just make a website that only exists on our computer.

To get started, make a new folder for your project -- you can name it whatever you want, something like `site` would make sense. In the example mine is called `example`. Then make a new file inside of it called `index.html`. _It's important that the file is called exactly `index.html`_.

## Structure of a website

Web browsers





You would typically use that name for one of your page, and it would usually be the home page.

When you arrive a website, for example `www.website.com`, you're not pointing to a file (like you would be if you typed `www.website.com/about.html`), you're pointing to a directory listing of all the files.

The webserver will try to serve a file, typically called `index.html` or `index.php` by default, but it could be something different, and it's configurable by editing your webserver's config files.

If the server doesn't find any file to serve (because you didn't include an `index.html` file or because you renamed it without editing the server's config) you will see a listing of the files, which is rarely the desired behavior,  especially at the root of a website.



 At this point, your project should look like the example here [TODO: links to tag 1-initial-setup], with a folder 













