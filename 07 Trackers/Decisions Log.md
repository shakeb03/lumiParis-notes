---
type: log
updated: 2026-10-04
---
# Decisions Log

Newest first. Never relitigate without a reason.

| Date | Decision | Why |
|---|---|---|
| 2026-10-04 | Storefront calls the cart "bag" everywhere (Add to bag, Your bag, sticky bar, cart page). Home hero text sits in a Lumi Cream panel over the media area | Founder preview feedback; brief says "Add to bag" and the hero message must show on first load |
| 2026-10-04 | Store build theme: "Lumi Paris — build", duplicated from live Horizon 4.2.0, unpublished. Code lives in the LumiParis-new repo; brand layer is `lumi-` sections, blocks and `assets/lumi.css` | Store Build Brief method; keeps the live theme untouched |
| 2026-10-04 | Fonts loaded from Google Fonts (Cormorant Garamond 500, Outfit 400/500) in theme code, overriding Horizon's font settings | Exact brand fonts; Shopify font library availability not verified. Revisit if page speed suffers |
| 2026-10-04 | TEST products are active and published to Online Store only, behind the store password (brief said draft) | Draft products don't show in theme previews. All six tagged `test`; delete before the password comes off |
| 2026-10-04 | New pages under new handles (about, questions, care, shipping-and-delivery, returns) with vault-verified copy only. Existing pages (our-story, faq, shipping, materials-care, size-guide, gifting) left untouched | Existing pages contain claims the vault doesn't support (UK/EU shipping, "a person answers", unconfirmed materials, "Gifts under $100"). Founder decides whether to delete them |
| 2026-10-04 | Build menus `lumi-build-main`, `lumi-build-help`, `lumi-build-brand` created; older `lumi-*` menus left untouched | Same reason: older menus link to pages and collections that conflict with the vault |
| 2026-10-04 | Product facts on the theme come from metafields `custom.material`, `custom.details`, `custom.size_guide`, filled from Branvas data only | No material claims in theme code |
| 2026-10-03 | Theme: a free Shopify theme, restyled hard to the brand (fonts, palette, spacing, section order, custom sections). Paid theme only if it falls short after the first orders | Founder choice; budget |
| 2026-10-03 | Change-of-mind details confirmed: unworn and in the original box, customer pays return shipping, store credit never expires, no cash refund, returns to our PO box | Founder choice |
| 2026-10-03 | Damaged, defective or incorrect items: free replacement, handled by Branvas and shipped directly to the customer. If a return is needed, the customer uses the address Branvas issues, which carries no Branvas details. Claim window 10 days from delivery (Branvas confirms 10 on its current page) | Founder choice; matches Branvas policy |
| 2026-10-03 | Change-of-mind returns accepted for store credit only, within 7 days of delivery. Supersedes "no change-of-mind returns". Details proposed in [[Policies]] | Founder choice; closes a conversion gap vs competitors. Costs us the piece and shipping |
| 2026-10-03 | Business is based in Canada, not yet registered: no taxes charged, prices include tax. Revisit when GST/HST registration is due | Founder; confirm threshold with an accountant |
| 2026-10-03 | Branvas plan bought once the store design is complete. Fake products added by the founder for theme testing (named "TEST", deleted before launch) | Founder choice |
| 2026-10-03 | Store design: mobile-first, quiet-camp competitors as model (Mejuri, Monica Vinader, Gorjana, Catbird); no popups, countdowns or sale styling. Plan in [[Store Design Plan]]. Nothing built yet | Founder asked for a plan first |
| 2026-10-03 | Observed: Shopify store is Lumi Paris, plan Shopify, base currency CAD, business country Canada, store email hello@thelumiparis.com. Not yet confirmed as intended | Read from Shopify; founder to confirm |
| 2026-10-03 | Brand image and consistency come first: only pieces that pass the Quality Gate are listed; small catalog is fine. Feel: quality wear, subtle, quiet-luxury mood | Founder choice. See [[Quality Gate]] |
| 2026-10-03 | Word of mouth is the growth approach (inspired by The Ordinary). Urgency is felt, never claimed: only true mechanisms (small edit, real stock sync, Notify me, early access, Christmas order-by dates, archive). No fake or hidden scarcity | Founder choice; honesty and advertising rules. See [[Word of Mouth and Urgency]] |
| 2026-10-03 | Pricing (supersedes the cost +75% row below): base price $129.99, nothing listed lower. Unit cost up to $75 lists at $129.99; above $75 lists at cost x 1.75, shipping not included in the 75%. Free shipping for all | Founder choice. Positive contribution at every tier ([[Products Index]]); reading awaiting founder confirmation |
| 2026-10-03 | Pricing target: Branvas unit cost + 75% with complimentary shipping (cost $100 → $175; landed $108.99). Applying the 75% to landed cost instead is recommended and awaiting founder choice | Founder choice. Cheap styles are thin or negative, see [[Products Index]] |
| 2026-10-03 | Pricing tactic: same number in both countries (US$X in the US, CA$X in Canada) on every product. Canada shows a "Canada price" label and Canada-only top bar, no strikethrough or fake discount. Canadian orders bring in about 27% less revenue; accepted | Founder choice. Contribution falls about half, so styles need a Canada floor ([[Products Index]]) |
| 2026-10-03 | Returns remedy (replacement or refund) on hold; returns policy blocked until decided | Founder to decide |
| 2026-10-03 | Ads: organic is primary. First ad test once we reach 20 orders | Founder choice |
| 2026-10-03 | Trademark search deferred until 1,000 orders. Supersedes the free self-check row below | Founder choice |
| 2026-10-03 | Support is AI: email bot plus website chatbot. If asked, say so plainly; never claim to be human | Founder choice; honesty |
| 2026-10-03 | Shipping is complimentary to customers. We absorb Branvas's $8.99 flat fee, so prices must cover it | Founder choice |
| 2026-10-03 | Currency: USD for the US, CAD for Canada. Founder has a pricing marketing tactic, ideas pending | Founder choice |
| 2026-10-03 | Customer-facing spelling is US "jewelry". Applied across the vault, including the approved name line ("Paris is how we look at jewelry, not where we're based") | Founder choice; US and Canada |
| 2026-10-03 | Fonts: Cormorant Garamond for headlines and any text-set wordmark; Outfit for body, buttons, prices; Outfit letter-spaced caps for small labels only | Founder choice |
| 2026-10-03 | U-to-M monogram can be an avatar (tentative; founder unsure) | Founder choice |
| 2026-10-03 | Payments: Shopify's built-in payments. Shopify trial started; Google Workspace bought; Branvas plan pending until the build starts | Founder choice |
| 2026-10-03 | No Branvas samples. The funds go to paying Branvas for orders once customers have paid. Product quality and delivery times are learned from the first real orders | Founder choice; keeps spend minimal. Risk: AI images rely on Branvas product photos, so first-order checks matter |
| 2026-10-03 | Trademark: free self-check only (USPTO, CIPO, web, socials); no filing or lawyer for now (recommended; founder to confirm) | Budget; check is cheap, filing can wait for traction |
| 2026-10-03 | Budget: Branvas plan $30, AI credits $50, Shopify $3 (3-month trial), Google Workspace $10, rest free. No ad budget; organic first | Small business, minimal capital. See [[Budget]] |
| 2026-10-03 | Business email hello@thelumiparis.com (Google Workspace) | Founder choice |
| 2026-10-03 | Branvas Growth plan, bought when building starts | Publish up to 75 styles; enough for launch |
| 2026-10-03 | Launch capsule of 12 to 24 quiet-glow styles (Sterling Luna, Sterling Glow, Steel Edit, Moissanite Spark, Feminine Aura); skip gothic, boho, statement, men's (proposed, founder to judge) | Fits positioning and voice |
| 2026-10-03 | Promises follow Branvas: US 5 to 8 and Canada 7 to 10 business days; returns only for damaged, defective or incorrect items; no change-of-mind returns; no warranty | Policies cannot promise more than the supplier covers |
| 2026-10-03 | Claim window 10 days from delivery until Branvas confirms (its pages say both 10 and 30) | Use the shorter window |
| 2026-10-03 | Material wording: "gold-plated" only, water-safe only for stainless steel, no hypoallergenic/eco/sustainable/handmade claims unless Branvas confirms | FTC Jewelry Guides, honesty |
| 2026-10-03 | All imagery and video AI-generated, no real people or photoshoots; people wearing plus close-ups; AI people never shown as customers; reviews from real buyers only | Founder choice; honesty |
| 2026-10-03 | Tagline: "Wear the light." Secondary: "Glow, not glitter." (social captions only) | Founder choice |
| 2026-10-03 | Customer: women 18 to 40, for themselves and gifting. Markets: US and Canada | Founder choice |
| 2026-10-03 | Reference brands: Mejuri, Missoma, Monica Vinader, Ana Luisa, Gorjana, Astrid & Miyu, EVRY Jewels, Aurate, En Route, Catbird. Avoid glitzy and discount-style | Founder choice |
| 2026-10-03 | Palette final: Lumi Cream #F7F2EA, Ivory Soft #EFE6D8, Warm Ink #1C1917, Champagne Hint #C4A574 (thin accents only), Stone Mist #A8A29E (borders only), Stone Text #6B645F (labels), Jardin Green #2C3A35 (one element per page) | Stone Mist fails text contrast (2.3:1); "Deep Atelier" renamed Jardin Green to avoid an atelier claim |
| 2026-10-03 | Positioning "luminous everyday jewellery, meant to be lived in"; art direction light first, logo second; voice calm, honest, plain | Founder choice |
| 2026-10-03 | Approved name line, word for word: "Lumi comes from lumière: light. Paris is how we look at jewellery, not where we're based." Never use "from Paris", "Parisian-made", "Paris, France", or Paris landmarks as origin proof | Honesty |
| 2026-10-03 | Address placeholders: `[BUSINESS ADDRESS]`, `[PO BOX / RETURNS ADDRESS]`, `[SHIP-FROM LOCATION]` replace `[ADDRESS TBD]`; nothing publishes without a real address | Pending founder |
| 2026-10-03 | TikTok handle is lumiparis (earlier typo corrected) | Founder confirmed |
| 2026-10-03 | Name is "Lumi Paris", never "The Lumi Paris" | Brand consistency |
| 2026-10-03 | "Paris" is a lens, not a place; no French studio/atelier claims | Honesty |
| 2026-10-03 | Operations run by AI; customers need not know | Founder choice |
| 2026-10-03 | Supplier Branvas; domain thelumiparis.com | |
| 2026-10-03 | Launch before Fri 9 Oct 2026; goal 50k orders by Christmas 2026 | |
| 2026-10-03 | Address/PO box undecided: use placeholders | Pending |
