# Intro to Coding: HTML and CSS

### Learning Objectives
- Get familiar with popular, browser-based tools
- Learn the basics of HTML and CSS
- Apply what you learn to a live webpage
- See what remote learning at GA is all about

## Intro
Welcome to SEI! During tonight's info session we are going to build a simple website on Codepen.io using HTML and CSS. This session is meant to provide you with a taste of what one of our SEI classes feels like in a remote format. Since you're just getting started, we'll use web-based tools to learn but know that as a student of the Software Engineering Immersive we will help you set up and learn using industry-standard software and tools.

Let's see what we're going to build. Check it out [here](http://intro-to-html-css.surge.sh/)

## Three Essential Ingredients
Three languages are responsible for every website that we visit: HTML, CSS, and Javascript. Tonight we'll focus on HTML and CSS with the majority of our time spent on CSS.

Broadly, let's think of HTML as **defining the structure and content of the page** and let's think of CSS as **providing the style of the page**.

Javascript is a major player and needs to be mentioned but we won't have time to dive into it tonight. Rest assured that it will be the primary focus of 9 out of 12 weeks in SEI.

### Tools
To build this site we'll be using two tools:
1. Codepen.io
  - it's free
  - provides an in-browser code editor
  - renders code instantly
  - lots of developers actively use it
2. A modern web browser (Google Chrome or Firefox are great choices)
  - both are free
  - both provide a comprehensive suite of developer tools

### Getting Started
1. Sign up and sign in to [codepen.io](http://codepen.io)
2. [Click this link](https://codepen.io/ZakkMann/pen/KRRqre?editors=1010) to open a pen that we've added some starter code to
3. In the top right menu, click "Fork" (this copies the codepen contents into a pen that you own and can change)

## HTML
HTML provides the structure and content for any web page. It does this using "elements" that describe what type of content needs to be displayed (a heading, paragraph, image, etc) and what that content is (the words of the heading or paragraph, a URL for the image, etc).

### Typical Tags
A typical HTML tag looks like this:

```html
<p>This text will be formatted as a paragraph and rendered to the page</p>
```

Notice the opening and closing tag that **wraps** the content to be displayed. Most elements will have both an opening and closing tag but some will "self close". Take a look:

```html
<img src="picture.jpg" />
```

An `img` tag doesn't need to wrap around any content because the content is provided by the `src` attribute. Wait, "attribute"? What's that?

### HTML Attriibutes
Attributes allow us to provide additional contextual information to our HTML elements. In the example above we see an attribute that provides content to be rendered to the page but sometimes attributes are used just to store stuff. It may be a class, it may be a piece of data, or, in the case of an anchor tag a link to an outside source.

```html
<a href="http://google.ca">Click me!</a>
```

Attributes follow a consistent format of key-value pairs like this: `attributeName="someValueWeProvide"`

### The HTML Shell
At its most basic, our HTML files will include the following code structure:

```html
<!DOCTYPE html>
<html>
  <head>
    <title></title>
  </head>
  <body>
    
  </body>
</html>
```

HTML has a very hierarchical structure and we represent that hierarchy by indenting the different elements and tags when they're enclosed by another.

Things to notice about this baseline structure:
- `<html>`: wrap around everything
- `<head>`: appears at the top of the file and contains meta information about the page like a title, or external files that need to be loaded. The contents of this tag are never rendered to the browser in a way that's visible to users (with one exception, do know it?)
- `<body>`: this is where a lot of the action will happen. We'll add additional tags here and they'll be ones visible to our users.

### Let's Get Coding
This has been a good introduction to HTML but to really get it, let's write some in our codepen.

### We do: Add Header, Main, and Footer
1. Within the body tag of your HTML file, add the following elements (type out the elements but feel free to copy and paste their contents):

```html
<header>
  <img src="https://brightcove04pmdo-a.akamaihd.net/5104226627001/5104226627001_5244714388001_5205235439001-vs.jpg?pubId=5104226627001&amp;videoId=5205235439001">
</header>

<main>
  <h1>Visit New York!</h1>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque placerat, sapien non lacinia consequat, massa just dictum lorem, pharetra rutrum purus sapien eget nunc. Proin ullamcorper euismod ex semper condimentum. Curabitur mattis dapibus eros at fringilla. Curabitur quis tempus sem. Mauris orci arcu, ultricies nec velit non, eleifend sagittis nunc. Nam eget massa in magna commodo volutpat at nec felis. Pellentesque sit amet semper justo, molestie pulvinar nunc. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Quisque gravida rhoncus ligula necultrices. Vivamus sit amet porta nisi. Vivamus lectus eros, iaculis non tellus at, finibus hendrerit felis.
  </p>
</main>

<footer>Copyright General Assembly</footer>
```

2. Make sure that your content is rendering in Codepen.

### You do: Add the remaining content. (10 min)
The best way to learn how to code is to do it for yourself and build your experience level. Now that you've seen a basic walkthrough, practice that skill by adding in the remaining two content sections to the `<main>` element. If you need help, don't be afraid to ask!

Once you're done with that, we're ready to talk CSS and this page certainly needs a lot of it.

## CSS
How do we describe CSS? CSS provides that style and visual interest that keeps our users' attention. HTML by itself is boring and hard to look at but we can change that.

Let's take a look at a page with and without CSS to get an idea of how important this language is.

### Basic Syntax

A CSS rule is made up of three parts: the selector, the declaration block (`{}`), and one or many declarations.

```css
selector {
  declaratioonProperty: declarationValue
}
```

A more real world example might look like this:

```html
<h1>I love Learning!</h1>
```

```css
h1 {
  color: red;
}
```

This CSS Rule:
- selects all `<h1>` elements
- declares that `<h1>` element text will be `red`

### Selectors, selectors, selectors
We're not limited to selecting HTML elements using their tag name, we can also select using a class like so:

```html
<h1 class="title">Hello World!</h1>
<p class="title">This is a title too</h1>
```

```css
.title {
  font-size: 40px;
  font-family: sans-serif
}
```

We select the class using "dot notation". In other words, we will select all elements with the class of title and apply the same set of style rules to each.

### CSS is Hard

See Peter Griffin GIF.

### Let's style it up
The CSS pane of your codepen will have some prompts for which CSS rules go where. We'll build out as many as we have time for and will leave the rest up to you.

## Conclusion
There you have it! An Intro to HTML and CSS is really just scratching the surface of modern web development. In SEI, we'll have the time and space to go wider and deeper into each topic and on the other side you'll not only be able to write pages like this one in your sleep, you'll be able to do quite a bit more. Happy coding! 
