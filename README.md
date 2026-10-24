---
license: cc-by-4.0
task_categories:
  - tabular-classification
  - question-answering
language:
  - en
tags:
  - municipal-solid-waste
  - landfill-tipping-fees
  - bulk-trash-pickup
  - dumpster-rental-costs
  - civic-open-data
  - right-of-way-permits
pretty_name: US Municipal Curbside Bulk Trash, County Landfill Tipping Fees & Roll-Off Dumpster Permit Dataset (2026)
size_categories:
  - n<1K
---

# US Municipal Curbside Bulk Trash, County Landfill Tipping Fees & Roll-Off Dumpster Street Permit Dataset (2026)

**Canonical Source & Interactive Calculator:** [**JunkHaul HQ (`https://junkhaulhq.com/`)**](https://junkhaulhq.com/)  
**Public Repository:** `https://github.com/rtpait/us-municipal-bulk-trash-fees-2026`  
**Dataset Version:** `2026.10.24` (Verified October 24, 2026)  
**License:** [Creative Commons Attribution 4.0 International (`CC-BY-4.0`)](https://creativecommons.org/licenses/by/4.0/)  
**Maintained By:** [JunkHaul HQ Research Team](https://junkhaulhq.com/about/) (*Research Triangle Park AI Transformation LLC*)

---

## 1. Overview & Civic Research Purpose

Municipal solid-waste rules across the United States are fragmented across hundreds of city 311 portals, county landfill fee schedules, and municipal Department of Transportation (DOT) right-of-way ordinances. Homeowners, contractors, property managers, and civic researchers frequently face three hidden friction points:

1. **Zero Municipal C&D Coverage:** Every major US municipal curbside bulk program (`14/14` audited cities) strictly prohibits **Construction & Demolition (C&D)** remodeling debris (drywall, tile, lumber, roofing shingles, carpet tear-outs, and concrete) at the curb.
2. **Wide County Landfill Tipping Fee Dispersion (`$37/ton` to `$85/ton`):** Municipal and county transfer station commercial scale rates vary by more than **2.2x** across metros—from **`$37.00/ton`** at Wake County's South Wake Landfill (`Apex/Raleigh/Cary, NC`) and **`~$38.70/ton`** for Class III C&D in `Orlando, FL` to **`$65.00/ton`** at the City of Durham Transfer Station and **`$55–$85/ton`** at Denver's DADS Landfill.
3. **Street Right-of-Way (ROW) Permit Bonds & Fines:** Placing a roll-off container on a private residential driveway requires **`$0` municipal permit** in all `14/14` audited cities, whereas placing a bin on a public street, curb lane, or alley requires a municipal ROW permit—including a **`$10,000` ROW Bond** in `Austin, TX`, a **`$5,000` bond + 15-day review** in `Raleigh, NC`, a **12–15 business day Accela MOT review** in `Tampa, FL`, and a **`$500` unpermitted street occupancy fine** in `Denver, CO`.

This repository provides a primary-source-verified tabular (`.csv`), nested (`.json`), Frictionless Data (`datapackage.json`), and Schema.org (`dataset-schema.jsonld`) benchmark across **14 metropolitan markets in 6 US states (`TX`, `NC`, `FL`, `GA`, `CO`, `AZ`)**, linking directly to all **64 canonical HTML reference guides** on [`junkhaulhq.com`](https://junkhaulhq.com/).

---

## 2. Files in This Repository

| File Name | Format | Description |
| :--- | :--- | :--- |
| `us-municipal-bulk-trash-and-landfill-fees-2026.csv` | `CSV` (`UTF-8`) | 14-city × 28-column flat tabular dataset ready for Pandas, R, DuckDB, Kaggle, and Hugging Face Datasets. |
| `us-municipal-bulk-trash-and-landfill-fees-2026.json` | `JSON` | Nested structured dataset including full municipal rule arrays, prohibited roll-off items, and all verified `.gov` source citations. |
| `datapackage.json` | `JSON` | Frictionless Data / Kaggle / Open Knowledge Foundation schema descriptor defining all 28 column types and provenance links. |
| `dataset-schema.jsonld` | `JSON-LD` | Schema.org `DataCatalog` + `Dataset` structured data payload for Google Dataset Search indexing. |
| `LICENSE` | `CC-BY-4.0` | Creative Commons Attribution 4.0 International license text. |

---

## 3. Master 14-Metro Comparison Matrix (Verified October 2026)

| Metro (`State`) | County & Primary Disposal Facility | Official Commercial Tipping Rate (`$/Ton`) | Curbside Bulk Pickup Program & Cost | 20-Yd Roll-Off (`7–10 Days`) | Public Street ROW Permit Rule | Canonical City Guides |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Austin, TX** | Travis County (Private Regional Landfills; ARR Drop-Off at 2514 Business Center Dr) | `~$52–$68/ton` (FM 812 closed) | **Free** (up to 3 On-Demand Bulk Pickups/yr via Austin Recycles app) | `$395–$555` (`$65–$85/t` overage) | ATPW AB+C Permit + Insurance + **`$10,000` ROW Bond** | [Austin Bulk Guide](https://junkhaulhq.com/junk-removal/austin-tx/) · [Austin Dumpster Guide](https://junkhaulhq.com/dumpster-rental/austin-tx/) |
| **Dallas, TX** | Dallas County (McCommas Bluff Landfill, 5100 Youngblood Rd) | `~$38–$45/ton` (Free resident self-haul) | **Free** Monthly Brush & Bulky (BABIC) up to `10 cu yd` | `$385–$540` (`$55–$75/t` overage) | Public Works ROW Closure Permit + reflective barricades | [Dallas Bulk Guide](https://junkhaulhq.com/junk-removal/dallas-tx/) · [Dallas Dumpster Guide](https://junkhaulhq.com/dumpster-rental/dallas-tx/) |
| **Houston, TX** | Harris County (Regional Landfills + 6 City Neighborhood Depositories) | `~$45–$65/ton` (Depositories free 4x/mo) | **Free** Even-Month Curbside Junk Waste up to `8 cu yd` | `$390–$550` (`$60–$80/t` overage) | Houston Permitting Center Mobility Permit + Fire Code (>60d) | [Houston Bulk Guide](https://junkhaulhq.com/junk-removal/houston-tx/) · [Houston Dumpster Guide](https://junkhaulhq.com/dumpster-rental/houston-tx/) |
| **Orlando, FL** | Orange County Landfill (5901 Young Pine Rd) & Porter/McLeod Transfer | `~$38.70/ton` C&D / `~$43.60/ton` MSW | **Free** Weekly Large Item Pickup (up to 2 items on yard waste day) | `$380–$535` (`$55–$75/t` overage) | City of Orlando ROW Utilization / Encroachment Permit | [Orlando Bulk Guide](https://junkhaulhq.com/junk-removal/orlando-fl/) · [Orlando Dumpster Guide](https://junkhaulhq.com/dumpster-rental/orlando-fl/) |
| **Tampa, FL** | Hillsborough County (McKay Bay Scale House, 114 S 34th St & SE Landfill) | `~$55–$75/ton` (Free 5 visits/yr for residents) | **Free** Annual SWEEP Curbside Pickup (up to `10 cu yd` by zone) | `$385–$545` (`$60–$80/t` overage) | Accela ROW Permit (**12–15 business days** + COI + MOT Plan) | [Tampa Bulk Guide](https://junkhaulhq.com/junk-removal/tampa-fl/) · [Tampa Dumpster Guide](https://junkhaulhq.com/dumpster-rental/tampa-fl/) |
| **Atlanta, GA** | Fulton & DeKalb (Seminole Rd & Chadwick Rd Landfills + Live Thrive CHaRM) | `~$45–$62/ton` (`$20/mattress` at CHaRM) | **Free** Scheduled Bulk Collection via ATL311 (up to 4 items) | `$390–$550` (`$60–$80/t` overage) | ATLDOT Right-of-Way / Temporary Container Permit | [Atlanta Bulk Guide](https://junkhaulhq.com/junk-removal/atlanta-ga/) · [Atlanta Dumpster Guide](https://junkhaulhq.com/dumpster-rental/atlanta-ga/) |
| **Denver, CO** | Denver County (DADS Landfill, 3500 S Gun Club Rd & Cherry Creek Drop-Off) | `~$55–$85/ton` (Cherry Creek free compost/recyc) | **Free** 4-Week Large Item Pickup (LIP: up to 5 items + 10 bags) | `$405–$565` (`$65–$85/t` overage) | DOTI E-Permits Street Occupancy + TCP (**`$500` unpermitted fine**) | [Denver Bulk Guide](https://junkhaulhq.com/junk-removal/denver-co/) · [Denver Dumpster Guide](https://junkhaulhq.com/dumpster-rental/denver-co/) |
| **Phoenix, AZ** | Maricopa County (27th Ave & North Gateway Transfer Stations -> SR 85) | `$55.00/ton` (`$40` min; 1 ton/mo free resident) | **Free** Appointment-Based Bulk Trash (up to 4x/yr, max `10 cu yd`) | `$385–$540` (or City `$165/pull + $55/t`) | Phoenix City Code Sec. 31-81 Temporary ROW Permit (2–3d notice) | [Phoenix Bulk Guide](https://junkhaulhq.com/junk-removal/phoenix-az/) · [Phoenix Dumpster Guide](https://junkhaulhq.com/dumpster-rental/phoenix-az/) |
| **Charlotte, NC** | Mecklenburg County (Foxhole Landfill, 17131 Lancaster Hwy + 3 Centers) | `$60.00/ton` weighed (`$35` min; `$15–$25` res) | **Free** Scheduled Curbside Bulky Pickup via CLT+ app or 311 | `$385–$535` (`$60–$80/t` overage) | CDOT Cityworks ROW Use Permit (72-hr review + daily fee) | [Charlotte Bulk Guide](https://junkhaulhq.com/junk-removal/charlotte-nc/) · [Charlotte Dumpster Guide](https://junkhaulhq.com/dumpster-rental/charlotte-nc/) |
| **Raleigh, NC** | Wake County (South Wake Landfill, 6300 Old Smithfield Rd + 11 Centers) | `$37.00/ton` MSW (`$15/mattress` shredder fee) | **Paid:** `$35` per `4 cu yd` Bulky Load (`$70` Special Load; Free Mon E-Waste) | `$385–$525` (`$55–$75/t` overage) | Raleigh DOT ROW Occupancy Permit (**15-day review + `$5,000` bond**) | [Raleigh Bulk Guide](https://junkhaulhq.com/junk-removal/raleigh-nc/) · [Raleigh Dumpster Guide](https://junkhaulhq.com/dumpster-rental/raleigh-nc/) |
| **Cary, NC** | Wake County (South Wake Landfill + Citizen's Center 313 N. Dixon Ave) | `$37.00/ton` MSW (`$15/mattress` shredder fee) | **Paid:** `$15` first bulky item + `$8` each additional via Cary 311 | `$390–$530` (`$55–$75/t` overage) | Prohibited on street without Cary 311 ROW authorization | [Cary Bulk Guide](https://junkhaulhq.com/junk-removal/cary-nc/) · [Cary Dumpster Guide](https://junkhaulhq.com/dumpster-rental/cary-nc/) |
| **Durham, NC** | Durham County (City of Durham Transfer Station, 2115 E. Club Blvd) | `$65.00/ton` commercial (`$10–$20` res pickup) | **Free** 1 Bulky Pickup/Week (up to 3 items via Durham One Call) | `$395–$540` (`$65–$85/t` overage) | Durham DOT (DDOT) Street Obstruction Permit required | [Durham Bulk Guide](https://junkhaulhq.com/junk-removal/durham-nc/) · [Durham Dumpster Guide](https://junkhaulhq.com/dumpster-rental/durham-nc/) |
| **Apex, NC** | Wake County (South Wake Landfill, Site 2 & Multi-Material right in Apex) | `$37.00/ton` MSW (`$15/mattress` shredder fee) | **Paid:** `$30` trip fee (1–2 items), `$15/item` (3+), `$15/mattress` Fri | `$380–$515` (`$55–$70/t` overage) | Town of Apex Public Works ROW approval + 20-ft fire lane | [Apex Bulk Guide](https://junkhaulhq.com/junk-removal/apex-nc/) · [Apex Dumpster Guide](https://junkhaulhq.com/dumpster-rental/apex-nc/) |
| **RTP Corridor, NC** | Durham Transfer (`2115 E. Club Blvd`) & Wake Site 3 (`266 Aviation Pkwy`) | `$65.00/ton` (Durham) / `$37.00/ton` (Wake) | Durham side: 3 free items/wk; Morrisville: semi-annual GFL Bulk Week | `$395–$545` (`$60–$85/t` overage) | No parkway placement in RTP covenants; dock/pad staging only | [RTP Bulk Guide](https://junkhaulhq.com/junk-removal/research-triangle-park-nc/) · [RTP Dumpster Guide](https://junkhaulhq.com/dumpster-rental/research-triangle-park-nc/) |

---

## 4. Complete Canonical Directory Index (`64` HTML Reference Guides on `junkhaulhq.com`)

### A. National Hubs, Calculators & Container Size Guides (`9` Pages)
- [JunkHaul HQ — Instant City & 5-Digit ZIP Cost, Landfill Fee & Street Permit Estimator (`/` & `/#city-zip-search`)](https://junkhaulhq.com/#city-zip-search)
- [National State & County Municipal Directory (`/#state-directory`)](https://junkhaulhq.com/#state-directory)
- [Roll-Off Dumpster Rental Cost, Size & Street Permit Hub (`/dumpster-rental/`)](https://junkhaulhq.com/dumpster-rental/)
  - [10 Yard Dumpster Rental Guide: Dimensions (`12' × 8' × 3.5'`), Weight Limit & Cost (`/dumpster-rental/10-yard/`)](https://junkhaulhq.com/dumpster-rental/10-yard/)
  - [20 Yard Dumpster Rental Guide: Dimensions (`22' × 8' × 4.5'`), Weight Limit & Cost (`/dumpster-rental/20-yard/`)](https://junkhaulhq.com/dumpster-rental/20-yard/)
  - [30 Yard Dumpster Rental Guide: Dimensions (`22' × 8' × 6'`), Weight Limit & Cost (`/dumpster-rental/30-yard/`)](https://junkhaulhq.com/dumpster-rental/30-yard/)
- [City-by-City Municipal Bulk Pickup & Landfill Fee Directory (`/junk-removal/`)](https://junkhaulhq.com/junk-removal/)
- [Item-by-Item Bulky Waste & EPA Disposal Guides (`/remove/`)](https://junkhaulhq.com/remove/)
- [About JunkHaul HQ & Editorial Methodology (`/about/`)](https://junkhaulhq.com/about/) · [Affiliate & Partner Disclosure (`/affiliate-disclosure/`)](https://junkhaulhq.com/affiliate-disclosure/)

### B. Item-Specific Disposal, EPA Section 608 & Hauling Guides (`17` `/remove/[item]/` Pages)
- **Furniture, Bedding & Flooring:** [Mattress Removal (`/remove/mattress/`)](https://junkhaulhq.com/remove/mattress/) · [Couch & Sofa Removal (`/remove/couch/`)](https://junkhaulhq.com/remove/couch/) · [Recliner & Lift Chair Removal (`/remove/recliner/`)](https://junkhaulhq.com/remove/recliner/) · [Carpet & Padding Removal (`/remove/carpet/`)](https://junkhaulhq.com/remove/carpet/) · [Piano Removal (`/remove/piano/`)](https://junkhaulhq.com/remove/piano/) · [Pool Table Removal (`/remove/pool-table/`)](https://junkhaulhq.com/remove/pool-table/)
- **Appliances & E-Waste (EPA Sec. 608 / State Bans):** [Appliance Removal (`/remove/appliance/`)](https://junkhaulhq.com/remove/appliance/) · [Refrigerator Disposal (`/remove/refrigerator/`)](https://junkhaulhq.com/remove/refrigerator/) · [Chest & Upright Freezer Disposal (`/remove/freezer/`)](https://junkhaulhq.com/remove/freezer/) · [Washer & Dryer Removal (`/remove/washer-dryer/`)](https://junkhaulhq.com/remove/washer-dryer/) · [Water Heater Removal (`/remove/water-heater/`)](https://junkhaulhq.com/remove/water-heater/) · [TV & Monitor E-Waste Disposal (`/remove/tv/`)](https://junkhaulhq.com/remove/tv/)
- **Heavy Demolition & Outdoor Structures:** [Construction & Remodeling Debris (`/remove/construction-debris/`)](https://junkhaulhq.com/remove/construction-debris/) · [Hot Tub & Spa Removal (`/remove/hot-tub/`)](https://junkhaulhq.com/remove/hot-tub/) · [Shed Demolition & Removal (`/remove/shed/`)](https://junkhaulhq.com/remove/shed/) · [Trampoline Disassembly & Disposal (`/remove/trampoline/`)](https://junkhaulhq.com/remove/trampoline/) · [Treadmill & Exercise Equipment Removal (`/remove/treadmill/`)](https://junkhaulhq.com/remove/treadmill/)

### C. City-Specific Item Disposal Guides (`10` `/junk-removal/[city]/[item]/` Pages)
- **North Carolina:** [Raleigh, NC Mattress Disposal (`/junk-removal/raleigh-nc/mattress/`)](https://junkhaulhq.com/junk-removal/raleigh-nc/mattress/) · [Charlotte, NC Mattress Disposal (`/junk-removal/charlotte-nc/mattress/`)](https://junkhaulhq.com/junk-removal/charlotte-nc/mattress/) · [Cary, NC Appliance Pickup (`/junk-removal/cary-nc/appliance/`)](https://junkhaulhq.com/junk-removal/cary-nc/appliance/)
- **Texas:** [Houston, TX Mattress Disposal (`/junk-removal/houston-tx/mattress/`)](https://junkhaulhq.com/junk-removal/houston-tx/mattress/) · [Houston, TX Couch & Sofa Disposal (`/junk-removal/houston-tx/couch/`)](https://junkhaulhq.com/junk-removal/houston-tx/couch/) · [Austin, TX Mattress Disposal (`/junk-removal/austin-tx/mattress/`)](https://junkhaulhq.com/junk-removal/austin-tx/mattress/) · [Dallas, TX Mattress Disposal (`/junk-removal/dallas-tx/mattress/`)](https://junkhaulhq.com/junk-removal/dallas-tx/mattress/)
- **Georgia, Colorado & Arizona:** [Atlanta, GA Mattress Disposal (`/junk-removal/atlanta-ga/mattress/`)](https://junkhaulhq.com/junk-removal/atlanta-ga/mattress/) · [Denver, CO Mattress Disposal (`/junk-removal/denver-co/mattress/`)](https://junkhaulhq.com/junk-removal/denver-co/mattress/) · [Phoenix, AZ Hot Tub Disposal (`/junk-removal/phoenix-az/hot-tub/`)](https://junkhaulhq.com/junk-removal/phoenix-az/hot-tub/)

---

## 5. Quick Usage Example (Python / Pandas)

```python
import pandas as pd

df = pd.read_csv("us-municipal-bulk-trash-and-landfill-fees-2026.csv")
print(df[["city", "state", "official_landfill_tipping_rate_usd_ton", "dumpster_20yd_7_10_day_range", "junkhaulhq_city_dumpster_guide_url"]])
```

---

## 6. How to Cite This Dataset

```bibtex
@dataset{junkhaulhq_municipal_waste_2026,
  author       = {{JunkHaul HQ Research Team}},
  title        = {{US Municipal Curbside Bulk Trash, County Landfill Tipping Fees & Roll-Off Dumpster Street Permit Dataset (2026)}},
  year         = {2026},
  month        = {10},
  version      = {2026.10.24},
  publisher    = {JunkHaul HQ (Research Triangle Park AI Transformation LLC)},
  url          = {https://junkhaulhq.com/}
}
```
