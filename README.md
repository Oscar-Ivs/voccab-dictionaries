# Voccab Stage 1 dictionary assets

Prepared English, Spanish, German and French dictionary data for Voccab.
Release tag: `stage1-2026-10-12`.

This repository/release is for dictionary data. It does not need the Voccab
application source. These are the exact prepared bundles from the completed
11 October 2026 Stage 1 update, preserved without content changes.

| Release asset | Language | Archive bytes |
| --- | --- | ---: |
| simple-v1.zip | Simple English | 2,364,290 |
| es-v1.zip | Spanish | 33,811,386 |
| de-v1.zip | German | 70,309,697 |
| fr-v1.zip | French | 85,214,394 |

Download the four dictionary ZIPs and accompanying checksum/licence files from
this repository's versioned release assets. Keep the ZIPs intact for the Voccab
build preparation step. GitHub's automatically generated source-code downloads
contain repository documentation, not the dictionary bundles.

`manifest.json` records exact archive lengths, SHA-256 checksums, extraction
counts and content hashes. `SHA256SUMS.txt` permits independent checks. The
application pins its own copy of the manifest; it does not trust a newly
downloaded manifest to change what a build accepts. Preserve this release
unchanged. A data update requires a new version and reviewed checksums.

Data comes from the native Wiktionary editions, extracted through
[Kaikki/Wiktextract](https://kaikki.org/dictionary/rawdata.html). The bundles
contain app-specific compacted/indexed data, not the raw source exports.
Definitions and examples have not been automatically rewritten or translated.
Contributor attribution, source links, changes and detailed notices are in
`DICTIONARY-LICENSES.txt`. The adapted dictionary data is distributed under
[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/); this data
licence does not automatically apply to application code.

After the source URL is configured, a clean application build downloads and
verifies these archives before extracting them to the original static paths.
The deployed app serves individual dictionary sections from its own origin.
Keep this versioned release available for future builds and retain a backup.
