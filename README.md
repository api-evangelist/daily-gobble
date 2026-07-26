# Daily Gobble

Daily Gobble was surfaced as a portfolio company of 500 Global and added to the API
Evangelist network as a stub for enrichment. A 2026-07-20 enrichment pass found no
operating company behind it.

**Status: defunct — no API surface to enrich.**

- `dailygobble.com` is a GoDaddy parked domain (NS `ns61`/`ns62.domaincontrol.com`),
  serving a JavaScript redirect to a `/lander` page. No MX records, no content.
- The parking host answers **HTTP 200 for every path**, including deliberately
  non-existent ones. `/.well-known/*`, `/llms.txt` and `/openapi.json` all return the
  same parking stub. These are soft-200s, not artifacts — a future pass must not
  record them as discovered documents.
- `relevantmobile.com`, the URL carried on the original stub, is **not** Daily Gobble.
  It now serves an unrelated Indonesian-language gambling/SEO spam site. The pointer
  has been removed rather than retained.
- No first-party client libraries found on npm or PyPI.

Operating history, product vertical, and shutdown date remain unverified — web search
was unavailable during this pass. A search-enabled re-run could complete the
historical record, but would not change the no-API-surface finding.
