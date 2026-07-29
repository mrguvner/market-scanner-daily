# MarketScanner daily exports

This public repository contains only GPG-encrypted CSV exports (`*.csv.gpg`).
Plaintext CSV files are intentionally excluded from Git.

To decrypt a file locally with GPG:

```powershell
gpg --output market.csv --decrypt market.csv.gpg
```

GPG will prompt for the encryption password.
