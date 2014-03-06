### [CoffeeKup Optimization][1] [&para;](#coffeekup-optimized)

Back when I was getting to know [CoffeeScript][2], I loved it so much I wanted
to use it for everything, including frontend templates. I found [CoffeeKup][3],
which seemed to offer everything I was looking for - not quite as nice looking
as [Jade][4], but it meant I could write my whole project, front-to-back, in the
*same language*.

The only problem was, it was a bit slow. Frontend pages need to be fast, and
slow templates can make things unresponsive... ah who am I kidding, it was fast
enough, I just got caught up in some serious premature optimization. So much
fun!

The idea was to compile the templates to javascript, do some static analysis of
the resulting code with [uglify-js][5], and move things around so that as much
as possible of the work that CoffeeKup was doing at run time was done at compile
time. The results were [pretty good][6].

[1]: https://github.com/mauricemach/coffeekup/pull/87
[2]: http://coffeescript.org/
[3]: http://coffeekup.org/
[4]: http://jade-lang.com/
[5]: http://github.com/mishoo/UglifyJS
[6]: http://jsperf.com/coffeekup-optimized/3
