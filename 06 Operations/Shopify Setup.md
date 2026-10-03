---
type: ops
status: draft
updated: 2026-10-03
---
# Shopify Setup (build brief)

## Current store (read from Shopify 2026-10-03)
- Name: Lumi Paris. Domain: thelumiparis.com (appears connected; verify). Store email: hello@thelumiparis.com
- Plan: Shopify (trial). Timezone: EDT
- **Base currency: CAD. Business country: Canada.** Confirm this is intended #founder. Base currency cannot be changed once orders exist

## Build order
1. **Confirm basics #founder:** business country, real business address (`[BUSINESS ADDRESS]`, `[PO BOX / RETURNS ADDRESS]`, `[SHIP-FROM LOCATION]`), tax registration (GST/HST in Canada; US sales tax once volume grows; ask an accountant)
2. **Buy Branvas Growth plan** #founder, install the Branvas app, connect to Shopify ([[Branvas]])
3. **Theme:** (plan in [[Store Design Plan]]) a free Shopify theme restyled to [[Brand Bible]]: Lumi Cream background, Ivory Soft bands, Warm Ink buttons, Cormorant Garamond headlines, Outfit body. If a font is missing from the library, add it in theme code
4. **Markets:** US in USD, Canada in CAD, fixed prices per market, same number in both ([[Products Index]]). Canada-only "Canada price" label and top bar ([[Voice and Rules]]). Check the theme can show them by market
5. **Shipping:** complimentary for US and Canada. Delivery windows from [[Branvas]]
6. **Pages:** Home, About (approved name line), Contact, FAQ, care guide, policies ([[Policies]])
7. **Products:** only styles that pass the [[Quality Gate]] and the founder's look check. Titles, copy, AI images ([[Imagery Prompts]]). Material wording exact
8. **Collections and navigation:** small and calm. Archive page for retired pieces
9. **Email list and Notify me:** early access sign-up; Notify me on out-of-stock pages. Check free options against the [[Budget]]. Canadian anti-spam rules (CASL) apply to marketing email: use clear opt-in consent
10. **Support:** email bot on hello@, chatbot on site ([[Support Playbook]])
11. **Payments and checkout:** Shopify Payments activated #founder; test order end to end including Branvas routing
12. **Go live:** remove store password, post launch content ([[Launch Checklist]])

## Settings to check
- Store currency CAD means US orders are paid out after USD to CAD conversion, and Branvas bills in USD. Re-run the contribution table in [[Products Index]] once the real fees are visible
- Checkout shows "Canada price" currency clearly (CA$)

## Claude's access to Shopify (checked 2026-10-03, read-only)
- **Can read and write (by granted scopes):** theme files (Liquid, CSS, JSON templates, sections, settings), products, collections, pages and blog content, navigation menus, Markets, shipping, files and images, translations, checkout branding, discounts, returns settings, metaobjects
- **Cannot:** activate payments, change store currency, plan or domain, set up taxes, install apps (Branvas app install is the founder's), or edit legal policy text (read only)
- **Not tested:** no writes made yet. Work happens in an unpublished theme copy. The live theme is changed only after founder approval
- **Themes found:** Horizon (live, Shopify's free theme, unmodified), "Lumi Paris — draft" (unpublished), "Lumi Paris — custom" (unpublished, last updated 2026-09-26, small custom theme). Origin of the last two to confirm with the founder #founder
- **Preview:** the built-in browser needs site approval per page; the founder can preview on a phone
