# HELENA SILK — IMAGE PRODUCTION & QA RULES

**Current status:** owner-approved *art direction*, but individual visuals are still drafts pending Helena's review.

## Core visual contract

1. Each output is **one vertical image** showing **one complete fashion look**, head to footwear (preferred 4:5 for Instagram; 2:3 source is acceptable if full outfit survives crop).
2. **Do not put giant numbers** such as 01, 11 or 26 on the artwork. Concept numbering belongs **only to metadata and filenames**.
3. Avoid brand logos and designer names on generated images; no false association with real shows.
4. Avoid baked-in caption paragraphs and mixed-language typography. Draft captions as editable text in DE/RU outside the image.
5. Model, pose, lighting, fabric behaviour and garment shapes should be plausible and richly detailed.
6. Keep visual coherence as a magazine series without using the same model or same dress shape for every post.
7. Every next concept should be meaningfully distinct from existing sets by **silhouette + colour + construction + materials + model presentation**.
8. Explicitly identify each generated image as **AI fashion illustration** rather than real runway photography.

## Previous batches — motifs to avoid overusing

- **B01:** ivory peplum jacket / gray-burgundy layers / butterfly-inspired printed suit / pale tweed / olive oversized coat / lilac fluid gown; some alternate versions.
- **B02:** black power suit, Burgundy tiered skirt/layers, ivory floral skirt, tweed, chocolate-brown coat; several repetitive beige coats.
- **B03:** purple-gold petals, burgundy floral organza, transparent silver couture, ivory origami, teal/embroidered outerwear, champagne waves, black/white geometry, plum-bronze asymmetry, mustard-plum layers, saffron floral embroidery.
- **B04:** cobalt/emerald dress, sunshine-yellow sheer ruffles, emerald-gold embroidery, yellow/silver geometry, chrome pleats, **fuchsia/orange pants**, cobalt pantsuit, emerald organza, chrome sculptural gown, yellow tailored couture.

## Fifth-batch candidate angles (NOT generated yet)

- Midnight-blue star-map embroidery; sharp closed or column silhouette instead of another ruffled gala gown.
- Chartreuse tailoring with sportswear construction and new practical footwear.
- Terracotta tapestry as a structured coat or trouser ensemble.
- Coral + cyan graphic colour blocking with a new figure silhouette.
- Optical prints, checks or unconventional geometries (not another generic black-white swirl).
- Complex handbag and footwear styling as the compositional centre within a full look.
- Modern Spanish-inspired sculptural jacket with structured trousers, avoiding invented brand attribution.
- Cool-white/navy technical textiles, interesting cut-outs used tastefully.
- Rich forest green as tailored suit rather than embroidered evening gown.
- Strong orange/rust geometric design with contrasting cool accessories.

## Per image acceptance checklist

- Single image? (No mosaics, contact sheets or side-by-side comparisons within original PNG)
- Person and footwear fully visible?
- No prominent numbers, logos, hallucinated designer labels?
- Distinct from prior 40 on colour, shape, material effect and accessories?
- Original image is stored in ZIP and `ASSET_MANIFEST.json` with SHA-256?
- Accurate natural RU and DE captions, not made-up garment composition?
- Status `VISUAL_DRAFT`; owner's approval recorded only after review?

## Workflow

Produce each image separately; visually inspect; reject collages and repeats; use logical filenames such as `HS_B05_01_<theme>.png`; create contact sheet **only after** all 10 standalone originals exist; package PNGs plus caption draft, manifest, QA notes in ZIP; register text in GitHub; upload binary files to GitHub via available mechanism or owner-assisted manual steps. Always disclose any unuploaded assets.
