# Top YouTube Shorts

A browser-only, full-screen feed of ten popular YouTube Shorts.

## Interaction

- Opens immediately on a worldwide approximation of the most-viewed Shorts published in the last seven days.
- Plays automatically (muted, as required by browser autoplay rules), advances when a Short ends, and loops the ten-video feed.
- Swipe up/down to move through the feed.
- Swipe right to save a video locally.
- Swipe left to hide a video permanently on that device.
- Move above the first feed video to browse saved videos, newest save first.
- Skip at least two videos within ten seconds to reveal search.
- Repeating the same search cycles through: 7 days, 1 month, 6 months, 1 year, all time, then back to 7 days.
- Search-period cycling is session-only. Saved and hidden videos persist in localStorage.
- Desktop equivalents: arrow down/up navigate; arrow right saves; arrow left hides. Double-click opens search.

## Accuracy and data limitations

This is an unofficial discovery feed, not an exhaustive or official global leaderboard.

1. YouTube search returns ranked samples, not every matching Short.
2. “Worldwide” merges samples from several large YouTube regional markets, deduplicates them, and ranks the returned videos.
3. Periods describe publication time; ranking uses current lifetime views, not views gained during that period.
4. YouTube's search filters do not expose an exact six-month window. The six-month pass is therefore an approximation drawn from the one-year result pool.
5. A blank search uses `#shorts`; it is not a neutral worldwide index.
6. YouTube indexing, experiments, location inference, throttling, and consent behavior can change results.
7. The app uses YouTube's undocumented InnerTube interface via [YouTube.js](https://github.com/LuanRT/YouTube.js), which can break when YouTube changes it.
8. Videos are embedded from YouTube and are never downloaded or rehosted.

No backend, scheduled collection, account, or server-side database is used.

This project is not affiliated with or endorsed by YouTube or Google.
