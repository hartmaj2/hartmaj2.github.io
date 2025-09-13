# Good resources for jekyll 

## Jekyll variables

- list of variables that can be used in jekyll by Liquid templating language
  - [link](https://jekyllrb.com/docs/variables/)

- one can do magic with them, for example automatically generate the navbar by looping through all pages `site.pages` and using their `page.title` and `page.url` values

## Permalinks

- [link](https://jekyllrb.com/docs/permalinks/)

- allow the internal folder structure to be different than the resulting rendered page

## Liquid templating language

- basics
  - [link](https://shopify.github.io/liquid/basics/introduction/)

- control flow
  - [link](https://shopify.github.io/liquid/tags/control-flow/)

## Technical site details

### Latex rendering

- for Latex rendering, we put `<script async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"> </script>` in the head of the layout html
  - `async` means that the script does not block rendering of the rest of the HTML document
  - CDN (Content Delivery Network) - delivers content from the nearest source to me using the same piece of code for everybody

### Top navbar

The top navbar can be found in `_includes/navigation.html`. The best feature of this navbar is, that it is created automatically using a for loop (written in liquid templating language) that goes through all pages in the sections.