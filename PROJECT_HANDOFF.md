# HELENA SILK — PROJECT HANDOFF / ВОССТАНОВЛЕНИЕ КОНТЕКСТА

> **START HERE IN ANY NEW CHAT.** Read this file first, then `README.md`, `docs/BRIEF_DECISIONS.md`, and the relevant batch registry.  
> **Snapshot:** 2026-11-16 · **Status:** 4/5 image batches created as drafts, fifth batch NOT started. **Owner approval pending.**

## Repository / branches

- Repository: https://github.com/klarekipro/Insta_Helena_Silk
- Ongoing editorial branch: `feat/editorial-foundation`
- `main` is a separate baseline. **Do not merge to main or delete the working branch without an explicit owner instruction.**
- Dedicated point-in-time checkpoint branch: `checkpoint/batch-04-handoff-2026-11-16` (created after the handoff files are committed, if permitted).
- Work under `feat/editorial-foundation`; fetch actual HEAD before editing. A commit SHA mentioned in a former chat may be stale.

## Unchanging editorial principle

**«Мы создаём не каталог красивой одежды, а авторский взгляд на мир моды».**

Helena Silk is an independent fashion-inspiration and fashion-education project. Helena's point of view, careful observation of materials/silhouettes/colours, and educational explanations give the posts value beyond attractive pictures. Do not claim that Helena is a certified stylist or sells products.

## Confirmed owner decisions

- **Language strategy:** two prospective Instagram accounts, German and Russian; one shared editorial source, **native DE/RU localization**, not mandatory literal translation. Account names not final.
- **Aesthetic:** classic elegance mixed with contemporary experiments.
- **Visual priority:** full-length fashion looks; details may follow as supplementary material.
- **Voice:** informative/educational analysis of fashion, not promotional copy.
- **Presentation rule:** **NO LARGE NUMBERS / NO OVERSIZED CONCEPT IDs printed on images**. Prefer clean vertical individual images, no grids or collages, no brand logos.
- **Originality rule:** avoid reusing nearly identical outfits, silhouettes, palettes and model styling across batches.
- **Fashion research:** collections AW 2026/27 and SS 2027 shown in Paris, Milan, Madrid; research files exist. Do not mix season with the show date.

## Actual production inventory

| Batch | Image PNGs | State | Character |
|---|---:|---|---|
| 01 | 10 | VISUAL_DRAFT | First pilots; **six themes + four variants**, not 10 wholly distinct concepts; some generated designer names |
| 02 | 10 | VISUAL_DRAFT | Individual posters but some repeated ivory/beige tailoring, luxury logos; not publication ready |
| 03 | 10 | VISUAL_DRAFT | More dramatic organza, embroidery, graphic black/white, gold/saffron; some internal colour overlap |
| 04 | 10 | VISUAL_DRAFT | Cobalt, emerald, sunshine yellow, chrome, standout **fuchsia/orange trouser suit**; **several close variants of blue/green/yellow/chrome** |
| **Total** | **40 PNGs** | **NOT APPROVED** | 40 image files ≠ 40 independent, publication-ready stories |
| 05 | 0 | **NOT STARTED** | 10 more proposed, requiring greater diversification |

**The 40 PNG binaries are NOT yet in this GitHub repository.** They exist as four conversation downloadable ZIP files. They must be downloaded and safely backed up by the owner, ideally uploaded into `visuals/assets/batch-01` through `batch-04`. This is a real outstanding dependency, not a completed GitHub backup.

**Important for image splitting:** The ZIPs already contain ten **separate PNGs** each. Do not crop the contact sheet to recover individual images; use the original PNGs. Contact sheets are only previews.

## Four ZIP backups — verify before moving

