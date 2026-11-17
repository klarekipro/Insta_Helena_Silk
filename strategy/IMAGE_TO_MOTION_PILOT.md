# HELENA SILK — IMAGE-TO-MOTION PILOT
**Research date:** 2026-11-17 · **Status:** PROPOSED / NO VIDEO GENERATED / NO PAID API CALLS AUTHORIZED

## Purpose
Turn selected existing original fashion PNGs into **short Instagram Reels** where an AI-created model walks naturally, fabric moves, and the educational fashion commentary stays truthful. Maintain editorial transparency: generated fashion imagery **does not document an authentic Dior/Prada/etc. runway**.

## Three levels of animation
1. **Camera-only motion (lowest risk):** FFmpeg / CapCut / Adobe Express pan, crop, parallax, zoom and soundtrack. Very low compute but model itself does not walk.
2. **Generative image-to-video (recommended first pilot):** original PNG as starting frame → prompt describing natural runway walk and garment movement → 5–8 s candidate. Services: Runway Gen-4.5, Kling 4.0, Luma Ray3. Verify availability, credits, output rights, data terms on actual plan.
3. **Motion transfer (if walking looks unnatural):** record or license a simple, continuous video of a real person walking with whole body in frame. Use a reference-video feature such as Kling Motion Control (or a suitable Runway motion tool) to guide synthetic fashion model motion. **Do not assume Runway Act-Two is optimized for full runway walking:** its published input best practices favor a waist-up performer with visible face.
4. **Dressing / jacket on-off (separate experimental pilot):** create two approved **fully clothed** keyframes of the same model at nearly identical pose/camera/lighting, one with jacket and one without, then use start+end frame interpolation / Kling Keyframes or Google Flow Frames. Do not expect precise physically accurate buttoning, zipper, sleeve or fabric deformation. Prefer two-shot editing or camera transition if the transform creates artifacts.

## Suitable prototype images
- `visuals/assets/batch-04/HS_B04_06_Fuchsia_Orange_Tailoring.png` (only after this file actually exists in GitHub): **natural forward runway walk**. Clear tailoring and trousers.
- `visuals/assets/batch-03/HS_B03_07_Black_White_Geometry.png`: **subtle walking + locked camera**, watch whether the graphic pattern survives.
- `visuals/assets/batch-04/HS_B04_08_Emerald_Sheer_Garden.png`: **slow fabric motion and single step**, test organza consistency; technically hardest.

**Do not claim that these binary paths exist** before checking. Last checkpoint had the 40 PNGs as four ZIP downloads with textual registries in GitHub; Claude Code is separately tasked with uploading them.

## Minimal pilot (not automatic execution)

### Test A — controlled 5–6 second walk
Input: `HS_B04_06_Fuchsia_Orange_Tailoring.png`  
Target: one uninterrupted portrait 9:16 clip, model remains full-length, natural one or two steps, camera slightly tracks backward. Clothing colour and silhouette unchanged.

**Suggested English motion prompt:**

> A single continuous high-fashion runway shot. The woman takes two natural, measured steps forward toward the camera. Her fuchsia tailored blazer keeps its clean shoulder structure and the bright orange wide-leg trousers sway realistically with each step. Her structured handbag moves gently with her arm. The camera tracks backward smoothly at the same pace, keeping her entire body, shoes and outfit in frame. Refined editorial lighting, realistic foot contact and subtle fabric movement.

Do not add contradictory long story beats. Start with this simple prompt, adjust **one variable at a time**.

### Test B — detail-preservation
Input: `HS_B03_07_Black_White_Geometry.png`  
Prompt: single short walk, locked camera, test whether lines stay aligned, shoes remain visible.

### Test C — slow textile study
Input: `HS_B04_08_Emerald_Sheer_Garden.png`  
Prompt: subtle weight shift and one step, translucent layers respond naturally. Evaluate whether embroidery and jewellery mutate.

## Acceptance criteria
- Face stable; no unmotivated changes to model's identity or hairstyle.
- Garment holds cut, colour, patterns and major accessories.
- Hands/fingers, knees, ankles, high heels and contact with floor remain plausible.
- Natural movement, no morphing/warping, abrupt cuts or missing feet.
- Entire body survives 9:16 reframing. If the 2:3 PNG needs more vertical space, **outpaint/extend canvas**, do not crop off shoes/hem.
- 5–8 seconds is enough for a test; longer Reel can consist of short passed clips plus voiceover/subtitles.
- Motion is aesthetically interesting *and* supports a single educational observation.
- Video/cover, native German/Russian captions, optional narration, descriptive alt text and accurate AI disclosure all independently reviewed.

## Pilot evaluation
Generate **one candidate per chosen model** after owner authorizes provider and budget. Rate 1–5 per: body/face continuity, apparel stability, gait realism, fashion appeal, watchability. Don't bulk-generate all 40 assets. Save original PNG, generation prompt, model/version, provider, settings, output MP4, cost/credits, review notes and SHA-256 in a future `motion/` registry.

## Cost / operational approach
- Runway official Gen-4.5 lists **12 credits per second** and 2–10 s generation. Example: 6 s × 12 = 72 credits per try, not a currency price. Pricing/plans vary.
- Kling 4.0 documents image-to-video, keyframes and 3–30 second outputs; provider costs vary.
- Free quotas may watermark outputs or limit export; verify before making any promise.
- For local no-fee motion, FFmpeg/CapCut-style pan and zoom is suitable, but it is **not a model walking**.

## Platform honesty
AI-generated photorealistic video on Instagram should be properly disclosed using the platform's AI info label where required, and explained in captions (e.g. `KI-generierte Modevisualisierung` / `AI-визуализация моды`). Never describe artificial video as authentic 2027 fashion show footage.

## Official references checked
- Runway Gen-4.5 specifications: https://help.runwayml.com/hc/en-us/articles/46974685288467-Creating-with-Gen-4-5
- Runway motion prompting: https://help.runwayml.com/hc/en-us/articles/48324313115155-Image-to-Video-Prompting-Guide
- Runway Act-Two limitations: https://help.runwayml.com/hc/en-us/articles/42311337895827-Performance-Capture-with-Act-Two
- Kling 4.0 image-to-video and keyframes: https://kling.ai/quickstart/kling-4-model-user-guide
- Kling 3.0 Motion Control: https://kling.ai/quickstart/motion-control-user-guide
- Luma Ray3 image/keyframes: https://lumalabs.ai/learning-hub/ray3-faqs
- Google Flow frames-to-video: https://support.google.com/flow/answer/16353334?hl=en
- Meta AI media labelling: https://about.fb.com/news/2026/02/meta-prepares-for-2026-us-midterms/

## Decisions needed before spending
1. Choose service / account to connect or use directly (e.g. Runway or Kling).
2. Authorize a test budget; keep first batch to 1–3 clips.
3. Choose whether to prioritize **walking** (recommended) or **jacket on/off** (harder).
4. Owner selects final outputs and localizes voiceover/overlays.
