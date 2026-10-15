# InternetUniverseBot

A small personal hobby crawler that maps links between public web pages for a visualization project. It is not a commercial service, and it does not sell or republish page content.

## How it behaves

- Identifies itself as `InternetUniverseBot` in the `User-Agent` header
- Obeys `robots.txt`, including `Crawl-delay`
- Waits at least 2 seconds between requests to the same site
- Makes one request at a time per site
- Only reads public pages, and never logs in or bypasses restrictions
- Stops retrying a site that keeps failing

## Block it

Add this to your site's `robots.txt` and it will stop crawling you:

```
User-agent: InternetUniverseBot
Disallow: /
```

## Contact

To ask me to slow down, remove your site from my index, or ask anything else, [open an issue](https://github.com/miguel20116/internet-universe-bot/issues) on this repo.
