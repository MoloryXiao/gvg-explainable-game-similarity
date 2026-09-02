# GVG Explainable Game Similarity Dataset 2026

Version: `0.1.0`  
Status: **public release package; not yet uploaded**  
Snapshot: 2026-09-02

## What is included

This release candidate contains 50 unique game pairs covering 82 games. Each row provides:

- stable game IDs, titles and Steam App IDs;
- a bilingual explanation of why the games are similar;
- a bilingual description of material differences;
- bilingual preference guidance;
- row-level IDs and URLs for both official Steam store sources;
- validation date and confidence label.

The annotations are GVG editorial judgments designed to make recommendations inspectable. They are not player-behavior ground truth and do not claim that one game is objectively better.

## Files

- `data/gvg-explainable-game-similarity-v0.1.csv` — the 50 reviewed pairs;
- `data/sources.csv` — deduplicated source IDs, URLs and capture dates;
- `DATA-DICTIONARY.md` — field definitions;
- `METHODOLOGY.md` — selection and validation method;
- `CORRECTIONS.md` — correction process;
- `audit/validation-summary.json` — public QA summary;
- `SHA256SUMS.json` — hashes for the two CSV files.

## Validation

All 50 rows were rewritten conservatively after checking the current official Steam records for both games. The review covered 82 unique Steam App IDs and 100 relation endpoints. No title/App ID mismatches, duplicate pairs, missing required fields or missing source URLs remain in this candidate.

Official store pages validate game identity and described features. They do not validate comparative quality or user preference; those parts remain clearly labeled editorial guidance.

## Citation

Suggested citation until a DOI is assigned:

> Miles. (2026). *GVG Explainable Game Similarity Dataset 2026* (Version 0.1.0). https://gamevgame.com/

Replace the website URL with the Zenodo DOI after publication.

## License

The GVG-authored dataset structure and annotations are licensed under the Creative Commons Attribution 4.0 International license (`CC BY 4.0`). See `LICENSE.md`.

## Corrections

Report a wrong identity, feature or translation at <https://gamevgame.com/contact> or `support@gamevgame.com`. Include the `relation_id` and the evidence URL.
