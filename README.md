# Top YouTube Shorts

An unofficial, browser-only explorer for finding popular YouTube Shorts across selected regional markets and publication periods.

## Features\n\nThe page opens on a default United States / 7-day feed. Use the Filters menu to change the topic, markets, period, ranking, or result depth.\n

- Searches one or more YouTube regional markets only when the visitor asks.
- Filters for Shorts and publication periods, including custom dates.
- Deduplicates videos appearing in multiple regional result sets.
- Sorts by lifetime views, average views per hour since publication, or date.
- Stores no server-side data and performs no scheduled collection.

## Accuracy and data limitations

This application does **not** claim to provide an exhaustive or official leaderboard.

1. YouTube search returns ranked samples, not every matching Short.
2. A region represents a YouTube market, not the creator's nationality or video's origin.
3. Periods describe publication time. Ranking uses current lifetime views, not views gained inside the period.
4. Average views/hour divides lifetime views by age; it is not recent hourly growth.
5. Custom dates post-filter returned results and cannot recover omitted videos.
6. Data comes from YouTube's undocumented InnerTube interface through [YouTube.js](https://github.com/LuanRT/YouTube.js). YouTube changes, experiments, indexing delays, consent screens, location inference, and throttling may affect results.
7. A blank search uses `#shorts`; it is not a neutral worldwide index.

## Development

```bash
npm install
npm run dev
```

This project is not affiliated with or endorsed by YouTube or Google.
