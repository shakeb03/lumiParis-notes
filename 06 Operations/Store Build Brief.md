---
type: ops
status: ready-for-build
updated: 2026-10-03
---
# Store Build Brief

Everything a fresh session needs to build the Lumi Paris store. Read `CLAUDE.md` first, then this note. Context: [[Store Design Plan]], [[Shopify Setup]], [[Brand Bible]], [[Voice and Rules]], [[Products Index]], [[Policies]].

## Non-negotiables
- Work only in an unpublished theme copy. Never edit or publish the live theme without the founder's approval in chat
- Nothing goes live while the store password is on; the founder removes it
- No product, material or review claims that are not in the vault. No popups, countdowns, sale styling or "limited" wording ([[Voice and Rules]])
- Address placeholders stay: `[BUSINESS ADDRESS]`, `[PO BOX / RETURNS ADDRESS]`, `[SHIP-FROM LOCATION]`. Never invent one. Do not show them on any live page
- Never mention Branvas on the storefront, in emails or in code comments visible to customers
- Founder judges the look on a phone; log every build decision in [[Decisions Log]] and update [[Task Tracker]]

## Environment
- Store: Lumi Paris, thelumiparis.com, base currency CAD, business country Canada, store email hello@thelumiparis.com
- Themes (2026-10-03): Horizon (live, unmodified), "Lumi Paris — draft" and "Lumi Paris — custom" (unpublished, origin unknown, do not modify or delete until the founder says)
- Needs a Shopify connector in the session with theme, product, content, navigation and Markets access. If it is missing, write the code into `04 Assets/build/` and tell the founder where to paste it
- Cannot be done by Claude: payments, tax, currency, domain, policy text, installing the Branvas app ([[Shopify Setup]])
- Method: duplicate Horizon into a new unpublished theme named "Lumi Paris — build". Edit there. Preview by theme preview link on a phone

## Design tokens (CSS)
```css
:root {
  --lumi-cream: #F7F2EA;   /* page background */
  --ivory-soft: #EFE6D8;   /* cards, bands */
  --warm-ink: #1C1917;     /* text, buttons */
  --stone-text: #6B645F;   /* secondary labels */
  --stone-mist: #A8A29E;   /* borders, dividers only, never text */
  --champagne: #C4A574;    /* hairlines, icons only, never text or large fills */
  --jardin: #2C3A35;       /* rare accent, one element per page */
  --font-heading: "Cormorant Garamond", Georgia, serif;
  --font-body: "Outfit", system-ui, sans-serif;
  --radius: 2px;
}
```
- Headings: Cormorant Garamond 500, mobile h1 about 40px, line height 1.05. Body: Outfit 300 or 400, 16px, line height 1.6. Prices: Outfit 400
- Small labels only: Outfit 400, 11 to 12px, uppercase, letter spacing 0.14em, colour stone-text
- Buttons: Warm Ink background, Lumi Cream text, Outfit 500 in normal case, 52px high, full width on mobile, radius 2px. Secondary: 1px Warm Ink outline. Visible focus ring
- Cards on Ivory Soft. Borders 1px stone-mist. Decorative rules 1px champagne. Generous space (16, 24, 40, 64px scale)
- Motion: minimal; no autoplay carousels; no hover-only information
- Load fonts with `font-display: swap`; two weights per family at most
- Logo: files in `04 Assets/logo/` (transparent PNG preferred). Header uses a centred logo

