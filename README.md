# Top YouTube Shorts

A browser-only, full-screen feed of ten popular YouTube Shorts.

## First visit

The app asks for the visitor's own YouTube Data API v3 key and links directly to:

- [Create an API key in Google Cloud](https://console.cloud.google.com/apis/credentials)
- [Enable YouTube Data API v3](https://console.cloud.google.com/apis/library/youtube.googleapis.com)

Restrict the key to the YouTube Data API v3 and to the HTTP referrer `https://kakkoidev.github.io/*`. The key is validated, then stored only in that browser's localStorage. It is sent to Google's YouTube Data API and nowhere else.

## Interaction

- Opens on videos published in the last seven days, ordered by lifetime views.
- Plays automatically muted, advances when a video ends, and loops ten results.
- Swipe up/down to move; right saves; left hides permanently on that device.
- Move above the first feed video to browse saved videos, newest save first.
- Skip at least two videos within ten seconds to reveal search.
- Repeating the same search cycles through 7 days, 1 month, 6 months, 1 year, all time, then back to 7 days.
- Search-period cycling is session-only. Saved and hidden videos persist locally.
- Desktop: arrow keys navigate/save/hide; double-click opens search.

## Limitations

This is an unofficial discovery feed, not an exhaustive worldwide leaderboard. YouTube's official API does not expose a definitive Shorts flag, so results are approximated using `#shorts`, short duration, publication date, and view count. Periods describe publication time; ranking uses lifetime views. Each search uses the visitor's API quota, and Google commonly grants 10,000 units per day while a search request costs 100 units.

No backend, scheduled collection, account, or server-side database is used. Videos remain embedded from YouTube.

This project is not affiliated with or endorsed by YouTube or Google.
