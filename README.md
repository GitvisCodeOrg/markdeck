# markdeck - presentations as code</br>

author cool slide decks, text-only, offline-ready, collaborative


## why?

* converts markdown to a clean html5 slide deck
* cool looking: based on battle-proven web frameworks, like reveal.js
* no uplink required, neither when authoring, nor presenting:</br>
    no awkward moments during presentation (no "I am still waiting for the Internet, sorry!")
* all batteries included: live renderer, pdf output, asciiart-converter
* text-only, easy syntax: just markdown
* fast-n-easy to write: bring your own editor!
* easy to collaborate-n-reuse: text-only, so bring your own VCS
* eye-candy: supports unicode, emojis, fontawesome, asciiart, math, charts, code highlighting,
    recorded terminal sessions, ...
* self-documenting [documentation slides](DOCUMENTATION.md#self-documenting-documentation-slides):</br>
    see the slide source and the result, side-by-side

You can also visit the shiny [landing page](https://arnehilmann.github.io/markdeck/)
or the [showcase](https://arnehilmann.github.io/markdeck/showcase/).


## install markdeck, tl;dr

You need `bash`, `curl`, `docker-compose` and an empty directory, then run the following command:
```
curl https://raw.githubusercontent.com/arnehilmann/markdeck/master/scaffold | bash
```

This will download a minimal setup, download all needed docker images,
then markdeck gets started...

Use `Ctrl-C` to stop markdeck, and `./start`, `./stop` or `./update-markdeck` to do the suitable things.


## documentation

... can be found in [DOCUMENTATION.md](DOCUMENTATION.md)


## how to start from scratch

```
mkdir my-slides && cd my-slides
curl -O https://raw.githubusercontent.com/arnehilmann/markdeck/master/scaffold
./scaffold
```

```
open http://localhost:8080
```

```
# edit slides.md, add assets/, consult documentation, ...
```


## how does this work

*markdeck* takes ```slide-*.md``` files in markdown format
and the assets subdir
and renders a html5 slidedeck, using [pandoc](http://pandoc.org) as converter
and [reveal.js](http://lab.hakim.se/reveal-js/) as the presenter framework.

see the
[side-by-side view](https://arnehilmann.github.io/markdeck/showcase/explain.html),
to get an idea how markdeck works and looks like, or have a look
at the [documentation](DOCUMENTATION.md).


## based on

[markdown](https://daringfireball.net/projects/markdown/syntax),
[pandoc](https://pandoc.org/),
[reveal.js](https://revealjs.com/#/),
[plantuml](http://wiki.plantuml.net/site/index),
[ditaamini](http://ditaa.sourceforge.net/),
[asciitosvg](https://github.com/dhobsd/asciitosvg),
[graphviz](https://www.graphviz.org/),
[asciinema](https://asciinema.org/),
[decktape](https://github.com/astefanutti/decktape), 
[vega-lite](https://vega.github.io/vega-lite/),
[mathjax-pandoc-filter](https://www.npmjs.com/package/mathjax-pandoc-filter), and
[font-awesome](https://fontawesome.com/).


## known issues

* custom layout hard, but possible
* pixel-perfect layout nearly impossible
* see the [todos](TODOS.md)


## similar projects

* http://bigsense.github.io/
* http://slideshow-s9.github.io
* https://github.com/FormidableLabs/spectacle
* https://github.com/divshot/markdeck
* https://github.com/jxnblk/mdx-deck
* https://github.com/munen/p_slides
* https://github.com/regebro/hovercraft
* https://github.com/sinedied/backslide
* https://gitpitch.com/
* https://godoc.org/golang.org/x/tools/cmd/present
* https://www.deckset.com/
* https://yhatt.github.io/marp/

### Code Visualization:

Here is a cool visualization of the code evolution

 [![Watch the video](https://img.youtube.com/vi/R6lO7N7pgkk/0.jpg)](https://www.youtube.com/watch?v=R6lO7N7pgkk)

 [https://www.youtube.com/watch?v=R6lO7N7pgkk](https://www.youtube.com/watch?v=R6lO7N7pgkk)

