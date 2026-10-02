# Crawl discovery notes

How fast does a search crawler find a new page, and which discovery path gets it there first?
This repository keeps the method and public results of a small field test we run on our own domains.

## What is measured

- Time from publication to the first verified crawler request (reverse DNS + forward DNS, never User-Agent alone).
- Time from the first crawl to the page appearing in the index (Search Console URL Inspection).
- Each group of test pages is exposed through exactly one discovery path: XML sitemap via robots.txt, sitemap submitted in Search Console, a WebSub-enabled Atom feed, a link from an established page, a link from a public hub, or a manual indexing request.

## Rules we keep

- Own domains only, one discovery variable per group, a control group that is never exposed.
- No Indexing API for regular pages, no link networks, no hidden links.
- Results are published after at least three clean rounds.

## Public hub of round 2

The hub page lists the notes that belong to the "public hub" group:
https://relay.maxstepanenko.com/hub/oju9c74x6owg

Feed: https://relay.maxstepanenko.com/feeds/oju9c74x6owg/hub.atom

## Status

Round 2 started on 2026-10-02 and runs for 14 days. Results will be added here.
