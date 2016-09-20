Once a month, web developers from across the Mozilla Project get together to talk about our side projects and drink, an occurrence we like to call "Beer and Tell".

There's a [wiki page available][wiki] with a list of the presenters, as well as links to their presentation materials. There's also a [recording available][recording] courtesy of Air Mozilla.

[wiki]: https://wiki.mozilla.org/Webdev/Beer_And_Tell/2016/September
[recording]: https://air.mozilla.org/webdev-beer-and-tell-september-2016/

## emceeaich: Gopher Tessel
First up was [emceeaich][], who shared [Gopher Tessel][], a project for running a [Gopher][] server (an Internet protocol that was popular before the World Wide Web) on a [Tessel][]. Tessel is small circuit board that runs [Node.js][] projects; Gopher Tessel reads sensors (such as the temperature sensor) connected to the board, and exposes their values via Gopher. It also can control lights connected to the board.

[emceeaich]: https://mozillians.org/en-US/u/emceeaich/
[Gopher Tessel]: https://github.com/emceeaich/gopher-tessel
[Gopher]: https://en.wikipedia.org/wiki/Gopher_(protocol)
[Tessel]: https://tessel.io/
[Node.js]: https://nodejs.org/en/

## groovecoder: Crypto: 500 BC - Present
Next was [groovecoder][], who shared a preview of a talk about cryptography throughout history. The talk is based on ["The Code Book" by Simon Sign][codebook]. Notable moments and techniques mentioned include:

- 499 BCE: Histiaeus of Miletus shaves the heads of messengers, tattoos messages on their scalps, and sends them after their hair has grown back to hide the message.
- ~100 AD: Milk of tithymalus plant is used as invisible ink, activated by heat.
- ~700 BCE: [Scytale][]
- 49 BC: [Caesar cipher][]
- 1553 AD: [Vigenère cipher][]

[groovecoder]: https://mozillians.org/en-US/u/groovecoder/
[codebook]: https://en.wikipedia.org/wiki/The_Code_Book
[Scytale]: https://en.wikipedia.org/wiki/Scytale
[Caesar cipher]: https://en.wikipedia.org/wiki/Scytale
[Vigenère cipher]: https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher

## bensternthal: Home Monitoring & Weather Tracking
[bensternthal][] was up next, and he shared his work building a dashboard with weather and temperature information from his house. Ben built several Node.js-based applications that collect data from his home weather station, from his [Nest][] thermostat, and from [Weather Underground][] and send all the data to an [InfluxDB][] store. The dashboard itself uses [Grafana][] to plot the data, and all of these servers are run using [Docker][].

The repositories for the Node.js applications and the Docker configuration are available on GitHub:

- [grafana-influxdb-docker](https://github.com/bensternthal/grafana-influxdb-docker)
- [wunderground-influxdb](https://github.com/bensternthal/wunderground-influxdb)
- [nest-influxdb](https://github.com/bensternthal/nest-influxdb)
- [tfws-influxdb](https://github.com/bensternthal/tfws-influxdb)

[bensternthal]: https://mozillians.org/en-US/u/bensternthal/
[Nest]: https://nest.com/
[Weather Underground]: https://www.wunderground.com/
[InfluxDB]: https://www.influxdata.com/
[Grafana]: http://grafana.org/
[Docker]: https://www.docker.com/

## craigcook: ByeHolly
Next was [craigcook][], who shared a [virtual yearbook page][] that he made as a farewell tribute to former-teammate Holly Habstritt-Gaal, who recently took a job at another company. The page shows several photos that are clipped at the edges to look curved like an old television screen. This is done in CSS using [clip-path][] with an [SVG][]-based path for clipping. The SVG used is also defined using proportional units, which allows it to warp and distort correctly for different image sizes, as seen by the variety of images it is used on in the page.

[craigcook]: https://mozillians.org/en-US/u/craigcook/
[virtual yearbook page]: http://craigcook.github.io/etc/byeholly/
[clip-path]: https://developer.mozilla.org/en-US/docs/Web/CSS/clip-path
[SVG]: https://developer.mozilla.org/en-US/docs/Web/SVG

## peterbe: react-buggy
[peterbe][] told us about [react-buggy][], a client for viewing Github issues implemented in [React][]. It is a rewrite of [buggy][], a similar client peterbe wrote for Bugzilla bugs. Issues are persisted in [Lovefield][] (a wrapper for IndexedDB) so that the app can function offline. The client also uses [elasticlunr.js][] to provide full-text search on issue titles and comments.

[peterbe]: https://mozillians.org/en-US/u/peterbe/
[react-buggy]: https://github.com/peterbe/react-buggy
[React]: https://facebook.github.io/react/
[buggy]: http://buggy.peterbe.com/
[Lovefield]: https://github.com/google/lovefield
[elasticlunr.js]: http://elasticlunr.com/

## shobson: tic-tac-toe
Last up was [shobson][], who shared a small [Tic-Tac-Toe][] game on the [viewsourceconf.org][] offline page that is shown when the site is in offline mode and you attempt to view a page that is not available offline.

[shobson]: https://mozillians.org/en-US/u/stephaniehobson/
[Tic-Tac-Toe]: https://viewsourceconf.org/offline/
[viewsourceconf.org]: https://viewsourceconf.org/

---

If you're interested in attending the next Beer and Tell, sign up for the [dev-webdev@lists.mozilla.org mailing list][mailing-list]. An email is sent out a week beforehand with connection details. You could even add yourself to the wiki and show off your side-project!

See you next month!

[mailing-list]: https://lists.mozilla.org/listinfo/dev-webdev
