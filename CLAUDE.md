# rss-feed

Lightweight, client-first RSS feed reader. Auto-discovers RSS/Atom feeds from website URLs, aggregates articles into a unified timeline, and persists everything in browser localStorage. No backend required.

## Tech Stack

- Next.js 14 (App Router) + TypeScript
- Tailwind CSS
- rss-parser (RSS/Atom parsing)
- cheerio (HTML parsing for feed discovery)
- Browser LocalStorage (persistence)

## Key Directories

| Directory     | Purpose                                    |
|---------------|--------------------------------------------|
| `app/`        | Next.js App Router (pages, API routes)     |
| `components/` | React components (feed sidebar, articles, search, bookmarks) |
| `lib/`        | Utilities (feed discovery, parser, hooks, storage, types) |

## Key API Routes

| Route               | Purpose                        |
|----------------------|--------------------------------|
| `api/discover/route.ts` | Auto-discovers RSS feeds from URLs |
| `api/feed/route.ts`     | Fetches and parses feeds (5-min cache) |
