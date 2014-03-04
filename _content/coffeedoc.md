### [CoffeeDoc][1]

I *loved* [CoffeeScript][2] when I first discovered it, back when the language
was picking up steam in 2011. I was just getting to grips with javascript, and
coming from python I found the indened, curly-brace free language far more
readable.

I was looking for some tools to generate documentation for a project, and came
across [Docco][3]. It could generate some nice-looking annotated source pages,
and was written by none other than the creator of CoffeeScript. But after
playing around with it I couldn't really see any benefit from generating
annotated source pages - why not just read the source? The comments are in
there.

I needed something that would show useful documentation for complex class
hierarchies spread across multiple files. After some messing about with the
CoffeeScript compiler, I had a working documentation tool.

It relies on a commenting convention based on python docstrings, so it might not
be an ideal fit for existing codebases, but if you're starting a new project and
you have a python background, you might like it. Have a look at [the lovely
wintersmith.io docs][4] to see what it can do.

[1]: https://github.com/omarkhan/coffeedoc
[2]: http://coffeescript.org/
[3]: http://jashkenas.github.com/docco/
[4]: http://wintersmith.io/docs/
