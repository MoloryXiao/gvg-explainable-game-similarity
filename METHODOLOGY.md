# Methodology

## Candidate selection

The internal pool contained 743 directional recommendations. v0.1 candidates had to meet all of the following automatic gates:

- `high` confidence;
- editorial similarity score at least 70 for selection only; the score is not published;
- at least two resolvable official-store sources;
- source URLs covering the Steam App ID of both games;
- basic agreement among slug, title and Steam App ID;
- no reverse-direction duplicate;
- no obvious dynamic-number or absolute promotional wording.

This produced 117 eligible directional rows and 112 unique pairs. The first 50 by selection score became the review set.

## Data-quality validation

- 50/50 unique relation IDs;
- 50/50 unique undirected pairs;
- 0 missing required fields;
- 82/82 current Steam App ID records retrieved successfully;
- 100/100 pair endpoints matched current official Steam titles and game type;
- 100/100 endpoints covered by row-level official source URLs.

## Content validation

Every row was reviewed against the current official Steam record for both games. All 50 original annotations were conservatively rewritten to remove unsupported rankings, quality claims, absolutes and marketing metaphors. English and Simplified Chinese were rewritten together.

The final text separates:

- source-backed identity and described features;
- GVG's editorial explanation of similarity;
- GVG's preference guidance.

## Limitations

- Steam descriptions are first-party marketing material and may change.
- This is a curated set, not a statistically representative sample of all games.
- Similarity and preference guidance are editorial, not behavioral measurement.
- v0.1 covers 50 pairs; it should not be used to claim full genre coverage.
- Corrections can change annotations in later versions while stable relation IDs are retained.
