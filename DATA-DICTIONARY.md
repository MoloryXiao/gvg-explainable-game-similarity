# Data dictionary

One row represents one unique, undirected game pair. The written recommendation is directional from `source_game_id` to `target_game_id`, but the pair is not repeated in reverse within this version.

| Field | Meaning |
|---|---|
| `relation_id` | Stable relation key: `source_game_id--target_game_id`. |
| `source_game_id`, `target_game_id` | GVG catalogue slugs. |
| `source_title`, `target_title` | Titles verified against Steam on 2026-09-02. |
| `source_steam_appid`, `target_steam_appid` | Steam application identifiers. |
| `why_similar_en`, `why_similar_zh` | Bilingual, GVG-authored explanation of shared mechanics or structure. |
| `key_differences_en`, `key_differences_zh` | Bilingual, evidence-bounded differences relevant to choosing. |
| `best_for_en`, `best_for_zh` | Bilingual editorial preference guidance, not measured player preference. |
| `confidence` | Upstream confidence label; all rows in v0.1 are `high`. |
| `assessment_type` | `fact_checked_editorial`: factual features checked against listed sources; comparison remains editorial. |
| `source_ids` | Pipe-separated source identifiers aligned with `source_urls`. |
| `source_urls` | Pipe-separated official Steam store URLs for both games. |
| `sources_captured_at` | Capture timestamps aligned with source IDs and URLs. |
| `validated_at` | Date of the manual identity, factual and bilingual review. |

The dataset deliberately excludes copied store descriptions, review text, images, prices, ratings, estimated session length and 1–10 experience scores.
