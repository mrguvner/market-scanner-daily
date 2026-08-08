# MarketScanner daily exports

The client-facing market dataset is published as compressed JSON:

- `latest.meta.json` describes the current file, row count, schema, and SHA-256.
- `latest.json.gz` is the current complete daily dataset.
- `archive/market-YYYY-MM-DD.json.gz` contains each dated dataset.

Private craft listings use a parallel schema so existing item-market clients
remain compatible:

- `latest-craft.meta.json` describes the current private-craft feed.
- `latest-craft.json.gz` contains `craft_observations`.
- `archive/craft-YYYY-MM-DD.json.gz` contains each dated craft dataset.

Plain CSV scanner inputs and local synchronization state are excluded from Git.
Gzip discourages casual browsing and reduces repository/download size; it is not encryption.
