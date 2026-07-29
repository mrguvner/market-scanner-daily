# MarketScanner daily exports

The client-facing market dataset is published as compressed JSON:

- `latest.meta.json` describes the current file, row count, schema, and SHA-256.
- `latest.json.gz` is the current complete daily dataset.
- `archive/market-YYYY-MM-DD.json.gz` contains each dated dataset.

Plain CSV scanner inputs and local synchronization state are excluded from Git.
Gzip discourages casual browsing and reduces repository/download size; it is not encryption.
