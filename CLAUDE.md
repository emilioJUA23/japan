# CLAUDE.md — Japan Trip Planning Guide

> This file tells Claude how this trip is being built: file structure, conventions, formatting rules, and what's been done so far.

---

## 📁 File Structure

```
japan/
├── CLAUDE.md                  ← You are here; project conventions for Claude
├── japan_poi.md               ← Points of Interest grouped by city → category (incl. time + entry fees)
├── japan_trip_overview.md     ← Route, logistics, transport, key events, useful links
├── japan_budget.md            ← Full budget tracker; Excel-ready format
├── japan_days_per_city.md     ← Days needed per city with suggested day breakdowns & calendar
├── japan_references.md        ← YouTube videos & articles for every POI (for research & decisions)
├── japan_todo.md              ← Master checklist: reservations, flights, hotels, vaccines, purchases
└── japan_itinerary.md         ← Full day-by-day itinerary: flights, transport, activities, meals
```

---

## 👤 Trip Profile

| Field | Value |
|---|---|
| Traveler | Luis (luis.juarez2394@gmail.com) |
| Departure city | Guatemala City, Guatemala (GUA) |
| Trip duration | ~30 days |
| Target season | Cherry Blossom — late March to early April 2027 |
| Key interests | Martial arts, manga/anime, cultural & historical sites, food |
| Passport | Guatemalan — visa-free entry to Japan up to 90 days |

---

## 📐 File Conventions

### General
- All files are **Markdown (.md)**
- Dates use **ISO format**: `YYYY-MM-DD`
- All monetary values in **USD** unless explicitly noted
- JPY exchange rate assumption: **¥150 = $1 USD** (verify before trip)
- Each file ends with a cross-reference footer linking to the other files
- Footer includes `Last updated: YYYY-MM-DD`

### `japan_poi.md` — Points of Interest
- **Structure:** City (H2) → Category (H3) → Table of POIs
- **Category order within each city:**
  1. ⛩️ Temples & Shrines
  2. 🏛️ Cultural & Historical
  3. 🥋 Martial Arts
  4. 🎌 Manga, Anime & Pop Culture
  5. 🌿 Nature & Parks
  6. 🍜 Food & Markets
  7. 🎡 Entertainment
  8. 🏙️ Modern & Architecture
  9. 🎭 Traditional Arts & Experiences
- **Table columns:** `Name | Neighborhood/District | Notes`
  - (Neighborhood column omitted when not applicable, e.g. small cities)
- Only include categories that exist for that city — don't add empty sections
- Use **bold** or ⚠️ to flag items that require advance booking

### `japan_budget.md` — Budget Tracker
- **Excel-ready format** — this file will eventually be imported into Excel
- Each `## TAB N —` section maps to one **Excel sheet/tab**
- **Standard columns for expense rows:**
  `Category | Item | Low (USD) | High (USD) | Planned (USD) | Actual (USD) | Notes`
  - Accommodation tab adds: `Nights | Low/Night | High/Night | Low Total | High Total`
  - Food tab adds: `Low/Day | High/Day | Days` before totals
  - Pre-trip tab adds: `Done` (Yes/No)
- **Totals rows** use bold text and repeat Low/High totals only (no formula syntax in MD)
- `Planned (USD)` = fill in when a purchase decision is made
- `Actual (USD)` = fill in after money is spent
- All prices are **numeric only** — no `$` signs, no ranges in a single cell
  - ✅ `1200` | ❌ `$1,200–2,200`
- When updating prices, update both the row and the TAB 9 summary total
- Keep `TAB 9` (Grand Total Summary) in sync whenever any tab changes

### `japan_trip_overview.md` — Logistics & Route
- High-level planning document; not Excel-bound
- Free-form markdown; tables and prose both fine
- Update the suggested route as the itinerary firms up

---

## ✅ What's Been Built So Far

| File | Status | Contents |
|---|---|---|
| `japan_poi.md` | ✅ Complete (v3) | 9 cities (Nagasaki removed); POIs with ⏱️ time + 💴 real entry fees |
| `japan_trip_overview.md` | ✅ Complete (v1) | Route, transport, budget overview, festivals, links |
| `japan_budget.md` | ✅ Complete (v3) | 9 tabs; Nagasaki removed; grand total $7,321–$14,508 |
| `japan_days_per_city.md` | ✅ Complete (v2) | Tokyo 8d, Kyoto 6d; 28-day calendar; Nagasaki removed |
| `japan_references.md` | ✅ Complete (v2) | Videos & articles for all active POIs (Nagasaki removed) |
| `japan_todo.md` | ✅ Complete (v1) | Master checklist: reservations, flights, hotels, vaccines, purchases |
| `japan_itinerary.md` | ✅ Complete (v1) | Day 0–29: full day-by-day with transport, activities, meals, costs |
| Packing list | 🔲 Not started | Will be `japan_packing.md` |
| Bookings tracker | 🔲 Not started | Will be `japan_bookings.md` |
| Flights (booked) | 🔲 Not started | Fill into `japan_budget.md` TAB 1 when purchased |

---

## 🧠 Research Done So Far

### Flights (GUA → Tokyo)
- Off-peak baseline: ~$672 one-way / ~$1,095 RT
- Cherry blossom season premium: +25–40% above baseline
- Budget target: $1,200 (low) → $2,200 (high) RT economy
- No direct flights; always 1–2 stops via US hubs (LAX, DFW, IAH)
- Best airlines: United (via IAH/LAX), American + JAL codeshare
- Best booking window: October–November 2026
- Sources checked: Expedia, Kayak, Cheapflights, Kiwi.com, Google Flights

### In-Japan Costs
- Pulled from `japan_trip_overview.md` and travel research
- JR Pass 30-day: ~$600–670 (must buy before leaving Guatemala)
- Daily food budget: $30–60/day mixing convenience + restaurants
- Accommodation: $50–100/night for business hotels

---

## 🔜 Next Steps (Suggested)

1. **Book flights** — set Google Flights alert for GUA → NRT/HND, target Oct–Nov 2026
2. **Book Ghibli Museum tickets** — go on sale ~3 months ahead; set reminder
3. **Book teamLab Borderless** — book as soon as dates are confirmed
4. **Build `japan_itinerary.md`** — day-by-day schedule with cities, POIs, travel days
5. **Build `japan_bookings.md`** — track all confirmed reservations (flights, hotels, tickets)
6. **Fill in `Planned (USD)` column** in `japan_budget.md` as decisions are made
7. **Verify JPY/USD exchange rate** closer to trip date and update throughout budget

---

## 💬 How to Work with Claude on This Trip

- **Adding POIs:** Say which city and category, Claude will append to the right section in `japan_poi.md`
- **Updating budget:** Specify the tab and item; Claude will update row + TAB 9 summary
- **Research requests:** Claude will search the web and add sourced data directly into the relevant file
- **New files:** Claude will follow the naming convention `japan_<topic>.md` and add a cross-reference footer
- **Excel export:** When ready, the MD tables in `japan_budget.md` can be copy-pasted into Excel; each `## TAB N` becomes a sheet. The columns are already aligned for this.
