# Astro Cloudflare CMS — Reference Content

This is the content-only sibling repository for
[Astro Cloudflare CMS](https://github.com/lmaung/Astro-Cloudflare-CMS).

It contains structured page content, configuration, and future site media. It
must not contain application logic, API handlers, UI components, build tooling,
or credentials.

## Local pairing

Clone the repositories as siblings:

```text
~/Repos/
  astro-boilerplate-cms/
  astro-boilerplate-cms-content/
```

The frontend validates `content-manifest.json` and reads page data from `pages/`.
Each page uses a permanent safe slug and a `published` or `archived` lifecycle
state. Navigation order is stored independently under `globals/`, so published
pages may remain intentionally unlisted. Local CMS saves update files atomically
and do not create Git commits; deployed CMS saves create validated content-only
commits without redeploying the frontend.

## Licensing

Original example content, configuration, and metadata in this repository are
dedicated to the public domain under [CC0 1.0 Universal](LICENSE).

CC0 does not grant trademark, patent, privacy, publicity, or third-party rights.
Files listed in [ASSET-LICENSES.md](ASSET-LICENSES.md), or carrying their own
license notice, are governed by those separate terms. Do not assume that future
customer content or media is CC0 merely because it uses this repository format.

## Contributions

See [CONTRIBUTING.md](CONTRIBUTING.md). Do not submit customer content,
personally identifiable information, secrets, or assets you cannot dedicate or
license for redistribution.
