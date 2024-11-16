# django-htmx-tag-search
This is a package designed to abstract a search-tag feature for multi-input inspired by [Shoelace.style's select multiple input](https://shoelace.style/components/select/#multiple)

I liked the methodology, but  I wanted it to work with HTMX and I found it to be more work than it was worth to do with javascript so I made the searching and adding piece to be done with HTMX.

I am by no means a front-end dev, but it seems to work the way I want so far. Would love all the help I can get (Including with this readme) as this is my first project I want to give back to the community with.

The goal behind this is to make it as easy as possible to integrate into your own forms

# Requirements
HTMX


# How does it work?

1. User searches into an input text field
2. The input field does an Async request to respond with the model you want queried
3. The user selects an option for the input field
4. It triggers a different view that will get the model's ID, the Model's value and return a tag with an "x" to remove it
5. The element appears with 2 values
   a. A div with a span for the actual text
   b. A hidden input that is the true value (This is what _actually_ gets submitted to the server


# Todo
- [ ] Add an option to remove the field from the dropdown if the dev doesn't want it selectable again
- [ ] Make it work as a multi-select or not
