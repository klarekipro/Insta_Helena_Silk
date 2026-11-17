# Helena Silk — Runway motion test 01

Date: 2026-11-17 (Europe/Berlin). Status: **MOTION_DRAFT / OWNER_REVIEW_PENDING**.

One image-to-video generation was submitted; one resulting clip was downloaded. No retries, extensions, upscales, edits or additional generated clips. This is an AI-generated fictional fashion illustration animated with AI, not authentic runway footage. Nothing was published to Instagram.

## Source and output

- Repository: `klarekipro/Insta_Helena_Silk`; branch: `feat/editorial-foundation`.
- Starting branch HEAD: `ed90d4af307ad0549a1c68975008817462ba670a`.
- Original source: [HS_B04_06_Fuchsia_Orange_Tailoring.png](../visuals/assets/batch-04/HS_B04_06_Fuchsia_Orange_Tailoring.png).
- Source SHA-256: `337b8cf12b0adeabe29c91a8676818ff5d440be89868d5e66715445a365285f8`.
- Source was uploaded unchanged, 1122 × 1402 pixels. The original file remains unchanged.
- Saved MP4: [HS_B04_06_Fuchsia_Orange_Tailoring_Runway_Test_01.mp4](../visuals/motion/test-01/HS_B04_06_Fuchsia_Orange_Tailoring_Runway_Test_01.mp4).
- MP4 SHA-256: `0f405ffdd524dc4026e8f3c4da3b255e8369c46f30616a6f9e241a3fb2119fa5`; size: 2,892,514 bytes.
- Original browser download retained in `/Users/admin/Downloads/` with Runway's generated filename: `Gen-4_5 - A single continuous high-fashion runway shot_ The woman takes two natural, measured steps.gen-4_5 - a single continuous high-fashion runway shot_ the woman takes two natural, measured steps.mp4`.
- [Runway session](https://app.runwayml.com/video-tools/teams/stechinua/ai-tools/generate?mode=tools&sessionId=88d11e42-648e-44d4-a5f2-422af1438b98) (account access required).

## Exact settings and observed output

| Parameter | Value |
|---|---|
| Provider / interface | Runway web app, Tool → Video; first-frame image-to-video |
| Model | Gen-4.5 |
| Generations submitted | 1 |
| Requested duration | 5 seconds |
| Output aspect ratio | 9:16 |
| Output resolution (Runway and file) | 720 × 1280 |
| Seed reported by Runway | 3463489034 |
| Fixed Seed switch before submission | Off; random seed assigned by Runway |
| Prompt enhancement / presets | Not used |
| Crop / sketch | Not manually applied |
| Output format | Default downloaded MP4; no upgrade or format change |
| Watermark | No, per Runway asset metadata |
| HDR conversion / upscale / interpolation | Not applied |
| Audio | No audio stream in downloaded file |
| Credit balance | 194 before, 134 after; observed usage 60 credits |
| Runway displayed generation time | Nov 17, 2026, 11:34 AM (browser local time) |
| Actual MP4 duration | 5.041667 seconds |
| Frames / frame rate | 121 frames / 24 fps |
| Codec / pixel format | H.264 High / yuv420p, progressive |

The source is approximately 4:5. Runway displayed **“Aspect ratios don't match”** after selecting 9:16; generation was submitted with the original uploaded image and no manual crop. The generated composition is narrower than the original. The source already contains seated spectators on both sides; the “no extra people” requirement is therefore assessed separately from retaining source background people.

## Exact submitted prompt

> A single continuous high-fashion runway shot. The woman takes two natural, measured steps forward toward the camera. Her fuchsia tailored blazer keeps its clean shoulder structure and the bright orange wide-leg trousers sway realistically with each step. Her structured handbag moves gently with her arm. The camera tracks backward smoothly at the same pace, keeping her entire body, shoes and outfit in frame. Refined editorial lighting, realistic foot contact and subtle fabric movement. Preserve the original colors, silhouette, accessories and overall look. Do not change the model’s identity, hairstyle, or outfit design. No cuts, no scene changes, no extra people, no text.

## QA

Method: full-file FFmpeg decode plus visual inspection of 20 chronological full-body samples at 4 fps (0.00–4.75 s), ten upper-body samples at 2 fps, and a full-resolution frame at 2.50 s. This is sampled-frame QA, not a claim of human real-time playback or exhaustive identity verification.

| Check | Assessment |
|---|---|
| Gait realism | Alternating runway strides, arm motion and fabric sway read plausibly in samples. **More than two steps** are visible; the action continues throughout the clip. Wide trouser hems obscure some foot contacts, so precise heel-to-floor contact is not fully established. |
| Face stability | Recognizably consistent face, hairstyle and earrings; subtle facial-detail drift and blinking. No obvious identity swap in inspected frames. Exact biometric identity preservation is not established. |
| Clothing stability | Fuchsia blazer, shoulder structure, lapels and orange wide-leg trousers remain recognizable. Folds and hem contours vary with motion; some synthetic smoothing/deformation is visible. |
| Accessory stability | Orange/navy structured handbag and blue pointed shoes remain present. Bag swings and rotates; handle/clasp and shoe-edge details vary and cannot be certified pixel-stable. |
| Framing / camera | Entire head, outfit and shoes visible in sampled full-body frames. Smooth-looking backward camera movement, but the model becomes smaller: distance increases rather than matching her pace exactly. Opening headroom is tight. |
| People / scene / text | No second walking model, cut, scene change or text overlay observed. More seated background spectators become visible as the view widens; strict “no extra people” is **not satisfied**. Some were already present in the source, and newly exposed background cannot be authenticated. |
| Instagram Reel suitability | Technically suitable vertical silent MP4 (9:16, 720p, about 5 s). Useful internal motion pilot; **not an exact brief pass or owner-approved publication asset** because step count, camera distance and background-person constraint diverge. |

**Another attempt recommended:** yes, if exact two-step timing, constant full-body scale and no background people are required. A later attempt should explicitly time two slow steps followed by a stationary hold, constrain constant camera distance, and resolve source spectators in a separately authorized source preparation step. No further generation was performed.

## Evidence and preservation

- [Chronological QA contact sheet](../visuals/motion/test-01/QA_CONTACT_SHEET.png) (read left-to-right, top-to-bottom; final unused tile is black).
- [Runway result screenshot](../visuals/motion/test-01/RUNWAY_RESULT_SCREENSHOT.png).
- [FFprobe technical metadata](../visuals/motion/test-01/FFPROBE.json).
- Full video decode completed without errors. The saved MP4 was copied byte-for-byte from the download, without re-encoding or trimming.
- `main` and `checkpoint/batch-04-handoff-2026-11-16` must remain unchanged. All work stays on `feat/editorial-foundation`; original PNG and source ZIP archives retained.
