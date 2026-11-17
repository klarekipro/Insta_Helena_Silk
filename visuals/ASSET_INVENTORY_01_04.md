# Asset inventory — batches 01–04

**Verified backup — 2026-11-17:** all 40 original AI-generated PNG drafts are saved in GitHub, 10 each in `visuals/assets/batch-01/` through `batch-04/`. Asset commit: `4c680ab95c8cd1d439f2ecc28a5e775c402a54a2`. ZIP SHA-256 and CRC checks passed; PNG bytes, filenames, chunk CRCs and decompression verified. All 30 available per-image reference hashes (batches 02–04) match; batch 01 has no original per-image hash reference. All images remain **VISUAL_DRAFT**, owner approval **PENDING**; Batch 05 **NOT STARTED**.

**Source:** four local ZIP archives in `/Users/admin/Downloads/`, matched to the pre-existing reference ZIP hashes below. Archives retained unchanged. [Per-image SHA-256, byte sizes, dimensions and source entries](ASSET_MANIFEST_01_04.json).

## Backups and checksums

| Batch | Archive | PNGs | ZIP SHA-256 |
|---|---|---:|---|
| 01 | `Helena_Silk_Batch_01_10_images.zip` | 10 | `389af8e1cf629a25a9199d7569f9091ef86bdbfc83050b7c5d0333b891d67141` |
| 02 | `Helena_Silk_Batch_02_10_images.zip` | 10 | `bb1981ef0a8207b339d929e189e643a7e099d50de02693dd33efbc921a561d29` |
| 03 | `Helena_Silk_Batch_03_10_images.zip` | 10 | `0322857218724718b9aa917407c6ee20f903197aa05a8a0b4c9c43f08b2da124` |
| 04 | `Helena_Silk_Batch_04_10_images.zip` | 10 | `669f9713ce96636fb683aa2421bde06224cee1d03cb3450a71f44301d6a12cf8` |

### Expected original image filenames

**Batch 01** (ten including alternates; some have misleading designer labels in image; do not publish as show photos):
```
HS_01_DIOR_v01.png
HS_01_DIOR_v02.png
HS_07_CHANEL_v01.png
HS_07_CHANEL_v02.png
HS_11_PRADA_v01.png
HS_11_PRADA_v02.png
HS_14_BOTTEGA_v01.png
HS_21_MANS_v01.png
HS_21_MANS_v02.png
HS_26_ERNESTO_v01.png
```

**Batch 02**:
```
HS_B02_01_Sculptural_Ivory_Coat.png
HS_B02_02_Burgundy_and_Ivory.png
HS_B02_03_Parisian_Flowing_Tailoring.png
HS_B02_04_Layering_in_Grey_and_Wine.png
HS_B02_05_Soft_Tailored_Jacket.png
HS_B02_06_Burgundy_Sculptural_Dress.png
HS_B02_07_Black_Power_Tailoring.png
HS_B02_08_Botanical_Skirt.png
HS_B02_09_Tweed_and_Contrast.png
HS_B02_10_Chocolate_Brown_Classic.png
```

**Batch 03**:
```
HS_B03_01_Petal_Sculpture_Purple_Gold.png
HS_B03_02_Burgundy_Floral_Organza.png
HS_B03_03_Silver_Transparent_Couture.png
HS_B03_04_Ivory_Satin_Origami.png
HS_B03_05_Teal_Embroidered_Coat.png
HS_B03_06_Champagne_Gold_Waves.png
HS_B03_07_Black_White_Geometry.png
HS_B03_08_Plum_Bronze_Asymmetry.png
HS_B03_09_Mustard_Plum_Layering.png
HS_B03_10_Saffron_Embroidered_Coat.png
```

**Batch 04**:
```
HS_B04_01_Cobalt_Emerald_Contrast.png
HS_B04_02_Sunshine_Transparent_Ruffles.png
HS_B04_03_Emerald_Gold_Embroidery.png
HS_B04_04_Yellow_Silver_Architecture.png
HS_B04_05_Chrome_Pleated_Futurism.png
HS_B04_06_Fuchsia_Orange_Tailoring.png
HS_B04_07_Cobalt_Pantsuit_Origami.png
HS_B04_08_Emerald_Sheer_Garden.png
HS_B04_09_Chrome_Studio_Sculpture.png
HS_B04_10_Yellow_Tailored_Couture.png
```

## Verified GitHub storage layout

```text
visuals/
  assets/
    batch-01/   # 10 unmodified PNG files
    batch-02/   # 10 unmodified PNG files
    batch-03/   # 10 unmodified PNG files
    batch-04/   # 10 unmodified PNG files
  BATCH_01_10_POSTERS.md
  BATCH_02_10_POSTERS.md
  BATCH_03_10_POSTERS.md
  BATCH_04_10_POSTERS.md
```

All four directories exist in the asset commit above, with exactly 10 original PNGs each. No previews or auxiliary ZIP files are counted.

For each ZIP, Mac verification: `shasum -a 256 ~/Downloads/Helena_Silk_Batch_04_10_images.zip` (adjust name/path).
For each extracted set, ensure ten `.png` files before and after upload.

See `docs/UPLOAD_IMAGE_BACKUPS.md` for copy-ready steps.

## Preservation verification

| Batch | GitHub path | PNGs | Source per-image SHA-256 references |
|---|---|---:|---|
| 01 | [assets/batch-01/](assets/batch-01/) | 10 | Not supplied; computed hashes recorded |
| 02 | [assets/batch-02/](assets/batch-02/) | 10 | 10 / 10 matched |
| 03 | [assets/batch-03/](assets/batch-03/) | 10 | 10 / 10 matched |
| 04 | [assets/batch-04/](assets/batch-04/) | 10 | 10 / 10 matched |

**Total: 40 PNGs; 40 distinct SHA-256 hashes; 91,413,877 original bytes.** Every extracted file is byte-identical to its source ZIP entry; PNG signature, chunk CRCs and IDAT decompression passed. No resizing, cropping, re-encoding or filename changes.
