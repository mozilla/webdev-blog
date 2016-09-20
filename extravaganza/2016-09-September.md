Once a month, web developers from across Mozilla get together to talk about the work that we've shipped, share the libraries we're working on, meet new folks, and talk about whatever else is on our minds. It's the Webdev Extravaganza! The meeting is open to the public; you should stop by!

You can check out the [wiki page][wiki] that we use to organize the meeting, or view a [recording of the meeting][recording] in Air Mozilla. Or just read on for a summary!

[wiki]: https://wiki.mozilla.org/Webdev/Meetings/2016/September
[recording]: https://air.mozilla.org/webdev-extravaganza-september-2016/

## Shipping Celebration
The shipping celebration is for anything we finished and deployed in the past month, whether it be a brand new site, an upgrade to an existing one, or even a release of a library.

### Survey Gizmo Integration with Google Analytics
First up was [shobson][], who talked about a survey feature on [MDN][] that prompts users to leave feedback about how MDN helped them complete a task. The survey is hosted by [SurveyGizmo][], and custom JavaScript included on the survey reports the user's answers back to [Google Analytics][]. This allows us to filter on the feedback from users to answer questions like, "What sections of the site are not helping users complete their tasks?".

[shobson]: https://mozillians.org/en-US/u/stephaniehobson/
[MDN]: https://developer.mozilla.org/en-US/
[SurveyGizmo]: https://www.surveygizmo.com/
[Google Analytics]: https://analytics.google.com/

### View Source Offline Mode
shobson also mentioned the [View Source][] website, which is now offline-capable thanks to [Service Workers][]. The pages are now cached if you've ever visited them, and the images on the site have offline fallbacks if you attempt to view them with no internet connection.

[View Source]: https://viewsourceconf.org/berlin-2016/
[Service Workers]: https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API

### SHIELD Content Signing
Next up was [mythmon][], who shared the news that [Normandy][], the backend service for [SHIELD][], now signs the data that it sends to Firefox using the [Autograph][] service. The signature is included with responses via the
[Content-Signature][] header. This signing will allow Firefox to only execute SHIELD recipes that have been approved by Mozilla.

[mythmon]: https://mozillians.org/en-US/u/mythmon/
[Normandy]: https://github.com/mozilla/normandy
[SHIELD]: https://wiki.mozilla.org/Firefox/SHIELD
[Autograph]: https://github.com/mozilla-services/autograph
[Content-Signature]: https://tools.ietf.org/html/draft-thomson-http-content-signature-00

## Open-source Citizenship
Here we talk about libraries we're maintaining and what, if anything, we need help with for them.

### Neo
[Eli][] was up next, and he shared [Neo][], a tool for setting up new [React][]-based projects with zero configuration. It installs and configures many useful dependencies, including [Webpack][], [Babel][], [Redux][], [ESLint][], [Bootstrap][], and more! Neo is installed as a command used to initialize new projects or a dependency to be added to existing projects, and acts as a single dependency that pulls in all the different libraries you'll need.

[Eli]: https://mozillians.org/en-US/u/eli/
[Neo]: https://github.com/mozilla/neo
[React]: https://facebook.github.io/react/
[Webpack]: http://webpack.github.io/
[Babel]: http://babeljs.io/
[Redux]: http://redux.js.org/
[ESLint]: http://eslint.org/
[Bootstrap]: http://getbootstrap.com/

## Roundtable
The Roundtable is the home for discussions that don't fit anywhere else.

### Standu.ps Reboot
Last up was [pmac][], who shared a note about how he and [willkg][] are re-writing the [standu.ps][] service using [Django][], and are switching the rewrite to use [Github][] authentication instead of [Persona][]. They have a staging server setup and expect to have news next month about the availability of the new service.

Standu.ps is a service used by several teams at Mozilla for posting status updates as they work, and includes an IRC bot for quick posting of updates.

[pmac]: https://mozillians.org/en-US/u/pmac/
[willkg]: https://mozillians.org/en-US/u/willkg/
[standu.ps]: http://www.standu.ps/
[Django]: https://www.djangoproject.com/
[Github]: https://github.com/
[Persona]: https://login.persona.org/

---

If you're interested in web development at Mozilla, or want to attend next month's Extravaganza, subscribe to the [dev-webdev@lists.mozilla.org mailing list][mailing-list] to be notified of the next meeting, and maybe send a message introducing yourself. We'd love to meet you!

See you next month!

[mailing-list]: https://lists.mozilla.org/listinfo/dev-webdev
