Terse Tally is a fork of the Bludit plugin Simple Stats created to avoid extra hits counted when used with [Prefetch Static Pages](https://github.com/stokesman/bludit-prefetch-static-pages). It also happens to avoid missed counts when used with [Cachy](https://plugins.bludit.com/plugin/cachy) and [Cache](https://github.com/Krakengr/Bludit/tree/master/cache-plugin). To prevent such miscounts, this plugin does not log a visit during a response as does the original. Instead, it adds markup to the response that, only when rendered by a client, will create the request whose response will log a visit.

## Other changes
- The option to output CSS that the theme or a page can use to display day's visits
- Respects 'Do Not Track' headers
- Some translation keys added/accessed by the settings interface