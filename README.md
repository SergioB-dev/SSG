# Static Site Generator

We will be learning the programming language `Rust` by building a
`Static Site Generator`

This project is aimed towards developers that are just starting out with the
language, as such we will be working gradually towards our end goal of a fully
functional `SSG`. We will be introducing ourselves into the project by learning
ohw to make a `lexer` and a `parser` for injecting data into `HTML` files. We
will cover `encoding/decoding` files (this should allow us to get to grips with
how file management works in `Rust`).

Finally, this is project is merely for educational purposes for now, should the
project gain more contributors & features develop into more robust ones, we
could potentially focus on a proper production level application.

## What is a Static Site Generator?

According to
[Cloudflare](https://www.cloudflare.com/en-gb/learning/performance/static-site-generator/#:~:text=A%20static%20site%20generator%20is,to%20users%20ahead%20of%20time.),
a `Static Site Generator` is defined as the following:

> A static site generator is **a tool that generates a full static HTML website
> based on raw data and a set of templates**. Essentially, a static site
> generator automates the task of coding individual HTML pages and gets those
> pages ready to serve to users ahead of time

This means that an end user can build a site (be it a blog, etc) with their
preferred language of choice (Javascript, Rust or even Markdown) & the tool will
process that file into a legit `HTML` syntax.

## What will we be doing?

A `Static Site Generator` can have any number of features. For our
implementation, we will be trying to get the following:

- HTML Template Engine (via JSON Objects)
- Markdown to HTML Parser
-

### HTML Template Engine

A definition that can be found to best describe a `Template Engine` can be
pulled from wiki:

> A **template processor** (also known as a **template engine** or **template
> parser**) is [software](https://en.wikipedia.org/wiki/Software "Software")
> designed to combine templates with a
> [data model](https://en.wikipedia.org/wiki/Data_model "Data model") to produce
> result
> documents.[[1]](https://en.wikipedia.org/wiki/Template_processor#cite_note-Niemeyer000-1)
> [[2]](https://en.wikipedia.org/wiki/Template_processor#cite_note-Manolescu000-2)
> [[3]](https://en.wikipedia.org/wiki/Template_processor#cite_note-Fowler000-3)
> The language that the templates are written in is known as a **template
> language** or **templating language**

Popular template engines such as [Handlebars](https://handlebarsjs.com/),
[Pugs](https://pugjs.org/api/getting-started.html), &
[Mustache](https://mustache.github.io/) allow developers to dynamically inject
data into HTML documents via their APIs. An example could be a Blog site, where
a user needs to populate the page with links to blog articles that are saved on
an external server. These HTML files will have special syntax to let the engine
know where in the document to populate the data. This is what we will be aiming
to create as part of the overall project.

### Markdown to HTML

Markdown is a lightweight markup language that you can use to add formatting
elements to plain text text documents. HTML is the language of the internet. It
can be a little more complex and verbose everything, from headers, to images
must be wrapped in tags. Apart of this generator will be to give the end user
the ability to write in Markdown and compile it into usable HTML.
