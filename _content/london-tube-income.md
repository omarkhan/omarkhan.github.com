### [Mind the Gap][1]

Inspired by [this feature in the New Yorker][2], this is my attempt to learn
[d3][3] while grappling with the UK neighbourhood statistics API.

The visualization shows income inequality along London tube lines. My only rule
here was to use *only* d3 (no jquery!). I can confirm that DOM apis are indeed
horrible, and that's without even trying to support IE.

For what it's worth I don't think the d3 api is very nice either, unless you
*really* like lots of chaining. I just don't find long chains of method calls
very readable.

[1]: http://omarkhan.me/london-tube-income/
[2]: http://www.newyorker.com/sandbox/business/subway.html
[3]: http://d3js.org/
