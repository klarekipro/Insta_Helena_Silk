# How to back up all four Helena Silk image batches to GitHub (Mac)

**Verified backup — 2026-11-17:** all 40 original AI-generated PNG drafts are saved in GitHub, 10 each in `visuals/assets/batch-01/` through `batch-04/`. Asset commit: `4c680ab95c8cd1d439f2ecc28a5e775c402a54a2`. ZIP SHA-256 and CRC checks passed; PNG bytes, filenames, chunk CRCs and decompression verified. All 30 available per-image reference hashes (batches 02–04) match; batch 01 has no original per-image hash reference. All images remain **VISUAL_DRAFT**, owner approval **PENDING**; Batch 05 **NOT STARTED**.

[Original PNGs](../visuals/assets/) · [Integrity manifest](../visuals/ASSET_MANIFEST_01_04.json). The instructions below are retained for recovery; compare existing file hashes before any upload to avoid duplicates.

**You do NOT need to split the contact sheets.** Each ZIP already contains 10 original independent PNG files. Extract those, not the contact sheet.

## Option A — GitHub web UI (no terminal)

1. Download and keep all four `Helena_Silk_Batch_0X_10_images.zip` archives from the original conversation.
2. Open https://github.com/klarekipro/Insta_Helena_Silk/tree/feat/editorial-foundation and confirm the branch selector reads **feat/editorial-foundation**, not main.
3. For each batch, unzip locally and locate exactly 10 `.png` originals. Ignore `PREVIEW_CONTACT_SHEET.jpg` and the Markdown/JSON for image counting.
4. In GitHub choose **Add file → Upload files**, upload the ten originals into directory `visuals/assets/batch-0X/` (create via Git on Mac if the web UI cannot create a folder destination conveniently). Commit each batch with message `assets: store batch 0X original AI PNGs`.
5. Verify the new filenames under the branch and update the batch registry status from `binary not uploaded` to `binary committed` only after checking.

## Option B — Mac Terminal (reliable; requires GitHub authentication)

```bash
cd "$HOME/Documents"
git clone https://github.com/klarekipro/Insta_Helena_Silk.git
cd Insta_Helena_Silk
git fetch origin
git switch feat/editorial-foundation
mkdir -p visuals/assets/batch-01 visuals/assets/batch-02 visuals/assets/batch-03 visuals/assets/batch-04
```

Put the four ZIP files in `~/Downloads`. Next run **one extraction command per batch** (with ZIP entry paths flattened):

```bash
unzip -jo "$HOME/Downloads/Helena_Silk_Batch_01_10_images.zip" '*.png' -d visuals/assets/batch-01/
unzip -jo "$HOME/Downloads/Helena_Silk_Batch_02_10_images.zip" '*.png' -d visuals/assets/batch-02/
unzip -jo "$HOME/Downloads/Helena_Silk_Batch_03_10_images.zip" '*.png' -d visuals/assets/batch-03/
unzip -jo "$HOME/Downloads/Helena_Silk_Batch_04_10_images.zip" '*.png' -d visuals/assets/batch-04/
```

This extracts PNGs only and retains original bytes. Do **not** import JPEG contact sheets as original look files.

Then verify counts and upload:

```bash
for batch in 01 02 03 04; do
  printf "batch-%s: " "$batch"
  find "visuals/assets/batch-$batch" -maxdepth 1 -type f -name '*.png' | wc -l
done
git status --short
git add visuals/assets/batch-01 visuals/assets/batch-02 visuals/assets/batch-03 visuals/assets/batch-04
git commit -m "assets: preserve original AI visuals from batches 01-04"
git push origin feat/editorial-foundation
```

Expected counts: **10 / 10 / 10 / 10**. Check `git status` for unrelated changes before committing. If the working directory already exists, do not clone again: open it, fetch, and check current branch and local changes first.

### Integrity check

Compare each ZIP hash to `visuals/ASSET_INVENTORY_01_04.md`. For example:

```bash
shasum -a 256 "$HOME/Downloads/Helena_Silk_Batch_04_10_images.zip"
```

If a checksum differs, stop and verify which archive you are using; do not overwrite an existing approved image.

### Update docs after upload

Change the corresponding batch registry to include correct relative paths, commit SHA and verification outcome. Do **not** mark the images Instagram-ready just because they exist in GitHub: they still need owner review, copy verification and correct AI disclosure.

**NEVER** merge these AI assets into `main` unless the owner explicitly asks.