| Local/archive filename | PNG count | SHA-256 of ZIP |
|---|---:|---|
| `Helena_Silk_Batch_01_10_images.zip` | 10 | `389af8e1cf629a25a9199d7569f9091ef86bdbfc83050b7c5d0333b891d67141` |
| `Helena_Silk_Batch_02_10_images.zip` | 10 | `bb1981ef0a8207b339d929e189e643a7e099d50de02693dd33efbc921a561d29` |
| `Helena_Silk_Batch_03_10_images.zip` | 10 | `0322857218724718b9aa917407c6ee20f903197aa05a8a0b4c9c43f08b2da124` |
| `Helena_Silk_Batch_04_10_images.zip` | 10 | `669f9713ce96636fb683aa2421bde06224cee1d03cb3450a71f44301d6a12cf8` |

The ZIPs lived under `/mnt/data/` **during the producing chat**; this is not a persistent Mac file path and must not be assumed to exist in future chats. The owner can download them from their original chat. See [image upload steps](docs/UPLOAD_IMAGE_BACKUPS.md).

## Documentation map

- `README.md`: mission, central idea, links.
- `docs/EDITORIAL_VISION.md`: philosophy and voice.
- `docs/CONTENT_STRATEGY_DE_RU.md`: two-language distribution.
- `docs/BRIEF_DECISIONS.md`: confirmed owner choices.
- `docs/MASTER_PROMPT.md`: research/30-story generation contract.
- `docs/RESEARCH_2026_2027.md`: fashion-show dates and sources.
- `content/CONCEPTS_30.md`: 30 researched editorial story candidates; story IDs FR/IT/ES.
- `content/PILOT_SHORTLIST_10.md`: suggested ten pilots, **not approved**.
- `visuals/BATCH_01_10_POSTERS.md` through `BATCH_04_10_POSTERS.md`: batch registers.
- `visuals/BATCH_03_CAPTIONS_DE_RU.md`, `visuals/BATCH_04_CAPTIONS_DE_RU.md`: bilingual caption drafts; second batch captions are also in its ZIP.
- `visuals/ASSET_INVENTORY_01_04.md`: expected files and ZIP hashes.
- `docs/CONTINUE_IN_NEW_CHAT.md`: **copy-ready next-chat prompt**, priorities, and QA.
- `docs/IMAGE_PRODUCTION_RULES.md`: production rules for further independent visuals.

## Exactly where to resume

1. **If the owner is now separating/saving the fourth batch:** do not create new images. Assist with placing the ten original PNG files under `visuals/assets/batch-04/` (or confirm owner has already done so), compare against the registry and verify at least file count and filenames. Also upload batches 01–03 if owner wants all forty protected.
2. **If the owner says "fifth batch" / "next ten":** create exactly 10 *individual* new images, not a contact sheet, guided by the no-repeat register. Avoid repeating metallic silver gowns, all-cobalt dresses, emerald floral evening gowns, and bright-yellow ruffles. Prefer new shapes, pants, coats, sports-influenced architecture, graphic prints, dark-blue star embroidery, chartreuse, coral/cyan, unexpected material pairings and different models. Review each separately before packaging.
3. Create native German and Russian descriptions, thoughtful questions, measured hashtags, and a binary manifest for each batch. Do not invent actual runway provenance or textile fibre compositions.
4. Save all text work and decisions to `feat/editorial-foundation`; **verify each GitHub write by reading it back.**
5. Only mark a post `APPROVED` after Helena or the owner says so. No Instagram publication is recorded.

## Copyright and factual safety

All generated fashion images are **AI illustrations**, not exclusive photographs from authentic Dior, Prada, Chanel, etc. events. Prior batches may include brand-looking text. Never attribute those synthetic garments as real shows. For reporting about actual collections, use authentic licensed photographs, verified sources, look IDs and usage rights. Avoid claims about silk/wool composition merely because renderings look that way.

## Current boundary

No Instagram handles finalized, no approved collection-to-image mapping, no verified photo licences, no real Instagram posts published, no automatic bot engagement, and no fifth image batch. The remaining work is explicitly recorded so a new chat does not silently assume completion.