## Build spec, mobile first (design at 375px, then scale up)
**Announcement bar (one line):** default "Complimentary shipping to the US and Canada". Canadian visitors only: "Canada price: the same number as our US price, in Canadian dollars. Complimentary shipping." Show by market (`localization.country.iso_code`).
**Header:** centred logo, menu icon left, search and bag right. Sticky.
**Menu:** Shop all · Earrings · Necklaces · Rings · Bracelets · Gifts. Footer: Archive.
**Home, in order:**
1. Hero: one soft-light image (placeholder: Ivory Soft block until AI images exist), headline "Wear the light.", line "Luminous everyday jewelry, meant to be lived in.", button "Shop the edit"
2. Four category tiles
3. The edit: 4 to 6 products in a swipe row with price
4. Three plain facts about materials and care (written from the real catalog once styles are chosen; leave `[FACT FROM BRANVAS DATA]` until then)
5. Brand line: "Lumi comes from lumière: light. Paris is how we look at jewelry, not where we're based."
6. Reviews block, hidden until real reviews exist
7. Early access sign-up, inline, no discount: "Be first to see new pieces." button "Join the list"
8. Footer: Shipping and delivery, Returns, Care, Contact, policies, hello@thelumiparis.com. No address until real
**Collection:** two-column grid. Card: image, name, material line, price, quick add. Filters: category, material. No sale styling. Badge "New" only
**Product page:** swipe gallery (5 to 6), name, price (Canada shows "Canada price" label and line "The same number as our US price, in Canadian dollars."), short description, variants, sticky Add to bag, wallets, reassurance row ("Complimentary shipping · Delivery 5 to 8 days US, 7 to 10 days Canada · 7-day returns for store credit · Gift-ready box"), accordions (Details, Materials and care, Shipping and returns), "Wear it with" row, size guide for rings and bracelets, reviews when real
**Cart:** slide-out bag, line "Complimentary shipping", wallets first. Currency always clear (US$ or CA$)
**Password page (until launch):** "Lumi Paris is opening soon. Wear the light." with the early access sign-up
**Pages:** About (name story), Contact (email, reply within 24 hours), FAQ, Care, Shipping and delivery, Returns. Policy text is pasted by the founder into Shopify policies

## Draft FAQ (verified facts only)
- Where do you ship? The United States and Canada.
- How much is shipping? Complimentary on every order.
- How long does delivery take? Usually 5 to 8 business days in the US and 7 to 10 in Canada.
- What if I change my mind? Return it within 7 days of delivery, unworn and in its original box, for store credit that does not expire. You cover return shipping.
- What if something arrives damaged, defective or incorrect? Write to hello@thelumiparis.com within 10 days of delivery with your order number and photos. We send a free replacement.
- How do I care for my jewelry? Keep pearls dry. Silver tarnishes in humidity, so store it dry and wipe it with the cloth in the box. Plated pieces wear at contact points. Only pieces marked water-safe are made for water.
- Is Lumi Paris based in Paris? Lumi comes from lumière: light. Paris is how we look at jewelry, not where we're based.
- Do not add a "duties included" line until the first Canadian order confirms it

## Markets and shipping
- US market: USD. Canada market: CAD. Fixed prices per market, the same number in both ([[Products Index]] for the pricing rules)
- Free shipping rate for both markets. Delivery windows as above
- Prices include tax while the business is unregistered. Do not add tax lines

## Collections
Earrings, Necklaces, Rings, Bracelets, Gifts, Archive (hidden from main nav). All pieces must pass the [[Quality Gate]] before being listed

## Test products
Name "TEST - ...", tag `test`, status draft. Placeholder images only. No material claims. Delete all before launch

## Acceptance checklist
- [ ] Looks right at 375px; text readable; tap targets at least 44px
- [ ] Palette and fonts exactly as the tokens; Stone Mist never used for text
- [ ] No popups, timers, sale badges or "limited" wording anywhere
- [ ] Canada bar and "Canada price" label show only to Canadian visitors
- [ ] Sticky Add to bag works; wallets show
- [ ] Mobile page speed checked; images compressed
- [ ] Placeholders hidden or replaced; no test products published
- [ ] Opens correctly in the Instagram, TikTok and Pinterest in-app browsers
- [ ] Founder approved on a phone

## Still needed from the founder
Branvas plan (product import), launch style approval, address, PO box, phone number, Shopify Payments, policy text pasted, AI images ([[Imagery Prompts]]).
