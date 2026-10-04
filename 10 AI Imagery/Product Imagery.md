---
type: assets
status: draft
updated: 2026-10-04
---
# Product Imagery

**Vision:** honest and precise. The customer sees the piece they will receive. A beautiful image that does not match the shipped piece is a defect, a complaint and a replacement. This category gets the most care and the strictest checks.

## Accuracy first
- Source of truth: the Branvas product page, its photos and its stated dimensions, saved in `10 AI Imagery/references/<product>/`
- Generate from the reference image (image-to-image or reference input), never from a text description alone
- Never improve the design: no extra stones, longer drop, thicker chain, different clasp, brighter plating colour, bigger stone
- Plating colour and metal tone must match the reference. "Gold-plated" shows as plated gold, not a rich solid-gold glow
- Scale must be true to the stated size. A 10 mm hoop is not shown as 20 mm on an ear
- Show only the Branvas piece. No other jewelry in the frame unless it is also in the catalog

## Shot set (5 to 6 per product, same order on every product page)
| # | Shot | Purpose |
|---|---|---|
| 1 | Clean still on cream, soft light streak, 4:5 | The first image: the piece alone, clear and exact |
| 2 | Close-up on skin or fabric | Detail, stones, finish |
| 3 | Worn: ear, neck, hand or wrist crop | Scale and how it sits |
| 4 | Layered with one or two catalog pieces | Styling ("Wear it with") |
| 5 | Scale shot (hand, ear or neck in context) | Honest size |
| 6 | Gift box and cloth | Only if it is the packaging we ship |

Sizes: 4:5 at 2000x2500 master, WebP for the site. One look across the whole catalog: same ground, light direction and grade as [[Website Imagery]], so a product page never looks like a different brand.

## Workflow
1. Save Branvas photos and dimensions to `references/`
2. Write a one-paragraph **accuracy note** in the product note: stone count, stone shape and size, chain type, clasp, closure, finish, thickness, measurements
3. Generate shot 1 first. Do not move on until it passes the check
4. Reuse the winning prompt and seed for the other shots
5. Side-by-side check at the same scale: AI image next to the Branvas photo
6. Founder approves the first product of each type (earrings, necklace, ring, bracelet) by look; after that AI approves and the founder spot checks
7. File as `lumi_<product>_<type>_<yyyymmdd>_v1`, add to [[Asset Index]], link in the product note

## Checklist (every product image)
- [ ] Shape and proportions match the Branvas photo
- [ ] Stone count, stone shape and stone size match
- [ ] Chain or band style, clasp and closure match
- [ ] Metal tone and finish match the reference
- [ ] Size matches the stated dimensions on the body
- [ ] No extra jewelry, no invented detail, no engraving or text
- [ ] Hands, ears, neck look natural, fingers correct
- [ ] Light and grade match the catalog look
- [ ] Alt text describes the piece only; never says "customer"

Any "no" means regenerate. Don't retouch around drift. Drift examples go in `rejected/`.

## Prompt block
`[Base style block]` + `product on cream ivory ground, soft window light, exact replica of the reference piece, same proportions, no added details, centered with generous negative space, 4:5, sharp focus on the piece` + shot-specific line (`close-up on skin`, `worn on ear, crop below the eye`, etc.)

## Risk notes
- If the AI cannot hold the design over several shots, use fewer shots. Three exact images beat six drifting ones
- If Branvas allows it, retouching the Branvas photo into our look (cleaned ground, matched light) can be more accurate than full generation. Ask in [[Imagery Hub]]
- Photo claims must match [[Voice and Rules]]. Don't show water or shower contexts unless the style is marked water-safe by Branvas
