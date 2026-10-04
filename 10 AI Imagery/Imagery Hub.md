---
type: assets
status: draft
updated: 2026-10-04
---
# AI Imagery Hub

Home for every AI image Lumi Paris makes. Three categories, three visions, three levels of effort. The reusable workflow is the `imagery` skill. Shared base style and credit rules: [[Imagery Prompts]]. Brand rules: [[Brand Bible]].

## The three categories
| | [[Website Imagery]] | [[Product Imagery]] | [[Socials Imagery]] |
|---|---|---|---|
| **Job** | Set the mood. First impression, trust, "this is not a dropshipping store" | Sell the exact piece. What the customer sees is what arrives | Make people stop, save and share. Word of mouth |
| **Vision** | Quiet editorial. Light on skin | Honest, precise, calm | Light-led, varied, platform-native |
| **Accuracy bar** | Medium: any jewelry shown must be a real catalog piece or cropped out | Highest: matches the Branvas piece exactly, every time | High for the featured piece, freer for mood |
| **Effort per image** | High: art-directed, many generations, best 1 in 10 kept | Highest: reference-based, side-by-side checked, two-stage approval | Medium: batch by theme, reframe winners |
| **Volume** | About 12 images total, then rarely changed | 5 to 6 per product | 9 per platform to start, then a steady flow |
| **Style** | One look, one grade | One look per product set, identical across the catalog | A few named styles, mapped to pillars |
| **Approver** | Founder, by look | AI checks, founder approves the first product of each type, then spot checks | Founder approves the style; AI approves posts inside it |
| **Credits** | Spend first | Spend most | Reframe, don't regenerate |

## Non-negotiables (all categories)
- No real people, no photoshoots. AI people are never shown as customers, reviewers or "real" wearers, in images or captions
- No Paris landmarks, French signage or Haussmann streets. Paris is how we look, not a setting
- No text in the image except the logo or "Wear the light.". No claims, prices or badges in the image
- Any jewelry in a frame is a catalog piece that ships. No decorative pieces we don't sell
- Natural hands, ears and fingers. Anything uncanny is regenerated, not retouched
- Palette stays inside [[Brand Bible]]: cream, ivory, warm stone; Warm Ink and Jardin Green only as small accents
- Use the platform's "AI-generated" label wherever it asks for one
- Never imply the image is a customer photo, a studio shoot or a real location

## Workflow (every image)
1. **Brief:** category, product or theme, shot type, aspect ratio, where it will be used
2. **Prompt:** base style block from [[Imagery Prompts]] plus the category block in its guide
3. **Test:** one generation per shot type before any batch (credits are limited, [[Budget]])
4. **Check:** the category checklist in its guide
5. **Approve:** per the table above
6. **File and log:** save as `lumi_<product-or-theme>_<type>_<yyyymmdd>_v1` in the category folder, add to [[Asset Index]], log the prompt and result in the prompt log below

## Folders
`10 AI Imagery/website/` · `10 AI Imagery/products/<product>/` · `10 AI Imagery/socials/instagram|tiktok|pinterest/` · `10 AI Imagery/references/` (Branvas photos used as accuracy references, never published) · `10 AI Imagery/rejected/` (drift examples, so we recognize them)

## Questions for Branvas (#ops)
- Can we use your product photos as reference for our own images? Do you offer clean or transparent cutouts?
- Exact dimensions per style: length, drop, ring size range, stone size, chain length and adjuster
- Is the packaging (box and cloth) the one we ship? A photo of it

## Prompt log
| Date | Category | Subject | Tool and model | Prompt | Result | Keep? |
|---|---|---|---|---|---|---|
| 2026-10-04 | Website | Home hero, collarbone and cream wrap, no jewelry | Higgsfield API | Hero prompt from [[Website Imagery]] (3:2) | `website/lumi_hero_collarbone_20261004_v1.webp`, 2016x1344. Only winner of the batch; other variants rejected | Yes, conditional: crop out lips and chin, lift shadows, upscale to 2400 |
| 2026-10-04 | Website | Home hero video from the collarbone still | Gemini video | Cinemagraph prompt, face still, light drift | Source 1280x720, 10 s, 24 fps, 2.4 MB, had audio. Made loop versions: desktop 1280x720 and mobile 4:5 720x900, ping-pong 20 s, no audio, 976 KB and 644 KB | Yes, conditional: preview on a phone, check the reverse half, face still allowed |
