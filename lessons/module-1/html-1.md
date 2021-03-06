---
title: HTML I - Structure, Semantics, Forms
length: 180
tags: html, introduction, practice
---

# Overview

The front-end of the web is based on three major technologies:

* __HTML aka "STRUCTURE"__:  HyperText Markup Language (HTML) defines the structure and semantics of web pages on the web.
* __CSS aka "PRESENTATION"__:  Cascading Style Sheets (CSS) sets the look and style of a web page. CSS provides style to the structure provided by HTML.
* __JavaScript aka "BEHAVIOR"__:  JavaScript allows us to define interaction in our pages. What happens when a user clicks on a certain area?

## Vocab

- `HTML` HyperText Markup Language
- `CSS` Cascading Style Sheet
- `CSS Property` The name of a display property of an HTML element (e.g., color, border)
- `HTML Element` A building block that makes up the structure of a web page
- `HTML Tag` Used to create HTML elements. Some elements have an opening and closing tag, others only have an opening tag.
- `Id` / `Class` Ways to identify HTML elements
- `Attribute` Additional values that configure HTML elements and adjust their behavior
- `Hyperlink` A reference to an external resource
- `Block` A block-level element occupies the entire width of its parent element (container), thereby creating a "block."
- `Inline` An inline-level element only occupies the space bounded by the tags defining the element, instead of breaking the flow of the content.

***

# What is HTML?

 * HTML is used to create electronic documents (pages) that are displayed on the Web
 * Each page contains a series of connections to other pages called `hyperlinks`
 * HTML ensures the proper formatting of content (text, images, video) so that your internet browser can display them as intended.
 * HTML is made up of many Elements
 * Elements are used to hold our content and define how the browser must format and display the content.
 * Elements are created with either one or two tags.
 * Tags are created with angle brackets `<>` and are used to create elements
 * Most elements consist of an opening and closing tag which wraps content (like text)
 * Markup = the set of tags used to structure a page

***

# Anatomy of a Tag

![Anatomy of an HTML Tag](/assets/images/html-tag.jpg)

## Elements
Elements are created with one or more tags. They are used to describe and hold our content.

