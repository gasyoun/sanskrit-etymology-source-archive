# Sanskrit etymology — Wiktionary source archive

_Independent backup, created 07-11-2026._

A byte-faithful, checksummed snapshot of
[Category:Sanskrit terms by etymology](https://en.wiktionary.org/wiki/Category:Sanskrit_terms_by_etymology)
on English Wiktionary. This repository exists so the source taxonomy survives
if the original page is moved, renamed, vandalised or lost — and so the loss of
the companion Pages site does not take the backup with it.

Live teaching view: <https://gasyoun.github.io/wiki/> ·
Companion archive page: <https://gasyoun.github.io/wiki/archive/>

## Why one page was not enough

The parent category contains **no word pages at all** — only 42
subcategories. A copy of the parent HTML would preserve 42 labels and none of
the vocabulary. This snapshot therefore also captures every direct member one
level down: **5426 titles** in total.

## Contents

| File | What it holds |
| --- | --- |
| `raw/category.html` | Original page as served, unmodified bytes. |
| `raw/category-rendered.json` | Rendered intro text (template-generated, absent from wikitext). |
| `raw/category-wikitext.json` | The full wikitext, `{{auto cat}}`. |
| `raw/subcategories.json` | MediaWiki API listing of the 42 subcategories. |
| `raw/subcategory-members.json` | Each subcategory mapped to its direct children and word pages. |
| `manifest.json` | Source URLs, UTC timestamp, byte sizes and SHA-256 for every raw file. |
| `CHECKSUMS.txt` | Standard `shasum -c` verification file. |
| `SNAPSHOT.md` | Complete human-readable record: all 42 categories, counts, links, descriptions. |

Snapshot id: `sanskrit-etymology-2026-11-07` · taken 2026-11-07T05:14:14Z.

## Verify and restore

```sh
shasum -a 256 -c CHECKSUMS.txt
```

`raw/subcategories.json` gives the authoritative list of the 42 subcategory
titles; `raw/subcategory-members.json` supplies their direct members. Together
they are enough to rebuild the taxonomy one level down without Wiktionary.
The original rendered page is preserved in `raw/category.html` and
`raw/category-rendered.json`.

To refresh, run `wiki/scripts/fetch_snapshot.py` in
[gasyoun/gasyoun.github.io](https://github.com/gasyoun/gasyoun.github.io) and
copy the regenerated `wiki/archive/` contents here.

## Rights

Wiktionary text is available under CC BY-SA; see
[Wiktionary:Copyrights](https://en.wiktionary.org/wiki/Wiktionary:Copyrights).
Category names, counts and structure are reproduced for teaching, citation and
preservation. The original URL is recorded for every item in `manifest.json`
and `SNAPSHOT.md`.
