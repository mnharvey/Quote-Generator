# Little 6 Industries — Internal Tools

**Veteran-Owned · Maricopa, Arizona · SDVOSB Certified**
> *The Brand Behind the Brand*

This repository contains internal sales and operations tools for Little 6 Industries LLC, operating under three brands: **Little 6 Industries** (B2B), **Transfers42** (DTF e-commerce), and **Promo with Grace** (promotional products).

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `L6I_Quote_Tool_v2.html` | Internal sales quote calculator — all pricing, print-ready quotes, email integration |
| `L6I_Pricing_Master.xlsx` | Master pricing spreadsheet — source of truth for all product pricing |
| `README.md` | This file |

---

## 🧾 Quote Tool (`L6I_Quote_Tool_v2.html`)

A single-file HTML sales tool. No installation, no server, no internet required after download. Open in any browser.

### Features
- **Product calculators** — 4mm Corrugated Signs, 10mm Corrugated Signs, Aluminum Signs, Vinyl Decals, T-Shirts + DTF, Cornhole Trophies
- **Automatic quantity break pricing** — correct tier applied automatically based on qty entered
- **Quote sheet** — add multiple line items, enter customer info, track running total
- **Print quote** — opens a clean branded print sheet with L6I logo and "America's SWAG" tagline
- **Email quote** — opens default email client pre-filled with full quote as plain text
- **Copy quote** — copies plain text to clipboard for pasting into any system
- **Mobile-friendly** — horizontal nav on phones, slide-up quote drawer, works as home screen app
- **Live pricing from Google Sheet** — fetches updated pricing on load if connected (see below)
- **Desktop layout** — three-column view on screens 900px+ (sidebar / calculator / quote sheet)

### How to Use
1. Download `L6I_Quote_Tool_v2.html`
2. Open in Chrome, Edge, or Safari
3. Select a product category from the sidebar or top nav
4. Enter job details and click **Calculate**
5. Click **+ Add to Quote** to add the line item
6. Repeat for additional products
7. Enter customer info in the Quote Sheet
8. Click **Print**, **Copy**, or **Email Quote**

### Mobile / Field Use
In Chrome on iPhone or Android:
1. Open the file
2. Tap the browser menu → **Add to Home Screen**
3. It appears as an app icon — tap to open like any app

### Google Sheet Pricing Connection
The tool can pull live pricing from a published Google Sheet. When connected, pricing updates automatically whenever Lindsay changes a number in the sheet — no code edits needed.

**To connect:**
1. Open `L6I_Pricing_Master.xlsx`, upload to Google Drive (it becomes a Google Sheet automatically)
2. In Google Sheets: **File → Share → Publish to Web → CSV → Publish**
3. Copy the published CSV URL
4. The tool already has the current sheet URL hardcoded — to update it, change the `SHEET_URL` constant at the top of the `<script>` section

**Current sheet URL is configured in the file.** The tool will show `"Pricing loaded from Google Sheet"` in green under the 4mm panel title when the connection is live.

---

## 💰 Pricing Master (`L6I_Pricing_Master.xlsx`)

Eight-tab Excel workbook. Upload to Google Drive to use as a live Google Sheet.

| Tab | Contents |
|-----|----------|
| 📋 Instructions | Who edits what, color legend, how to publish as CSV |
| 🪧 4mm Corrugated | Yard sign pricing — 7 sizes, single/double, qty breaks at 1/10/100/500/1000 |
| 🪧 10mm Corrugated | Heavy-duty sign pricing — 4 sizes, qty breaks at 1/2/5/10/20 |
| 🔩 Aluminum | Per-square-foot rates for .04" and .08", single and double sided |
| 🎨 Vinyl Decals | Per-square-foot rate + application fee |
| 👕 Shirts + DTF | All shirt styles (MSRP/sale/cost), DTF transfer costs, press fees, live formula |
| 🏆 Cornhole Trophies | Tiered pricing 1–100+ pieces, design fee |
| 🔗 Quote Tool Export | Machine-readable tab — **this is the one published as CSV** |

**Color coding:**
- 🟡 Yellow + blue text = editable price (Lindsay updates these)
- ⬜ Gray = key/ID field (do not edit)
- 🟢 Green = calculated formula (do not edit)

---

## 🔧 Making Changes

### Pricing updates (no code needed)
1. Open the Google Sheet version of `L6I_Pricing_Master.xlsx`
2. Find the yellow cell for the price you want to change
3. Update the number
4. Save — the Quote Tool pulls the new price on next load

### Adding new product categories
Requires a code edit to the HTML file. Contact Matt or open an issue in this repo.

### Updating the tool itself
1. Open `L6I_Quote_Tool_v2.html` in a text editor (VS Code recommended)
2. Make changes
3. Test in browser
4. Commit and push to this repo

---

## 🏢 Business Info

| | |
|--|--|
| **Company** | Little 6 Industries LLC |
| **Certification** | SDVOSB (Service-Disabled Veteran-Owned Small Business) |
| **Location** | Maricopa, Arizona |
| **Phone** | 520-705-4026 |
| **Sales email** | sales@little6llc.com |
| **Website** | [little6llc.com](https://little6llc.com) |
| **DTF Store** | [transfers42.com](https://transfers42.com) |
| **Promo Products** | [promowithgrace.com](https://promowithgrace.com) |

---

## 📋 Capabilities

- DTF Transfers (by the foot, gang sheets, wholesale)
- UV Printing (flatbed + roll-to-roll with die-cut)
- Laser Engraving (CO2, UV, Fiber — three systems)
- Custom Stickers (die-cut, kiss-cut, vinyl)
- Decorated Apparel (DTF, embroidery, HTV)
- Corrugated & Aluminum Signage
- Promotional Products (60+ supplier catalog via Promo with Grace)

---

## 🤝 Contributing

This is an internal tool. If you find a bug or want a feature added:
1. Open an issue describing the problem or request
2. Or contact Matt directly

---

*Last updated: March 2026*
