# Primer Packs

Loadable **next-word suggestion primer** packs for LeanType
(https://github.com/LeanBitLab/LeanType).

A primer pack is a small JSON file of n-gram statistics (unigrams, bigram and
trigram continuation probabilities) computed from the Leipzig Corpora
Collection news text (CC-BY 4.0; sources listed below). The keyboard
interpolates this statistical backbone with your personal typing history to
produce next-word suggestions that work from day one.

Packs are **static data**: no code, no AI model, nothing runs in the
background. The suggestion engine itself is unchanged.

## Naming convention

`pgen_<lang>[_<REGION>].json` — e.g. `pgen_en_GB.json`, `pgen_pl_PL.json`.
The keyboard resolves packs for its active locale by this filename, both for
downloaded copies (app external files dir, `primer/`) and for any pack bundled
in an APK build. One scheme everywhere.

## Available packs

| File | Locale | Size | Corpus |
|---|---|---|---|
| [`pl_PL/pgen_pl_PL.json`](pl_PL/pgen_pl_PL.json) | Polish | 12.9 MB | Leipzig `pol_news_2023_100K` |
| [`en_GB/pgen_en_GB.json`](en_GB/pgen_en_GB.json) | British English | 27.1 MB | Leipzig `eng_news_2020_1M`, spelling-folded toward en-GB |

## Installation

1. Download the pack file for your language.
2. In the keyboard: **Settings → Libraries → Suggestion Primers → Import pack
   file**, pick the downloaded file.
3. Enable the master switch (or use the wizard's Libraries step on first run).
   No restart needed — suggestions reload immediately.

## Sources & licence

Corpus: Wortschatz-Korpora / Leipzig Corpora Collection,
https://downloads.wortschatz-leipzig.de/corpora/ — distributed under CC-BY 4.0.
This repository therefore distributes the derived packs under
**CC-BY 4.0**: you may share and adapt them with attribution.
