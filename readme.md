# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

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

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
Tag 1 is an image tag, which displays the image linked in the "src" (source) location, and if the image won't display, displays the "alt" (alternate) description.
Tag 2 is a "div", or container, that lets you divide your website up into different areas to do different things.
```

---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Inline CSS hard-codes your style/CSS into your HTML, and is the least preferable.
Internal style sheets link your HTML file with a separate CSS file where you make your changes, and allows you to keep all your style changes to a certain element, class, or ID in one spot.
External style sheets allow you to quickly use a pre-set style sheet, and quickly add style and polish to your document.
```

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* will turn your "box" div into a spherical or oval div */
div {
  border-radius: 50%;
}

/* gives paragraphs that are children of the class "header" an 18pixel font-size */
.header p {
  font-size: 18px;
}

/* gives your elements with class "footer" a fixed (absolute) position, and a bottom of 0 */
.footer {
  position: absolute;
  bottom: 0;
}

/* Gives elements with class "splash-image" a background image, tells it to cover the whole element, and gives it a width of the entire page*/
.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}

/* Changes elements with the class "ninja:hover" to display nothing, and have a color of black*/
.ninja:hover {
  display: none;
  color: black;
}
```

