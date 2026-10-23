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
├── japan_itinerary.md         ← Full day-by-day itinerary: flights, transport, activities, meals
└── japan_winter_sakura.md     ← DRAFT: Feb–Apr 2028 snow + sakura option, decision checklist
```

---

## 👤 Trip Profile

| Field | Value |
|---|---|
| Traveler | Luis (luis.juarez2394@gmail.com) |
| Departure city | Guatemala City, Guatemala (GUA) |
| Trip duration | ~30 days |
| Target season | ❄️ Winter — **2028-01-07 → 2028-02-04** (on `main`; the `sakura` branch keeps the cherry blossom 2027 plan) |
| Key interests | Martial arts, manga/anime, cultural & historical sites, food, **snowboarding** |
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
| `japan_poi.md` | ✅ Complete (v4) | Okinawa removed; Nagano & Hakuba added; sumo + Shirakawa-go; ⏱️ time + 💴 fees |
| `japan_trip_overview.md` | ✅ Complete (v2) | Winter route, no-JR-Pass transport plan, winter events, links |
| `japan_budget.md` | ✅ Complete (v4) | 10 tabs; snowboarding in TAB 5; grand total $6,951–$14,517; savings $550/mo to Jan 2028 |
| `japan_days_per_city.md` | ✅ Complete (v3) | Tokyo 7d, Nagano 1d, Hakuba 4d, Kanazawa 3d, Kyoto 6d; dated 28-day calendar |
| `japan_references.md` | ✅ Complete (v3) | Okinawa removed; Hakuba, Snow Monkeys, sumo, Shirakawa-go added |
| `japan_todo.md` | ✅ Complete (v2) | Winter 2028 deadlines; no JR Pass; ski lodging, sumo, rentals |
| `japan_itinerary.md` | ✅ Complete (v2) | Day 0–29 winter route; PDF export is stale (still the spring plan) |
| `japan_winter_sakura.md` | 📝 Draft (v1) | Decision draft: Feb 20 – Apr 4, 2028 snow + sakura trip; compares all 3 plans; not yet adopted |
| Packing list | 🔲 Not started | Will be `japan_packing.md` |
| Bookings tracker | 🔲 Not started | Will be `japan_bookings.md` |
| Flights (booked) | 🔲 Not started | Fill into `japan_budget.md` TAB 1 when purchased |

---

## 🧠 Research Done So Far

### Flights (GUA → Tokyo)
- Off-peak baseline: ~$672 one-way / ~$1,095 RT
- Mid-January is close to off-peak (avoid late-Dec/early-Jan holiday peak)
- Budget target: $1,000 (low) → $1,700 (high) RT economy
- No direct flights; always 1–2 stops via US hubs (LAX, DFW, IAH)
- Best airlines: United (via IAH/LAX), American + JAL codeshare
- Best booking window: October–November 2027 (for January 2028)
- Sources checked: Expedia, Kayak, Cheapflights, Kiwi.com, Google Flights

### In-Japan Costs
- Pulled from `japan_trip_overview.md` and travel research
- **No 30-day JR Pass exists** (7/14/21-day only). On the winter route, point-to-point Shinkansen (~$440–500) beats the 21-day pass (¥100,000); Hokuriku Arch Pass (¥35,000/7d) doesn't pay off either
- Hakuba lift tickets (2025/26): Happo-one ~¥8,400/day, Hakuba Valley ~¥10,400/day
- Snow Monkey Park: ¥800; date-specific advance ticket required Dec–Mar
- January sumo tournament starts the 2nd Sunday of January → expected Jan 9–23, 2028; tickets on sale ~early December
- Daily food budget: $30–60/day mixing convenience + restaurants
- Accommodation: $50–100/night for business hotels

---

## 🔜 Next Steps (Suggested)

1. **Keep saving** — $550/mo through Dec 2027 (see `japan_budget.md` TAB 10)
2. **Re-point flight alerts** to Jan 7 → Feb 4, 2028 once fares appear (~Feb 2027)
3. **Book Hakuba lodging + Shibu Onsen ryokan** — June 2027
4. **Check Shirakawa-go light-up dates** — announced ~July 2027
5. **Book city hotels** — August 2027 (Kyoto overlaps Chinese New Year, Jan 26)
6. **Book flights** — October–November 2027
7. **Sumo + Ghibli + Snow Monkey tickets** — early December 2027
8. **Regenerate PDFs** of `japan_itinerary.md` and `japan_days_per_city.md` (the current ones show the spring plan)
9. **Build `japan_packing.md`** — winter + snowboard packing list

---

## 💬 How to Work with Claude on This Trip

- **Adding POIs:** Say which city and category, Claude will append to the right section in `japan_poi.md`
- **Updating budget:** Specify the tab and item; Claude will update row + TAB 9 summary
- **Research requests:** Claude will search the web and add sourced data directly into the relevant file
- **New files:** Claude will follow the naming convention `japan_<topic>.md` and add a cross-reference footer
- **Excel export:** When ready, the MD tables in `japan_budget.md` can be copy-pasted into Excel; each `## TAB N` becomes a sheet. The columns are already aligned for this.
