# Technical site details

## Latex rendering

- for Latex rendering, we put `<script async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"> </script>` in the head of the layout html
  - `async` means that the script does not block rendering of the rest of the HTML document
  - CDN (Content Delivery Network) - delivers content from the nearest source to me using the same piece of code for everybody

## Top navbar

The top navbar can be found in `_includes/navigation.html`. The best feature of this navbar is, that it is created automatically using a for loop (written in liquid templating language) that goes through all pages in the sections.

Introduced a variable `navbar_order` which can be added to front matter to control the order of the page in the navbar. The code that does this uses sorting to create a new sorted list of pages with `{% assign nav_pages = site.pages | sort: "title" | reverse | sort: "navbar_order" | reverse %}`

The navbar has two layers. The main navbar and secondary navbar. A page will appear on the main navbar if it has `navbar_order` set to some value.

The secondary navbar appears only for pages which are part of a section with subsections. If that is so, the page has to have `section_key` set.

## Blogposts

- `external-link` in the front matter allows a redirect straight to the url provided

# Technical tricks

`where_exp` is like `where` but is written like a general lambda function.