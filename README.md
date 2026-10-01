# Listing feeds

Generated ad feeds, served over HTTPS for Meta and Google to pull on a
schedule. **Nothing here is written by hand** — every file is produced by the
daily run in `listing-clients` and force-pushed here.

Served at `https://feeds.redmoon.media/<client>/meta-catalog.csv`

## Why this repo is public

GitHub Pages serves from public repositories on the free plan, and the
contents are MLS listing data that is already public on each client's website.
No configuration, credentials, CRM data or client agreements live here — those
stay in the private `listing-clients` repo.

## Files

| Path | Consumer |
|---|---|
| `<client>/meta-catalog.csv` | Meta catalog scheduled feed |
| `<client>/google-feed.csv` | Google Ads business data feed |

Feed URLs are permanent. When a client changes website platforms, the feed
changes behind the URL and the ad platforms never notice — which is the whole
point of hosting them here rather than linking to a vendor's export.
