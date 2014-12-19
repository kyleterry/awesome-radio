# Contributing

These are the contributing guidlines:

* To add to this list, you must fork, edit and submit a pull request.
* To remove an item from this list, you must open and issue explaining why it
  needs to be removed.

## Quality Standard

* Links and information must be useful to the community.
* Make sure there aren't a bunch of broken links
* Stick to the format outlines below as much as you can

## Formating Sections

Here is the markdown template for formating a new or existing section:

```markdown
## Radio Type

Here lies introductory information about that type of radio.

### General Use

How is this radio used and can we use it as citizens?

### Links

* [Link title](https://example.com) - [optional text describing the link]
* [Keep it bulleted](http://example.com)

### Additional Sections Related

These additional sections can be used to describe a feature or installation
process. For instance, in CB, I made a section on SWR since it's so vital to
operating a CB radio.
```

Section headlines are h2 (##). Sub headers related to that section are h3 (###).

For readability, please wrap lines at around 80 characters. Most browser will do
this for you, but a lot of people use `less` to read Markdown. I set `vim` to
automatically do this for me with `au BufRead,BufNewFile *.markdown,*.md,*.txt
setlocal spell textwidth=80`.
