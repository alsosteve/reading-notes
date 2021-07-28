# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
code fellows 102

## Read: 04 - Structure web pages with HTML

### Wire Frame

A __*Wire frame*__ is a drawn out plan for a website, a blueprint if you will.  Programers use this to preplan out a website before they create one. Examples of wire frame include:
* pen and paper drawings
* web based drawing apps
* drawing apps
* picture boards

When you make a wire frame you should consider who may see or use it. You should make it clear concise, and simple. The best tools for wireframing are the free ones. Nobody likes to waste money. Not even Jeff Bezos. 

Some free stuff:
* [uxpin](https://www.uxpin.com/)
* [invision](https://www.invisionapp.com/)
* [wirefram.cc](https://wireframe.cc/)

Before you start you should:
1. Do your research
2. Look for quick references
3. Map out a user flow chart
4. Sketch it out
5. Make details and test them out
6. Prototype it

### HTML

__*HTML*__ stands for hypertext markup language. I know, that's 2 words not 4... Everything you type into a html file needs to be contained. How you ask, well I'm glad you asked. Evements and text need to be contained in tags. An opening and closing one. it looks like this

![example of tag](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)


#### Here are some tags
| Tags | Description |
| --- | --- |
| <p> | text |
| <strong> | strongly empasize text |
| <img src="images/firefox-icon.png" alt="My test image"> | image from a webpage |

A basic completed page should look like this:

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="My test image">
  </body>
</html>

#### To make a tag you do this:

<ul>
  <li>technologists</li>
  <li>thinkers</li>
  <li>builders</li>
</ul>

#### A link looks like this:

<a href="https://www.mozilla.org/en-US/about/manifesto/">Mozilla Manifesto</a>

#### More Tags
<article>
<aside>
<details>
<figcaption>
<figure>
<footer>
<header>
<main>
<mark>
<nav>
<section>
<summary>
<time>
<h1>