Once a month, web developers from across the Mozilla Project get together to
talk about our side projects and drink, an occurrence we like to call "Beer and
Tell".

There's a [wiki page available][wiki] with a list of the presenters, as well as
links to their presentation materials. There's also a [recording
available][recording] courtesy of Air Mozilla.

[wiki]: https://wiki.mozilla.org/Webdev/Beer_And_Tell/February_2016
[recording]: https://air.mozilla.org/webdev-beer-and-tell-20160219/

## Bruce Banner: Web Developer
[shobson][] was up first with [Bruce Banner: Web Developer][], a small webcomic
generator. It provides sweet relief from those workplace stressors via the
violent justice of The Incredible Hulk. The idea came from [willkg][], the code
from shobson, and the art from [craigcook][]. Excelsior!

[shobson]: https://mozillians.org/en-US/u/stephaniehobson/
[Bruce Banner: Web Developer]: http://stephaniehobson.github.io/bbwd/
[willkg]: https://mozillians.org/en-US/u/willkg/
[craigcook]: https://mozillians.org/en-US/u/craigcook/

## Dokku + Let's Encrypt
Next up was [pmac][], who showed off [dokku][], a small PaaS implementation
similar to [Heroku][], that uses [Docker][] containers. Not only is it
convenient for running several apps on a single server, but there is also a
plugin called [dokku-letsencrypt][] that lets you automatically retrieve and
install TLS certificates from [letsencrypt.org][]. Easy peasy!

[pmac]: https://mozillians.org/en-US/u/pmac/
[dokku]: http://dokku.viewdocs.io/dokku/
[Heroku]: https://heroku.com/
[Docker]: https://www.docker.com/
[dokku-letsencrypt]: https://github.com/dokku/dokku-letsencrypt
[letsencrypt.org]: https://letsencrypt.org/

## RPG Maker MV
Next was [Osmose][] (that's me!) who talked about [RPG Maker MV][], the latest
entry in the RPG Maker series of game-making tools. Interestingly, RPGMV uses
HTML and JavaScript to implement the engine used to run games made with it. The
application itself edits JSON files that are loaded by the web-based engine. The
engine itself uses [pixi.js][] for rendering, and can be extended via plugins
written in JavaScript.

[Osmose]: https://mozillians.org/en-US/u/Osmose/
[RPG Maker MV]: http://www.rpgmakerweb.com/
[pixi.js]: http://www.pixijs.com/

## Battleshits
[peterbe][] stopped by to share [Battleshits][], a mobile-friendly web app and a
fairly gross version of the popular boardgame Battleship. The game connects you
with other players via WebSockets and [Fanout][], and most of the interface is
implemented using [React][].

[peterbe]: https://mozillians.org/en-US/u/peterbe/
[Battleshits]: https://btlsh.it/
[Fanout]: https://fanout.io/
[React]: https://facebook.github.io/react/

## Chava
Last up was [jpetto][] with a small personal project memorializing his local
coffeeshop, [Chava][], which closed earlier this year. The page uses
[Hammer.js][] for touch events and [LazyLoad][] to lazily load the images, but
the lightbox implementation is custom-made from scratch. Neato!

[jpetto]: https://mozillians.org/en-US/u/jpetto/
[Chava]: http://chava.equalparts.io/
[Hammer.js]: http://hammerjs.github.io/
[LazyLoad]: http://verlok.github.io/lazyload/

---

If you're interested in attending the next Beer and Tell, sign up for the
[dev-webdev@lists.mozilla.org mailing list][mailing-list]. An email is sent out
a week beforehand with connection details. You could even add yourself to the
wiki and show off your side-project!

See you next month!

[mailing-list]: https://lists.mozilla.org/listinfo/dev-webdev