Elements which are created with only one tag are called [empty elements](https://developer.mozilla.org/en-US/docs/Glossary/Empty_element) and cannot have any child elements. Examples of this are `<img>` and `<input>`.

Elements which can contain child elements are created with an opening and closing tag which surround the child elements and/or text content. `<h1>Text Content</h1>`

## Example

Let's say that we had some text and we wanted to denote that this text was a paragraph.

```
This is an example paragraph. We should probably place this inside of a tag. If we place it in a tag it will be easier to access and style.
```

We'd wrap the text in paragraph tags.

```html
<p>This is an example paragraph. We should probably place this inside of a tag. If we place it in a tag it will be easier to access and style.</p>
```

We use `<p>` to signal to the browser that everything that's about to follow is part of a paragraph and `</p>` to let the browser know that this paragraph is done. When a user visits our application, the browser loads up the HTML and parses it into the elements that will eventually make up our user interface.

Here is an example of a slightly more robust document:

<p data-height="300" data-theme-id="23788" data-slug-hash="VjvOyd" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="Very Basic HTML Page" data-editable="true" class="codepen">
  See the Pen <a href="http://codepen.io/team/turing/pen/VjvOyd/">Very Basic HTML Page</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.
</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

### Turn and Talk:

* What is an HTML tag?
* What is an element?
* What makes an HTML element different that an HTML tag?
* What is the difference between a “regular” element and an self-closing, or empty, element?

***

# Required Structure of any HTML Page

Every page that is built with HTML needs to have the four same elements to start:

* `<!doctype html>` declaration: The doctype declaration is not an HTML tag, but rather tells the browser which version of HTML the page is written in.  
  - [W3C DTD Docs](https://www.w3.org/QA/2002/04/valid-dtd-list.html)  
* `<html></html>` tag wraps the entire document
* `<head></head>` tag wraps elements that shouldn't be rendered: information about the page and how to process it
* `<body></body>` tag wraps elements that should be displayed: the actual content

<p data-height="300" data-theme-id="23788" data-slug-hash="gLxjjy" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="A complete but small document" class="codepen">See the Pen <a href="http://codepen.io/team/turing/pen/gLxjjy/">A complete but small document</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

### Turn and Talk:

* What are the required elements in an HTML page?
* Why do we need to include the `<!doctype html>` declaration?
* What type of content goes in the `<head>` tag?
* What type of content goes in the `<body>` tag?

***

# Practice: Layout Structure

As front-end developers, you'll use HTML to build layouts given to you by a designer or client. It's an interesting challenge that can seem overly simple, but how you structure your HTML can have a very real impact in how you have to write your CSS and even how you use Javascript. Remember, HTML is like the frame of a house -- it has to be stable and well thought through for everything to be stable!

### Containing Elements, Semantics & Text

HTML5 has a variety of _semantic tags_, or HTML tags that provide additional meaning through descriptive naming, available for us to use. These tags are an easy way to not only make our code more understandable and clear to other developers (and our future selves), but they are also a great way to incorporate basic accessibility into your HTML for users who may need to access your website in non-traditional ways.

Let's experiment with the following semantic tags in codepen:

* `header`
* `footer`
* `h1 - h6`
* `section`
* `article`
* `p`
* `ul` and `ol`
* `div`

Use these tags to create the structure of the newspaper. Do not worry about recreating exactly, the goal is just to create the structure.

![Alien Paper](/assets/images/alien-paper.png)

<p data-height="300" data-theme-id="23788" data-slug-hash="oYePxJ" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="Blank" data-editable="true" class="codepen">See the Pen <a href="http://codepen.io/team/turing/pen/oYePxJ/">Blank</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


### Turn and Talk

*  What limitations did you notice only using raw HTML to create your newspaper site?

***

# Page Flow

### Block and Inline Elements

You might have noticed that some tags behave a little differently in a layout than others. Some tags make content stack, while others let content sit next to each other. What's that about?

This is an important distinction:

- `Block elements` stack on top of each other. Each one starts and ends on its own line.
- `Inline elements` can be used to mark up a few words inside of a block element.

Most elements are block elements. Some common inline tags you might see in the wild:

- `<em>` is used to denote that you'd like to emphasize some text.
- `<strong>` is used to denote that this text is important.

We use `<em>` and `<strong>` to denote the semantic meaning of the content.

<p data-height="583" data-theme-id="23788" data-slug-hash="ezpwZe" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="A Page with a Link" data-editable="true" class="codepen">See the Pen <a href="http://codepen.io/team/turing/pen/ezpwZe/">A Page with a Link</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

You may notice that the `<em>` tags are italicized and the `<strong>` tags are displayed in bold. The browser does this by default. That said, you should still only use these tags to convey meaning. We can change the way stuff looks later with CSS.

### `<span>` and `<div>`

All of the tags we discussed above have some kind of semantic meaning. Assistive technology devices will use them to help people with visual impairments understand the page. Search engines will use them to figure out the structure of your page. You should use semantic HTML tags whenever possible and appropriate.

Sometimes, however, you don't want a tag to have any meaning. Typically, this is when you just want to target a certain portion of the page with CSS or JavaScript and none of the semantic tags really apply.

<aside>
  <strong>Disclaimer</strong>: There are many, many more semantic tags than the ones we're discussing today.
</aside>

I like to think of `<span>` and `<div>` as the flavorless Jello of HTML tags, they don't have any meaning in and of themselves and they typically don't come with any built-in styling from the browser.

There is just one important difference between the two.

- `<div>` is a block element.
- `<span>` is an inline element.

We'll discuss these more in a later lesson when we talk about CSS.

### Turn and talk

* What is the difference between block and inline elements?

## Images and Attributes

Now that we better understand why elements decide to sit where they do on a page, let's talk about two types of *inline* HTML elements that make our pages more interactive and beautiful!

We use HTML tags to mark up text to show its semantic meaning. The browser uses these tags to structure the document. As we talked about earlier in this lesson, _most_ tags have an opening and closing tag, but a few do not. For example, images—defined using the `<img>` tag do not have a closing tag.

_Note: Elements which do not have closing tags and cannot have child elements are called [empty elements](https://developer.mozilla.org/en-US/docs/Glossary/Empty_element)_.

Consider the following:

```html
<img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/t-340/turing.png">
```
Our browser is more than happy to load up an image, but we need to tell it where that image is located. Our `<img>` tag needs extra information to know which image to display. That's where the `src` attribute comes in.

![Anatomy of an HTML Tag](/assets/images/html-tag-anatomy.png)

Let's update our page with the image above.

<p data-height="471" data-theme-id="23788" data-slug-hash="XKmwqR" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="A Page with an Image" data-editable="true" class="codepen">See the Pen <a href="http://codepen.io/team/turing/pen/XKmwqR/">A Page with an Image</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


###  Turn and Talk

* What are attributes and what are they used for?
* What are some other attributes you have used?
* Why do some elements have two tags and others just have one?


## Hyperlinks

Another important tag is the `<a>` tag. These are the tags we use for creating hyperlinks. You might have noticed that the `<a>` tag behaves a little differently than the `<h1>`, `<h2>`, and `<p>` tags. We can use the `<a>` tag to mark up a few words, while the other tags denote a big section-let's call it a "block"—of our page.

Consider the following example:

```html
<p>
  Welcome to the <a href="http://turing.io">Turing School of Software and Design</a>.
</p>
```

In this case, the `<a>` tag needs to know which url it should be linked to. We use the `href` attribute to set the links destination. `href` is an abbreviation for "hypertext reference."

<p data-height="300" data-theme-id="23788" data-slug-hash="yJYdyb" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="A Page with a Link" data-editable="true" class="codepen">See the Pen <a href="http://codepen.io/team/turing/pen/yJYdyb/">A Page with a Link</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>


***

# Your Challenge

We've covered a lot of ground so far, but there's one element we haven't talked about yet: `<table>`

And -- surprise! -- we're not going to cover it together: you're going to test out your Googling skills!

Build the structure of these following layout. Only use HTML for this challenge. The goal is to focus on building the structure of your application.

### Create this table
You can use codepen or create your own html file.

** Hint: Research the [table element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table) in HTML

# ![Flags Table](/assets/images/flags-table.jpg)

***

### Docs

* [MDN HTML Overview](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [MDN HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference)
* [HTML Styleguide](https://github.com/turingschool-examples/html)
* Also, check out the cheat sheets in independent study

***

# Forms

So far, we've done an excellent job of displaying information to the user, but we haven't really asked them for their input. HTML also includes a set of elements for building forms. Forms are an important part of a website. They allow users to send data to the web site. Most of the time that data is sent to the web server, but the web page can also intercept it to use it on its own.

### Docs

HTML Guide and form structure
* [MDN HTML Forms Guide](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Forms)
* [MDN How to Structure an HTML Form](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Forms/How_to_structure_an_HTML_form)

### Form Basics: Inputs and Buttons

So far, we've done an excellent job of displaying information to the user, but we haven't really asked them for their input. HTML also includes a set of elements for building forms.

There is a lot to forms that we'll go into depth in a moment, to start we'll focus on two elements:

- `<input>` creates an input field. `<input>` is like `<img>` in that it does not require or support a closing tag. It can take an optional `type` attribute that helps validate user input in some browsers.
- `<button>` creates a button. `<button>` on the other hand does support a closing tag.

<p data-height="300" data-theme-id="23788" data-slug-hash="MeaMEr" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="Inputs and Buttons" data-editable="true" class="codepen">See the Pen <a href="http://codepen.io/team/turing/pen/MeaMEr/">Inputs and Buttons</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

### Forms: Next Level
Basic input and button elements are a great starting point, but to build a truly usable form we need to use the following base elements:

* `form`
* `label`
* `input`
* `submit`

<p data-height="300" data-theme-id="26495" data-slug-hash="JbyeZM" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="Super Basic HTML Form" data-editable="true" class="codepen">See the Pen <a href="http://codepen.io/team/turing/pen/JbyeZM/">Super Basic HTML Form</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

## Your Challenges (2)

### Part One:
Partner up and answer the following questions:

* What is the attribute `for` indicate on the `label` element? Do you always have to use it? Why or why not?
* What are 5 values for the `type` attribute of an `input` element and how do they work?
* What is the significance of the `name` attribute in a form?
* What is a `fieldset` element?
* Why would a `legend` element be important?

### Part Two:
Copy the form code below into your own Pen, and then refactor as follows:

* Validate for email type
* Add a set of radio buttons with at least three options - only allowing one to be selected at a time
* Include placeholders for name, email, and message
* Add a drop down for favorite color with at least three options
* Use an input for submit instead of a button

<p data-height="458" data-theme-id="26495" data-slug-hash="Lbjgwy" data-default-tab="html,result" data-user="turing" data-embed-version="2" data-pen-title="Basic HTML Form" data-editable="true" class="codepen">See the Pen <a href="http://codepen.io/team/turing/pen/Lbjgwy/">Basic HTML Form</a> by Turing School of Software and Design (<a href="http://codepen.io/turing">@turing</a>) on <a href="http://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

***

# Additional Resources

* [W3C Markup validation](https://validator.w3.org/#validate_by_uri)
* [Turing HTML Style Guide](https://github.com/turingschool-examples/html)

### For Placement Only (FPO)
"For Placement Only" (FPO) options are placeholder content for use in design layouts. Often, you will find yourself forced to build interfaces before you have content. In such cases, you can use FPO content. There are many options for FPO copy, images, and video on the interwebs. Here are some to get you started:

* [Meet the Ipsums](http://meettheipsums.com/)
* [FPOImg](http://fpoimg.com/)
* [FillMurray](http://www.fillmurray.com/)
* [Lorem Pixel](http://lorempixel.com/)
* [Unsplash](https://unsplash.com/)
* [SampleVideos](http://www.sample-videos.com/)
* [Article with useful sites for free icons, image assets, etc.](https://www.elegantthemes.com/blog/resources/10-of-the-best-places-to-find-free-icons-and-image-assets-online)
