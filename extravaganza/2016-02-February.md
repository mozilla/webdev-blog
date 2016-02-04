Once a month, web developers from across Mozilla get together to talk about the
work that we've shipped, share the libraries we're working on, meet new folks,
and talk about whatever else is on our minds. It's the Webdev Extravaganza! The
meeting is open to the public; you should stop by!

You can check out the [wiki page][wiki] that we use to organize the meeting, or
view a [recording of the meeting][recording] in Air Mozilla. Or just read on for
a summary!

[wiki]: https://wiki.mozilla.org/Webdev/Meetings/2016/February_2
[recording]: https://air.mozilla.org/webdev-extravaganza-february-2016/

## Shipping Celebration
The shipping celebration is for anything we finished and deployed in the past
month, whether it be a brand new site, an upgrade to an existing one, or even a
release of a library.

### Git Submodules are Gone from MDN
First up was [jezdez][] with news about [MDN][] moving away from using
[git submodules][] to pull in dependencies. Instead, MDN now uses [pip][] to
pull in dependencies during deployment. Hooray!

[jezdez]: https://mozillians.org/en-US/u/jezdez/
[MDN]: https://developer.mozilla.org/
[git submodules]: https://git-scm.com/book/en/v2/Git-Tools-Submodules
[pip]: https://pip.pypa.io/

### Careers now on AWS/Deis
Next was [giorgos][] who let us know that [careers.mozilla.org][] has moved over
to the Engagement Engineering [Deis][] cluster on [AWS][]. For deployment, the
site has [Travis CI][] build a [Docker][] image and run tests against it. If the
tests pass, the image is deployed directly to Deis. Neat!

[giorgos]: https://mozillians.org/en-US/u/giorgos/
[careers.mozilla.org]: https://careers.mozilla.org/
[Deis]: http://deis.io/
[AWS]: https://aws.amazon.com/
[Travis CI]: https://travis-ci.org/
[Docker]: https://www.docker.com/

### Privacy Day
[jpetto][] helped ship the [Privacy Day][] page. It includes a mailing list
signup form as well as instructions for several platforms on how to update your
software to stay secure.

[jpetto]: https://github.com/jpetto
[Privacy Day]: https://petitions.mozilla.org/stay-secure/

### Automated Functional Testing for Mozilla.org
[agibson][] shared news about the migration of previously-external functional
tests for [mozilla.org][] to live within the [Bedrock][] repository itself. This
allows us to run the tests, which previously were run by the WebQA team against
live environments, whenever the site is deployed to dev, stage, or production.
Having the functional tests be a part of the build pipeline ensures that
developers are aware when the tests are broken and can fix them before deploying
broken features. A [slide deck is available][] with more details.

[agibson]: https://mozillians.org/en-US/u/agibson/
[mozilla.org]: https://www.mozilla.org/
[Bedrock]: https://github.com/mozilla/bedrock/
[slide deck is available]: https://docs.google.com/presentation/d/1j9LdiFR452IgHtfSr7EWpsDtMit-yEOazZZmezSpaI8/edit?usp=sharing

### Peep 3.x
[ErikRose][] shared news about the 3.0 (and 3.1) release of [Peep][], which
helps smooth the transition from Peep to [Pip 8][pip], which now supports hashed
requirements natively. The new Peep includes a `peep port` command for porting
Peep-compatible requirements files to the new Pip 8 format.

[ErikRose]: https://mozillians.org/en-US/u/ErikRose/
[Peep]: https://github.com/erikrose/peep/

## Open-source Citizenship
Here we talk about libraries we're maintaining and what, if anything, we need
help with for them.

### Jazzband
[jezdez][] shared news about [JazzBand][], a cooperative experiment to reduce
the stress of maintaining Open Source software alone. The group operates as a
Github organization that anyone can join and transfer projects to. Anyone in the
JazzBand can access JazzBand projects, allowing projects that would otherwise
die due to lack of activity thrive thanks to the community of co-maintainers.

Notable projects already under the JazzBand include [django-pipeline][] and
[django-configurations][]. The group is currently focused on Python projects and
is still figuring out things like how to secure releases on PyPI.

[JazzBand]: https://jazzband.co/
[django-pipeline]: https://github.com/jazzband/django-pipeline
[django-configurations]: https://github.com/jazzband/django-configurations

### django-configurations 1.0
Speaking of the JazzBand, members of the collective pushed out the 1.0 release
of [django-cofigurations][], which is an opinionated library for writing
class-based settings files for Django. The new release adds Django 1.8+ support
as well as several new features.

## Roundtable
The Roundtable is the home for discussions that don't fit anywhere else.

### Travis CI Sudo for Specific Environments
Next was [ErikRose][] with an undocumented tip for Travis CI builds. As seen on
the [LetsEncrypt travis.yml][], you can specify `sudo: required` for a specific
entry in the build matrix to run only that build on Travis' container-based
infrastructure.

[LetsEncrypt travis.yml]: https://github.com/letsencrypt/letsencrypt/blob/4bafe9695d56dc63951962221b82908ec50b0129/.travis.yml#L51-L54

### Docker on OS X via xhyve
Erik also shared [xhyve][], which is a lightweight OS X hypervisor. It's a port
of [bhyve][], and can be used as the backend for running Docker containers on
OS X instead of [VirtualBox][]. Recent changes that have made this more feasible
include the removal of a 3 gigabyte RAM limit and experimental NFS support that,
according to Erik, is faster than VirtualBox's shared folder functionality.
Check it out!

[xhyve]: https://github.com/mist64/xhyve
[bhyve]: http://www.bhyve.org/
[VirtualBox]: https://www.virtualbox.org/

---

If you're interested in web development at Mozilla, or want to attend next
month's Extravaganza, subscribe to the
[dev-webdev@lists.mozilla.org mailing list][mailing-list] to be notified of the
next meeting, and maybe send a message introducing yourself. We'd love to meet
you!

See you next month!

[mailing-list]: https://lists.mozilla.org/listinfo/dev-webdev
