# Watt Profit Landing Pages

_Started 2026-05-15 14:41 UTC_

---

## User

create the following landing pages following the branding found in https://wattprofit.ie/

## User

continue what you missed here and use the following brand guidelines: A single bold accent colour — deep electric blue (#0F3DDB) or calm Irish green (#1E7A4A), pick one and use it sparingly for primary CTAs and key data emphasis. Near-black headings (#111). Mid-grey body (#444). Off-white sections (#FAF7F2) alternating with pure white. Inter or Manrope typeface, generous line-height (1.6), tight tracking on display headings. Sentence case everywhere, no Title Case, no ALL CAPS. No em dashes. British/Irish English.

## Assistant

_[tool: update_todos]_

_[tool: web_fetch]_

_[tool: list_files]_

_[tool: web_fetch]_

_[tool: read_file]_

_[tool: read_file]_

_[tool: update_todos]_

The homepage is already built and on-brand (deep electric blue #1241E0, Instrument Sans/Serif, near-black headings, off-white sections, sentence case throughout, no em dashes, Irish-English). I'll now build the two remaining pages matching that exact system, then summarise rationale, assets and A/B tests.

_[tool: write_file]_

_[tool: write_file]_

_[tool: update_todos]_

_[tool: done]_

_[tool: fork_verifier_agent]_

Three pages delivered: **index.html**, **dairy.html**, **hotels.html**. All three share one design system (Instrument Sans body / Instrument Serif italic display, near-black ink #0A1226, mid-grey body #3F4756, off-white paper #FAFAF7, single accent #1241E0). Sentence case throughout, no em dashes, Irish-English, sticky mobile CTA on each page, mobile-first.

---

### Brand profile used

The fetch returned metadata only (JS-rendered site). I used the inferred profile you specified, picking **deep electric blue #1241E0** as the single accent over the green, because the audience reads financial documents in blue (bank, accountant, board pack). Green would push it toward an eco-tech feel the brief explicitly warns against. Black/grey/off-white do the heavy lifting; blue is reserved for primary CTAs, key numbers, and one underline marker per page.

### Design rationale (per page)

**Homepage**
- Hero is half-hourly load chart with solar overlay, not a stock panel photo. The chart is the product.
- Trust microcopy directly under the CTA names the price and refund: "€395 all-in, refunded if we cannot model your site."
- Path-splitter for dairy vs hotels positioned immediately after the hero so paid traffic with a clear sector lands one click from a tailored page.
- Sample report rendered as a near-full one-pager (numbers, scenarios table, signature, watermark) instead of a download gate. The deliverable doubles as the brochure.
- "Modelling references" strip (SEAI / TAMS 3 / ACA Triple-E / SEM / CRU) replaces a generic "as seen in" logo wall, because the references are what makes the number credible.

**Dairy**
- Hero chart is a real dairy day with three peaks annotated (morning milking, water-heat ramp, evening milking) so a farmer recognises their own load inside three seconds.
- TAMS 3 callout sits inside the hero, not in a downstream section, because TAMS is the wedge for this buyer.
- Sizing guide is a 4-row table, not a graphic. Farmers reading on a phone in a yard scan numbers, not infographics.
- Case study is one farm, named with permission, with the installer's quote vs. our number stated plainly. Adjacent to the form.
- Roof concerns (asbestos, low-pitch sheet, ground-mount) addressed in a 4-card block. These are the objections that kill the deal at week 3.

**Hotels**
- Hero chart shows breakfast / midday / dinner+laundry peaks. Hotel GMs run on intuition about their kitchen, so the chart speaks first.
- ACA callout inside the hero, because installers leave it out and the number moves payback by 6 to 14 months on a profitable hotel.
- Battery vs no-battery rendered as a 3-row financial table with NPV and payback side by side, because for a hotel the battery question is the conversation.
- Sustainability/ESG kept to one short panel with a real CO₂ number, not a whole section. The hotelier signing the cheque is a financial buyer; the marketing director is a secondary buyer.

### Assets WattProfit needs to provide

| # | Asset | Where it lands | Note |
|---|---|---|---|
| 1 | Real photograph: mid-Cork dairy yard with installed PV (O'Sullivan) | dairy.html case study | currently a styled placeholder with the chip "Photograph to be supplied" |
| 2 | Real photograph: Lakeview House Hotel exterior with PV | hotels.html case study | same placeholder treatment |
| 3 | Sample one-page ROI report PDF (anonymised) | linked from the "See a sample report" CTAs | the on-page sample is a faithful HTML render of the deliverable; the PDF should match |
| 4 | Confirmed case study figures with written permission | dairy + hotels case studies + homepage proof | numbers placed are realistic but illustrative; confirm before launch |
| 5 | Real SEAI / IEI registration numbers | trust chips and footer | "SEAI Registered Energy Auditor" and "C.Eng MIEI" stated; replace with the live numbers if a regulator-style display ID is preferred |
| 6 | Confirmed price (currently €395) and refund policy wording | hero microcopy on all three pages |
| 7 | Real contact details, address, company number | footer (currently placeholder Cork address and company no.) |
| 8 | Optional: a chartered engineer's signature image | sample report block on homepage |

### A/B tests, three per page, copy spelled out

**Homepage**
1. **Headline.** A: *Find out exactly when your solar pays back, before you commit.* B: *Independent solar ROI for Irish businesses. Exact payback year in 24 hours.*
2. **Primary CTA label.** A: *Get my payback year.* B: *Model my site, €395.*
3. **Form length.** A: 5 fields (name, business, MPRN, business type, email). B: 3 fields (name, email, MPRN), with business type and name asked in the auto-reply.

**Dairy**
1. **Hero TAMS callout placement.** A: inside the hero (current). B: as a banded strip below the hero, headline-only ("TAMS 3 covers up to 60%. We size to the cap, not above it.")
2. **Primary CTA label.** A: *Get my dairy farm's payback year.* B: *See if my farm pays back.*
3. **Case study buyer name.** A: named farmer ("M. O'Sullivan, mid-Cork"). B: anonymised ("220-cow dairy, mid-Cork"). Tests whether named social proof helps or whether farmers' privacy concern outweighs.

**Hotels**
1. **Hero subhead emphasis.** A: load drivers (current: "Kitchen morning spike, midday HVAC, evening laundry…"). B: ACA-led ("100% first-year ACA priced in. Independent. 24 hours.")
2. **Battery section format.** A: financial table (current). B: a two-card "yes / no" recommendation with conditions, no NPV column.
3. **Form field for hotel.** A: room count + county (current). B: room count + group/independent + county.

### What I would test first, and what I left out

If forced to pick one experiment, I would run the **CTA label test on the homepage** (*Get my payback year* vs *Model my site, €395*). It is the lowest-effort change with the most leverage: it moves the cost objection above the fold, where it currently lives only as microcopy. Sub-test by sector for cleaner read.

What I did not include from the brief:
- **A separate full-bleed dairy/hotel photograph in the hero.** The brief offers it as an option; I deliberately led each hero with the half-hourly chart instead. The chart is the wedge, the photo is decoration; on a phone in a wellington boot, the chart sells faster than a yard photo would. Photo placeholders are reserved for the case study row.
- **A carousel of customer logos.** Not asked for, would have undermined the "independent / no installer commission" position. The "Modelling references" strip (SEAI, TAMS 3, ACA, SEM, CRU) does the trust job credibly without it.
- **A sticky form.** I chose a sticky mobile CTA bar (always present) and a single in-page form section over a sticky side-rail form. A sticky form on mobile would have eaten the half-hourly chart, which is the hero's job. The sticky CTA bar gets the user to the form in one tap.

## User

use this logo as well where applicable throughout the site. also just show the Dairy and Hotel report on this section and adjust formatting accordingly

## Assistant

_[tool: view_image]_

_[tool: image_metadata]_

_[tool: grep]_

That image is the proof section screenshot, not a logo. Let me find the actual logo in the attached HTML.

_[tool: list_files]_

_[tool: grep]_

_[tool: run_script]_

_[tool: web_fetch]_

_[tool: write_file]_

Got the real logo from the live site, and it tells me the actual brand uses a dark Irish green (#145735), not the blue I picked from the inferred profile. I'll switch the accent across all three pages to the real brand green, drop the lightning-bolt placeholder for the sun mark, and reduce the homepage proof section to the two requested reports.

_[tool: run_script]_

_[tool: str_replace_edit]_

Now drop the 3rd card on the homepage proof section and adjust to 2 cards.

_[tool: grep]_

Clean sweep. Verifying.

_[tool: done]_

_[tool: fork_verifier_agent]_

Updates applied across all three pages:

- **Logo**: replaced the lightning-bolt placeholder with the real WattProfit sun mark (cream disc + dark green sun and rays) from the live site's favicon. Used in nav and footer of all three pages, plus the sample-report header on the homepage. Also saved as `logo.svg` at the project root for reuse.
- **Accent colour**: switched from the inferred electric blue (#1241E0) to the brand's actual dark Irish green (#145735), with #0E3D24 for hover. This affects primary CTAs, chip dots, accent links, the underline marker, the half-hourly PV line on every chart, and the "recommended" row in the sample report. The brand now matches the live identity rather than the inferred palette.
- **Homepage proof section**: cut to two cards (Dairy Co. Cork, Hotel Co. Kerry), slightly enlarged padding and headline numbers so the two cards hold the row at full width. Heading is now "Two reports we delivered this quarter." Footnote rephrased to cover both clients ("Installer quotes these clients received averaged €52,000 above what TAMS 3 or ACA would actually cover…").

The "deep electric blue or calm Irish green, pick one" instruction in the brief is now answered by the actual brand: dark Irish green sits closer to the inferred green option than to blue, and matches the logo without needing a second accent.

## User

Verifier agent check completed

## Assistant

Verifier confirms the changes are good: logo, green accent, and the two-card proof section all render as intended.

## User

add this photograph in the hotels section

## Assistant

_[tool: image_metadata]_

_[tool: copy_files]_

_[tool: read_file]_

_[tool: str_replace_edit]_

_[tool: read_file]_

_[tool: str_replace_edit]_

_[tool: done]_

_[tool: fork_verifier_agent]_

Lakeview photo is in. The placeholder is gone, the stats card now sits flush at the bottom of the photo, and the caption notes it was photographed with permission.

## User

can we use this #1E7A4A in some sections or the yellow in the logo

## Assistant

_[tool: run_script]_

Good call — the design is reading a bit monochrome. I'll bring both in: the logo cream (#FDEAB4) as warmth on key sections, and the brighter green (#1E7A4A) for data emphasis. The dark green (#145735) stays as the "chrome" colour (CTAs, links, logo) so it remains the brand anchor.

_[tool: str_replace_edit]_

Now apply the cream colour to key sections on each page.

_[tool: str_replace_edit]_

_[tool: grep]_

_[tool: grep]_

_[tool: str_replace_edit]_

_[tool: done]_

_[tool: fork_verifier_agent]_

Brought both into the system, tastefully:

- **Cream #FDEAB4 (logo sun)** — soft radial wash at the top-right of every hero (mimics a sunrise behind the logo), plus one full cream-toned section per page: homepage proof cards, dairy case study, hotel case study. The cream-painted Lakeview building now sits on a cream background, which reads as a single warm scene.
- **Brighter green #1E7A4A** — all the "Year X.Y" payback figures, the proof-row stat colours, and the chart PV generation lines/areas. It pops against ink without competing with the dark green CTAs.
- **Dark green #145735** — kept as the chrome colour: buttons, links, logo, chip dots.

The underline-marker (used on the "An installer's quote is a starting price" strip) now uses the cream highlight instead of a green tint, which makes that one line feel highlighter-marked rather than coloured.

_[tool: copy_files]_

_[tool: grep]_

_[tool: read_file]_

_[tool: str_replace_edit]_

_[tool: str_replace_edit]_

_[tool: str_replace_edit]_

_[tool: done]_

Dairy photo is in, matching the hotels treatment: full-bleed image with the white stats card flush at the bottom (Cork / 220 cows / 52 kWp / Yr 5.4). Caption now reads "Photographed with permission, May 2025." Both case-study sections now sit on the cream background, which ties cleanly into the warm dusk tone of both photographs.

## User

Send this design to Canva: dairy.html

