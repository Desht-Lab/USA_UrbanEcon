# US Metro Niche Clusters — Economic Profiles (V4)

An industry-level economic profile of the **10 niche-metro clusters** produced by the TF-IDF / cosine / Louvain pipeline in `CityNiches_V4_202606.ipynb`, built from CBP-2023 establishment data over 6-digit (MECE) NAICS for the **151 niche metros**. For each cluster it sets out what the group specializes in *as a whole*, the rare specializations that *bind its cities together*, and a sharper name. Clusters are ordered by economic complexity (mean ECI).

## How to read this

- **Specialized / `m_cp`** — a metro is *specialized* in an industry when its payroll-based Revealed Comparative Advantage (RCA) ≥ 1 (its share of that industry exceeds the national average).
- **% metros** — share of the cluster's metros that are specialized in the industry (the shared-ness of the trait).
- **Lift** — `% metros specialized in this cluster ÷ % specialized across all 151 niche metros`. Lift > 1 means the industry is over-represented here; high lift + high % = a defining, *binding* specialization.
- **Exclusivity** — of all niche metros specialized in the industry, the share that sit in this cluster.
- **PCI** — Product Complexity Index of the industry (higher = more knowledge-intensive / less ubiquitous).
- **ECI** — metro Economic Complexity Index; **Niche** — strength of rare-industry specialization (IDF-weighted basket norm); **Avg wage** — annual payroll ÷ employment ($k/worker).

## Cluster overview

| # | Cluster | Metros | Jobs | Avg wage | Mean ECI | Basket PCI | Identity |
|---|---------|-------:|-----:|---------:|---------:|-----------:|----------|
| 6 | **Diversified Industrial & Logistics Powerhouses** | 22 | 31,676,477 | $69k | 3.06 | -0.10 | National tier-1 metros — vast, diversified service economies whose distinctive thread is heavy industrial supply-chain manufacturing. |
| 7 | **Coastal Superstar & Tech-Finance Metros** | 21 | 36,224,228 | $85k | 2.67 | -0.24 | The highest-wage knowledge and finance hubs on the coasts and in the Mountain West. |
| 9 | **Southern New England Hardware & Instruments** | 5 | 1,024,639 | $64k | 1.63 | -0.58 | Five compact New England metros specialised in wire, metal and precision devices. |
| 3 | **Carolina Piedmont Textile & Fiber Belt** | 7 | 1,797,391 | $58k | 1.60 | -0.56 | The most extreme single-industry concentration in the network. |
| 2 | **Great Lakes Precision Metalworking Belt** | 23 | 5,828,382 | $59k | 1.53 | -0.59 | Mid-size legacy industrial metros built on the metalworking trades. |
| 5 | **Gulf Coast Oil, Gas & Petrochemicals** | 10 | 4,672,153 | $70k | 1.36 | -0.57 | The U.S. hydrocarbon value chain, end to end. |
| 4 | **Central Pennsylvania Logistics & Capital Services** | 2 | 504,577 | $56k | 1.36 | -0.66 | A two-metro Pennsylvania pairing — the state capital plus an interstate logistics hub. |
| 8 | **High-Amenity, Knowledge & Tourism Economies** | 43 | 9,172,113 | $72k | 0.99 | -0.79 | The most heterogeneous cluster — capital, college, coast and resort towns bound by amenity and knowledge services. |
| 0 | **Upper-Midwest Paper, Dairy & Food Machinery** | 6 | 673,797 | $57k | 0.96 | -0.77 | Wisconsin's Fox Valley paper-and-food cluster plus kindred small metros. |
| 1 | **Plains Agribusiness, Grain Trade & Insurance** | 12 | 1,368,086 | $61k | 0.62 | -0.89 | The grain-belt agribusiness-and-finance complex. |

> *Basket PCI is the mean complexity of the industries a cluster's metros are specialized in. It is negative for most clusters because RCA-of-payroll surfaces many ubiquitous or resource/consumer-service lines; the **distinctive** tables below isolate the rarer, higher-lift specializations that actually define each group.*

---

## 6. Diversified Industrial & Logistics Powerhouses

*Renamed from “Large diversified metros”.* National tier-1 metros — vast, diversified service economies whose distinctive thread is heavy industrial supply-chain manufacturing.

**22 metros · 31,676,477 jobs · $69k avg wage · mean ECI 3.06 · mean niche 46.5 · basket PCI -0.10**

States: MI (2), OH (2), WI (2), IL-IN (1), TX (1), PA-NJ-DE-MD (1), GA (1), MN-WI (1)

**What binds these cities.** Despite spanning Chicago and Dallas down to Grand Rapids and Madison, these 22 metros share a dense layer of mid-stream industrial manufacturing that rarely co-occurs elsewhere: fluid-power pumps and motors, abrasives, printing ink, petroleum lubricants, springs, and industrial furnaces and process ovens — plus passenger-car leasing and pet-food. None dominate employment (which, as in any big metro, is led by health, retail and hospitality), but their RCA footprint runs ~5x the niche-metro baseline. That is the signature of full, deep production ecosystems rather than any single specialty.

**Reading.** The highest-complexity cluster (mean ECI 3.06) and by far the largest by jobs (31.7M). These are the metros that make a little of everything and anchor national distribution and the capital-goods supply chain. Wages ($69k) are solid but trail the coastal superstars — value here comes from breadth and logistics, not finance/tech rents.

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Fluid Power Pump and Motor Manufacturing | 36% | 5.5× | 1.8 | 80% | 2,422 |
| Abrasive Product Manufacturing | 36% | 5.0× | 1.5 | 73% | 3,185 |
| Passenger Car Leasing | 36% | 5.0× | 1.7 | 73% | 6,384 |
| Printing Ink Manufacturing | 59% | 5.0× | 1.6 | 72% | 4,175 |
| Dog and Cat Food Manufacturing | 46% | 4.9× | 0.4 | 71% | 4,458 |
| Petroleum Lubricating Oil and Grease Manufacturing | 55% | 4.8× | 1.2 | 71% | 3,964 |
| Spring Manufacturing | 55% | 4.8× | 1.2 | 71% | 5,960 |
| Industrial Process Furnace and Oven Manufacturing | 59% | 4.7× | 1.1 | 68% | 3,977 |
| Industrial Truck | 59% | 4.7× | 1.2 | 68% | 5,904 |
| Drive-In Motion Picture Theaters | 46% | 4.6× | 1.1 | 67% | 119 |
| Nonferrous Metal Die-Casting Foundries | 46% | 4.6× | 0.7 | 67% | 7,441 |
| Plastics Bag and Pouch Manufacturing | 55% | 4.6× | 1.0 | 67% | 11,717 |
| Ball and Roller Bearing Manufacturing | 36% | 4.6× | 1.2 | 67% | 4,095 |
| Other Lighting Equipment Manufacturing | 50% | 4.4× | 2.0 | 65% | 1,801 |
| Tire Retreading | 50% | 4.4× | 1.3 | 65% | 1,645 |

**Employment by sector** (top): Health Care & Social Assistance 16% · Retail Trade 11% · Accommodation & Food Services 10% · Manufacturing 8% · Professional, Scientific & Technical 8% · Transportation & Warehousing 6%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Other Lighting Equipment Manufacturing (PCI 2.0), Software and Other Prerecorded Compact Disc (PCI 1.9), Flavoring Syrup and Concentrate Manufacturing (PCI 1.8), Fluid Power Pump and Motor Manufacturing (PCI 1.8), Office Supplies (except Paper) Manufacturing (PCI 1.7), Other Metal Container Manufacturing (PCI 1.7)

<details><summary><b>Member metros</b> (22, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Chicago-Naperville-Elgin | IL-IN | 4,282,854 | $77k | 4.38 | 65.0 |
| Dallas-Fort Worth-Arlington | TX | 3,577,011 | $72k | 3.61 | 54.9 |
| Philadelphia-Camden-Wilmington | PA-NJ-DE-MD | 2,864,094 | $72k | 3.71 | 50.7 |
| Atlanta-Sandy Springs-Roswell | GA | 2,684,526 | $72k | 3.62 | 50.9 |
| Minneapolis-St. Paul-Bloomington | MN-WI | 1,869,491 | $73k | 3.41 | 50.6 |
| Detroit-Warren-Dearborn | MI | 1,839,877 | $68k | 3.57 | 50.0 |
| Riverside-San Bernardino-Ontario | CA | 1,400,038 | $54k | 2.64 | 51.3 |
| St. Louis | MO-IL | 1,247,007 | $66k | 2.93 | 45.4 |
| Charlotte-Concord-Gastonia | NC-SC | 1,220,136 | $69k | 3.32 | 48.4 |
| Pittsburgh | PA | 1,115,840 | $64k | 2.99 | 46.1 |
| Portland-Vancouver-Hillsboro | OR-WA | 1,101,223 | $73k | 2.91 | 49.6 |
| Cincinnati | OH-KY-IN | 1,010,064 | $64k | 3.29 | 46.0 |
| Kansas City | MO-KS | 993,590 | $65k | 2.78 | 43.2 |
| Nashville-Davidson--Murfreesboro--Franklin | TN | 992,254 | $67k | 2.65 | 42.3 |
| Columbus | OH | 967,778 | $61k | 2.50 | 39.0 |
| Indianapolis-Carmel-Greenwood | IN | 967,619 | $64k | 2.38 | 37.5 |
| Cleveland | OH | 949,809 | $66k | 3.98 | 51.0 |
| Milwaukee-Waukesha | WI | 763,309 | $67k | 3.40 | 47.6 |
| Louisville/Jefferson County | KY-IN | 619,819 | $59k | 2.50 | 40.1 |
| Grand Rapids-Wyoming-Kentwood | MI | 518,752 | $57k | 2.51 | 44.0 |
| Allentown-Bethlehem-Easton | PA-NJ | 347,513 | $59k | 2.32 | 36.5 |
| Madison | WI | 343,873 | $68k | 1.98 | 32.1 |

</details>

---

## 7. Coastal Superstar & Tech-Finance Metros

*Renamed from “Superstar tech / finance / knowledge”.* The highest-wage knowledge and finance hubs on the coasts and in the Mountain West.

**21 metros · 36,224,228 jobs · $85k avg wage · mean ECI 2.67 · mean niche 39.8 · basket PCI -0.24**

States: CA (5), FL (3), UT (3), NY-NJ (1), MA-NH (1), AZ (1), WA (1), CO (1)

**What binds these cities.** New York, LA, San Francisco, Boston, Seattle, San Diego, San Jose, Denver and Miami, joined by fast-growing entrants (Phoenix, Salt Lake, Provo, Reno, Huntsville). Their truly defining sectors — finance, software, professional services — are too ubiquitous to register high lift, so the distinctive RCA markers are the adjacent knowledge services that pool where talent concentrates: computer and language training, in-vitro diagnostics, solar generation, specialised information services and ophthalmic goods. The binding trait is a high-wage, human-capital-intensive service base, not any factory specialty.

**Reading.** Highest wages in the network ($85k) and second-largest by jobs (36.2M). Complexity (2.67) sits just below cluster 6 because these economies are service-deep and manufacturing-light — the one place where the method's payroll-RCA lens understates the obvious (finance/tech) and surfaces the rarer tells instead.

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Computer Training | 38% | 4.8× | 0.7 | 67% | 12,189 |
| Gypsum Product Manufacturing | 33% | 4.6× | 1.3 | 64% | 1,855 |
| Language Schools | 48% | 4.0× | 1.0 | 56% | 10,926 |
| In-Vitro Diagnostic Substance Manufacturing | 33% | 3.9× | 1.4 | 54% | 18,060 |
| Metal Household Furniture Manufacturing | 33% | 3.9× | 1.1 | 54% | 1,128 |
| Solar Electric Power Generation | 52% | 3.6× | 0.7 | 50% | 4,442 |
| Ophthalmic Goods Merchant Wholesalers | 48% | 3.6× | 1.3 | 50% | 9,230 |
| All Other Information Services | 38% | 3.6× | 0.7 | 50% | 5,310 |
| Medicinal and Botanical Manufacturing | 52% | 3.4× | 0.6 | 48% | 13,738 |
| Apparel Accessories and Other Apparel Manufacturing | 48% | 3.4× | 0.9 | 48% | 2,532 |
| Footwear Merchant Wholesalers | 38% | 3.4× | 1.3 | 47% | 14,342 |
| Casinos (except Casino Hotels) | 33% | 3.4× | 0.2 | 47% | 20,199 |
| Portfolio Management | 33% | 3.4× | -0.8 | 47% | 199,676 |
| Advertising Material Distribution Services | 33% | 3.1× | 0.8 | 44% | 6,900 |
| Investment Advice | 33% | 3.1× | -0.4 | 44% | 45,546 |

**Employment by sector** (top): Health Care & Social Assistance 16% · Retail Trade 11% · Accommodation & Food Services 10% · Professional, Scientific & Technical 10% · Administrative & Waste Services 6% · Construction 6%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Office Machinery and Equipment Rental and Leasing (PCI 1.4), In-Vitro Diagnostic Substance Manufacturing (PCI 1.4), Gypsum Product Manufacturing (PCI 1.3), Sports Teams and Clubs (PCI 1.3), Doll (PCI 1.3), Footwear Merchant Wholesalers (PCI 1.3)

<details><summary><b>Member metros</b> (21, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| New York-Newark-Jersey City | NY-NJ | 8,554,409 | $90k | 3.82 | 54.2 |
| Los Angeles-Long Beach-Anaheim | CA | 5,566,652 | $75k | 4.16 | 66.2 |
| Boston-Cambridge-Newton | MA-NH | 2,667,556 | $94k | 4.16 | 49.5 |
| Miami-Fort Lauderdale-West Palm Beach | FL | 2,424,379 | $65k | 2.84 | 51.2 |
| San Francisco-Oakland-Fremont | CA | 2,386,872 | $128k | 4.17 | 41.5 |
| Phoenix-Mesa-Chandler | AZ | 2,066,523 | $65k | 2.50 | 47.7 |
| Seattle-Tacoma-Bellevue | WA | 1,877,354 | $96k | 3.36 | 39.8 |
| Denver-Aurora-Centennial | CO | 1,406,517 | $76k | 2.35 | 41.9 |
| San Diego-Chula Vista-Carlsbad | CA | 1,386,384 | $76k | 2.94 | 43.7 |
| Tampa-St. Petersburg-Clearwater | FL | 1,281,491 | $62k | 2.50 | 42.7 |
| Orlando-Kissimmee-Sanford | FL | 1,220,157 | $56k | 2.16 | 40.5 |
| Baltimore-Columbia-Towson | MD | 1,205,307 | $70k | 2.48 | 39.2 |
| San Jose-Sunnyvale-Santa Clara | CA | 1,173,388 | $181k | 4.93 | 25.8 |
| Sacramento-Roseville-Folsom | CA | 813,516 | $69k | 1.68 | 37.5 |
| Salt Lake City-Murray | UT | 697,673 | $70k | 2.54 | 40.3 |
| Bridgeport-Stamford-Danbury | CT | 386,442 | $98k | 2.63 | 37.1 |
| Provo-Orem-Lehi | UT | 265,961 | $55k | 1.79 | 31.3 |
| Fayetteville-Springdale-Rogers | AR | 230,701 | $68k | 1.27 | 22.7 |
| Reno | NV | 224,167 | $62k | 1.36 | 31.1 |
| Huntsville | AL | 202,680 | $66k | 1.22 | 21.3 |
| Ogden | UT | 186,099 | $50k | 1.29 | 30.9 |

</details>

---

## 9. Southern New England Hardware & Instruments

*Renamed from “Southern New England mid-size (mfg + eds/meds)”.* Five compact New England metros specialised in wire, metal and precision devices.

**5 metros · 1,024,639 jobs · $64k avg wage · mean ECI 1.63 · mean niche 29.7 · basket PCI -0.58**

States: MA (2), CT (2), NH (1)

**What binds these cities.** Worcester, New Haven, Manchester, Springfield and Waterbury share an unusually old-industrial niche: communication and energy wire, copper rolling, pressed/blown glass, rolling-mill machinery, surgical and medical instruments and electronic connectors — with savings institutions a shared financial relic. Wire/cable and instruments run at 4-8x baseline, and surgical instruments appear in all five.

**Reading.** Small (5 metros, 1.0M jobs) but distinctive — a miniature eastern analogue of the Great Lakes metalworking belt with a precision-instruments and connectors twist, the legacy of New England's brass-and-hardware valley.

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Other Communication and Energy Wire Manufacturing | 80% | 8.1× | 1.3 | 27% | 1,329 |
| Copper Rolling | 40% | 5.5× | 0.4 | 18% | 511 |
| Other Pressed and Blown Glass and Glassware Manufacturing | 40% | 5.0× | 0.4 | 17% | 139 |
| Rolling Mill and Other Metalworking Machinery Manufacturing | 60% | 4.8× | 1.0 | 16% | 297 |
| Surgical and Medical Instrument Manufacturing | 100% | 4.7× | 0.4 | 16% | 2,526 |
| Radio and Television Broadcasting and Wireless Communications Equipment Manufacturing | 60% | 4.5× | 0.6 | 15% | 676 |
| Electronic Connector Manufacturing | 40% | 4.3× | 1.4 | 14% | 377 |
| Savings Institutions | 100% | 4.1× | -1.1 | 14% | 3,763 |
| Optical Instrument and Lens Manufacturing | 60% | 3.9× | 0.8 | 13% | 957 |
| Business Associations | 80% | 3.9× | -1.3 | 13% | 918 |
| Special Die and Tool | 100% | 3.9× | -0.5 | 13% | 481 |
| Analytical Laboratory Instrument Manufacturing | 60% | 3.8× | 0.6 | 12% | 4,746 |
| Bolt | 60% | 3.8× | 0.6 | 12% | 708 |
| Electromedical and Electrotherapeutic Apparatus Manufacturing | 60% | 3.8× | 1.3 | 12% | 2,049 |
| Limousine Service | 100% | 3.7× | 0.1 | 12% | 589 |

**Employment by sector** (top): Health Care & Social Assistance 22% · Retail Trade 14% · Accommodation & Food Services 9% · Manufacturing 8% · Educational Services 7% · Professional, Scientific & Technical 6%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Electronic Connector Manufacturing (PCI 1.4), Other Communication and Energy Wire Manufacturing (PCI 1.3), Electromedical and Electrotherapeutic Apparatus Manufacturing (PCI 1.3), Stationery Product Manufacturing (PCI 1.2), All Other Converted Paper Product Manufacturing (PCI 1.0), Rolling Mill and Other Metalworking Machinery Manufacturing (PCI 1.0)

<details><summary><b>Member metros</b> (5, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Worcester | MA | 307,383 | $63k | 1.92 | 34.8 |
| New Haven | CT | 249,241 | $64k | 1.79 | 29.0 |
| Manchester-Nashua | NH | 176,867 | $72k | 1.56 | 29.6 |
| Springfield | MA | 156,740 | $56k | 1.13 | 25.9 |
| Waterbury-Shelton | CT | 134,408 | $66k | 1.73 | 29.3 |

</details>

---

## 3. Carolina Piedmont Textile & Fiber Belt

*Renamed from “SE Piedmont textiles / furniture / carpet”.* The most extreme single-industry concentration in the network.

**7 metros · 1,797,391 jobs · $58k avg wage · mean ECI 1.60 · mean niche 30.3 · basket PCI -0.56**

States: NC (3), SC (2), VA (1), GA (1)

**What binds these cities.** Greenville, Greensboro, Winston-Salem, Spartanburg, Hickory, Dalton and Richmond carry the highest lifts found anywhere: hosiery (16x), fiber/yarn/thread (14x), and broadwoven, knit and nonwoven fabric mills, textile finishing and piece-goods (Dalton alone is roughly three-quarters of world carpet). 70-86% of members specialize in the core fabric trades.

**Reading.** 7 metros, 1.8M jobs, ECI 1.60. A textbook Marshallian district — a tightly localized textile and fabric value chain consolidated in the Piedmont. The fabric lines carry low PCI, but the concentration is so strong the cluster forms effortlessly.

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Hosiery and Sock Mills | 43% | 16.2× | -0.0 | 75% | 1,632 |
| Fiber | 86% | 14.4× | -0.4 | 67% | 4,637 |
| Broadwoven Fabric Mills | 71% | 12.0× | 0.1 | 56% | 2,833 |
| Nonwoven Fabric Mills | 86% | 11.8× | 0.4 | 55% | 3,228 |
| Crushed and Broken Granite Mining and Quarrying | 86% | 9.2× | 0.4 | 43% | 752 |
| Knit Fabric Mills | 43% | 9.2× | 0.8 | 43% | 1,251 |
| Textile and Fabric Finishing Mills | 71% | 8.3× | 0.5 | 38% | 2,591 |
| Piece Goods | 86% | 5.4× | 0.3 | 25% | 1,728 |
| Credit Card Issuing | 43% | 5.4× | 1.0 | 25% | 16,189 |
| Upholstered Household Furniture Manufacturing | 43% | 5.4× | 0.2 | 25% | 15,433 |
| Other Paperboard Container Manufacturing | 43% | 4.3× | 0.9 | 20% | 693 |
| Sawmills | 71% | 4.0× | -1.3 | 18% | 688 |
| Manufactured (Mobile) Home Dealers | 86% | 3.8× | -0.9 | 18% | 224 |
| Logging | 57% | 3.8× | -1.6 | 17% | 556 |
| Consumer Lending | 71% | 3.7× | -1.6 | 17% | 1,485 |

**Employment by sector** (top): Health Care & Social Assistance 14% · Retail Trade 13% · Manufacturing 11% · Accommodation & Food Services 11% · Administrative & Waste Services 7% · Professional, Scientific & Technical 6%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Plastics Packaging Film and Sheet (including Laminated) Manufacturing (PCI 1.1), All Other Converted Paper Product Manufacturing (PCI 1.0), Adhesive Manufacturing (PCI 1.0), Credit Card Issuing (PCI 1.0), Gasket (PCI 0.9), Unlaminated Plastics Film and Sheet (except Packaging) Manufacturing (PCI 0.9)

<details><summary><b>Member metros</b> (7, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Richmond | VA | 565,083 | $68k | 1.93 | 34.8 |
| Greenville-Anderson-Greer | SC | 363,349 | $53k | 1.86 | 35.9 |
| Greensboro-High Point | NC | 311,260 | $54k | 1.93 | 35.8 |
| Winston-Salem | NC | 243,447 | $56k | 1.69 | 30.9 |
| Spartanburg | SC | 133,451 | $52k | 1.48 | 28.6 |
| Hickory-Lenoir-Morganton | NC | 127,344 | $49k | 1.50 | 28.5 |
| Dalton | GA | 53,457 | $51k | 0.81 | 17.7 |

</details>

---

## 2. Great Lakes Precision Metalworking Belt

*Renamed from “Rust Belt durable-goods manufacturing”.* Mid-size legacy industrial metros built on the metalworking trades.

**23 metros · 5,828,382 jobs · $59k avg wage · mean ECI 1.53 · mean niche 30.3 · basket PCI -0.59**

States: OH (5), NY (4), PA (3), IN (2), RI-MA (1), CT (1), AL (1), OK (1)

**What binds these cities.** Akron, Buffalo, Rochester, Dayton, Toledo, Fort Wayne, Rockford, Erie and fifteen others form the most internally coherent specialization in the whole network: electroplating and metal coating, heat treating, machine-tool and cutting-tool manufacturing, industrial molds, metal crowns/closures and overhead cranes. 60-83% of members specialize in these lines at ~2.5-3x baseline — a genuine shared 'machine-shop' production system spanning the lower Great Lakes and upstate New York.

**Reading.** 23 metros, 5.8M jobs, mid wages ($59k), ECI 1.53. The classic durable-goods supply base: lower complexity than the giants but the tightest, most consistent niche in the network — which is why it survives re-clustering robustly (matching the validation finding that 'Midwest manufacturing' is one of the stable clusters).

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Metal Crown | 65% | 2.9× | 0.1 | 44% | 5,823 |
| Metal Heat Treating | 61% | 2.9× | 0.5 | 44% | 1,922 |
| Electroplating | 83% | 2.7× | 0.0 | 41% | 5,752 |
| Machine Tool Manufacturing | 61% | 2.7× | 0.0 | 41% | 3,691 |
| Industrial Mold Manufacturing | 65% | 2.7× | 0.0 | 40% | 3,981 |
| Cutting Tool and Machine Tool Accessory Manufacturing | 65% | 2.5× | 0.2 | 38% | 3,042 |
| Overhead Traveling Crane | 30% | 2.4× | 0.9 | 37% | 2,492 |
| Rolling Mill and Other Metalworking Machinery Manufacturing | 30% | 2.4× | 1.0 | 37% | 1,676 |
| Special Die and Tool | 61% | 2.4× | -0.5 | 36% | 3,822 |
| Rubber Product Manufacturing for Mechanical Use | 30% | 2.3× | 0.9 | 35% | 2,177 |
| Saw Blade and Handtool Manufacturing | 52% | 2.3× | 0.4 | 34% | 3,170 |
| Corrugated and Solid Fiber Box Manufacturing | 74% | 2.2× | 0.0 | 33% | 6,767 |
| Bolt | 35% | 2.2× | 0.6 | 33% | 2,785 |
| Motor Vehicle Metal Stamping | 35% | 2.2× | -0.1 | 33% | 8,669 |
| Crushed and Broken Limestone Mining and Quarrying | 52% | 2.1× | -0.8 | 32% | 1,361 |

**Employment by sector** (top): Health Care & Social Assistance 19% · Retail Trade 13% · Manufacturing 11% · Accommodation & Food Services 10% · Professional, Scientific & Technical 6% · Administrative & Waste Services 6%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Rolling Mill and Other Metalworking Machinery Manufacturing (PCI 1.0), Gasket (PCI 0.9), Overhead Traveling Crane (PCI 0.9), Rubber Product Manufacturing for Mechanical Use (PCI 0.9), Other Measuring and Controlling Device Manufacturing (PCI 0.7), Instruments and Related Products Manufacturing for Measuring (PCI 0.7)

<details><summary><b>Member metros</b> (23, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Providence-Warwick | RI-MA | 636,876 | $61k | 2.32 | 44.8 |
| Hartford-West Hartford-East Hartford | CT | 529,690 | $71k | 2.58 | 35.4 |
| Birmingham | AL | 469,011 | $63k | 1.86 | 35.2 |
| Buffalo-Cheektowaga | NY | 455,918 | $56k | 2.18 | 39.6 |
| Rochester | NY | 420,804 | $56k | 2.16 | 38.2 |
| Tulsa | OK | 390,107 | $58k | 1.79 | 36.0 |
| Albany-Schenectady-Troy | NY | 348,476 | $64k | 1.49 | 31.6 |
| Dayton-Kettering-Beavercreek | OH | 315,310 | $57k | 1.92 | 32.4 |
| Akron | OH | 284,528 | $57k | 1.94 | 33.0 |
| Syracuse | NY | 249,655 | $57k | 1.42 | 30.1 |
| Toledo | OH | 245,316 | $54k | 1.64 | 32.1 |
| Fort Wayne | IN | 193,589 | $54k | 1.54 | 31.2 |
| York-Hanover | PA | 155,688 | $54k | 1.24 | 26.6 |
| Davenport-Moline-Rock Island | IA-IL | 152,564 | $58k | 0.84 | 23.7 |
| Reading | PA | 147,952 | $57k | 1.19 | 26.5 |
| Canton-Massillon | OH | 132,938 | $49k | 1.10 | 28.4 |
| Youngstown-Warren | OH | 132,047 | $48k | 1.15 | 29.1 |
| Elkhart-Goshen | IN | 124,000 | $57k | 2.38 | 30.1 |
| Rockford | IL | 117,453 | $54k | 1.53 | 28.7 |
| Erie | PA | 104,001 | $50k | 0.93 | 22.6 |
| Kalamazoo-Portage | MI | 103,607 | $59k | 1.01 | 22.6 |
| Waterloo-Cedar Falls | IA | 62,454 | $54k | 0.34 | 18.9 |
| Racine-Mount Pleasant | WI | 56,398 | $53k | 0.60 | 20.2 |

</details>

---

## 5. Gulf Coast Oil, Gas & Petrochemicals

*Renamed from “Gulf/SW oil, gas & petrochemicals”.* The U.S. hydrocarbon value chain, end to end.

**10 metros · 4,672,153 jobs · $70k avg wage · mean ECI 1.36 · mean niche 27.9 · basket PCI -0.57**

States: TX (4), LA (4), TN-MS-AR (1), CO (1)

**What binds these cities.** Houston, New Orleans, Baton Rouge, Beaumont, Lake Charles, Midland and Odessa — plus Greeley, CO — span the whole chain: natural-gas extraction, drilling, oilfield machinery and support services, crude pipelines, inland-water freight, petroleum refining and petrochemical manufacturing, with 40-90% of members specialized at 6-15x baseline.

**Reading.** 10 metros, 4.7M jobs, $70k wages. Note the low PCI on the upstream lines (drilling, support activities and pipelines score -1.0 to -1.5) versus higher PCI on refining and petrochemicals — a reminder that resource extraction scores low on complexity even when it pays well. One of the validation-stable clusters (Gulf petrochem + Permian oil).

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Petrochemical Manufacturing | 40% | 15.1× | 0.4 | 100% | 8,278 |
| Pipeline Transportation of Crude Oil | 90% | 10.5× | -1.0 | 69% | 3,578 |
| Inland Water Freight Transportation | 60% | 10.1× | 0.2 | 67% | 7,719 |
| Oil and Gas Field Machinery and Equipment Manufacturing | 60% | 10.1× | -0.9 | 67% | 13,427 |
| Drilling Oil and Gas Wells | 50% | 8.4× | -1.4 | 56% | 12,738 |
| Natural Gas Extraction | 70% | 7.0× | -1.2 | 47% | 6,278 |
| Support Activities for Oil and Gas Operations | 80% | 6.7× | -1.5 | 44% | 58,295 |
| Petroleum Refineries | 50% | 6.3× | 0.8 | 42% | 16,904 |
| Crude Petroleum Extraction | 70% | 6.2× | -1.4 | 41% | 18,523 |
| Marine Cargo Handling | 60% | 6.0× | 0.4 | 40% | 7,311 |
| Deep Sea Freight Transportation | 40% | 6.0× | 1.0 | 40% | 1,077 |
| Oil and Gas Pipeline and Related Structures Construction | 90% | 5.9× | -1.2 | 39% | 66,101 |
| Pipeline Transportation of Natural Gas | 90% | 5.7× | -1.1 | 38% | 5,831 |
| Navigational Services to Shipping | 70% | 5.0× | -0.4 | 33% | 3,586 |
| Other Support Activities for Water Transportation | 60% | 5.0× | 0.0 | 33% | 2,367 |

**Employment by sector** (top): Health Care & Social Assistance 14% · Accommodation & Food Services 12% · Retail Trade 12% · Construction 8% · Professional, Scientific & Technical 7% · Manufacturing 7%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Sports Teams and Clubs (PCI 1.3), Petroleum Lubricating Oil and Grease Manufacturing (PCI 1.2), All Other Miscellaneous Nonmetallic Mineral Product Manufacturing (PCI 1.0), Deep Sea Freight Transportation (PCI 1.0), Gasket (PCI 0.9), Industrial Valve Manufacturing (PCI 0.9)

<details><summary><b>Member metros</b> (10, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Houston-Pasadena-The Woodlands | TX | 2,859,297 | $75k | 3.77 | 52.0 |
| Memphis | TN-MS-AR | 543,439 | $60k | 2.21 | 33.2 |
| New Orleans-Metairie | LA | 400,740 | $61k | 1.83 | 36.4 |
| Baton Rouge | LA | 341,793 | $61k | 1.60 | 31.0 |
| Beaumont-Port Arthur | TX | 126,469 | $60k | 1.08 | 25.4 |
| Midland | TX | 98,316 | $89k | 0.65 | 17.9 |
| Greeley | CO | 94,725 | $65k | 0.65 | 22.8 |
| Lake Charles | LA | 79,080 | $56k | 0.57 | 21.8 |
| Houma-Bayou Cane-Thibodaux | LA | 66,733 | $63k | 0.76 | 21.0 |
| Odessa | TX | 61,561 | $73k | 0.53 | 17.9 |

</details>

---

## 4. Central Pennsylvania Logistics & Capital Services

*Renamed from “Pennsylvania logistics / warehousing”.* A two-metro Pennsylvania pairing — the state capital plus an interstate logistics hub.

**2 metros · 504,577 jobs · $56k avg wage · mean ECI 1.36 · mean niche 27.1 · basket PCI -0.66**

States: PA (2)

**What binds these cities.** Harrisburg and Scranton-Wilkes-Barre share (in both, 100%) an idiosyncratic mix: insurance carriers, ice-cream and confectionery manufacturing, charter-bus transport, specialty hospitals, libraries/archives and political organizations — the fingerprint of a state-capital service economy bolted onto the I-81/I-78 warehousing corridor (transportation is 11% of jobs).

**Reading.** The smallest cluster (2 metros, 0.5M jobs) and the least robust: it exists only because two adjacent PA metros share this capital-plus-distribution profile. With n=2 it is the most fragile grouping (consistent with the validation note that only ~42/151 metros are robustly placed).

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Other Direct Insurance (except Life | 100% | 10.1× | 0.9 | 13% | 377 |
| Ice Cream and Frozen Dessert Manufacturing | 100% | 7.5× | 0.7 | 10% | 524 |
| Confectionery Manufacturing from Purchased Chocolate | 100% | 5.8× | 0.0 | 8% | 3,448 |
| Political Organizations | 100% | 5.8× | -0.2 | 8% | 60 |
| Confectionery Merchant Wholesalers | 100% | 5.2× | -0.2 | 7% | 1,987 |
| Libraries and Archives | 100% | 5.2× | -0.9 | 7% | 613 |
| Charter Bus Industry | 100% | 4.7× | 0.5 | 6% | 122 |
| Specialty (except Psychiatric and Substance Abuse) Hospitals | 100% | 4.7× | 0.1 | 6% | 1,598 |
| Meat Processed from Carcasses | 100% | 4.4× | -0.2 | 6% | 2,550 |
| All Other Miscellaneous Waste Management Services | 100% | 4.1× | -0.1 | 5% | 110 |
| Other Support Activities for Road Transportation | 100% | 4.1× | -0.3 | 5% | 666 |
| Paint | 100% | 4.0× | -0.1 | 5% | 112 |
| Asphalt Paving Mixture and Block Manufacturing | 100% | 3.9× | -0.2 | 5% | 105 |
| Couriers and Express Delivery Services | 100% | 3.6× | -1.2 | 5% | 8,353 |
| Water Supply and Irrigation Systems | 100% | 3.6× | -1.2 | 5% | 581 |

**Employment by sector** (top): Health Care & Social Assistance 22% · Retail Trade 14% · Transportation & Warehousing 11% · Accommodation & Food Services 9% · Manufacturing 6% · Administrative & Waste Services 6%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Other Direct Insurance (except Life (PCI 0.9), Ice Cream and Frozen Dessert Manufacturing (PCI 0.7), Charter Bus Industry (PCI 0.5), General Line Grocery Merchant Wholesalers (PCI 0.3), Specialty (except Psychiatric and Substance Abuse) Hospitals (PCI 0.1), Direct Health and Medical Insurance Carriers (PCI 0.1)

<details><summary><b>Member metros</b> (2, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Harrisburg-Carlisle | PA | 283,572 | $61k | 1.23 | 24.8 |
| Scranton--Wilkes-Barre | PA | 221,005 | $50k | 1.49 | 29.5 |

</details>

---

## 8. High-Amenity, Knowledge & Tourism Economies

*Renamed from “University / govt-research / amenity-tourism / specialty”.* The most heterogeneous cluster — capital, college, coast and resort towns bound by amenity and knowledge services.

**43 metros · 9,172,113 jobs · $72k avg wage · mean ECI 0.99 · mean niche 25.8 · basket PCI -0.79**

States: CA (8), HI (3), CO (3), MT (3), NC (2), ID (2), MI (2), WA (2)

**What binds these cities.** 43 metros from Washington DC, Austin, Raleigh-Durham and Boulder to Honolulu, Naples, Santa Barbara, Bend and Barnstable. What they share is not an industry but an amenity/knowledge service profile: hotels and traveler accommodation, wineries, art dealers, environmental consulting, bed-and-breakfasts, gift shops and full-service restaurants (50-77% of members at ~2.2-2.7x baseline). Professional and technical services are the second-largest sector by employment.

**Reading.** Largest by count (43 metros, 9.2M jobs), $72k wages, but the lowest-complexity high-amenity tail (ECI 0.99, basket PCI -0.79) because the distinctive activities are consumer-facing services. It is really two overlapping types — knowledge/government hubs and tourism/lifestyle metros — merged because both run light on tradable manufacturing and heavy on high-end services. A prime candidate to split at higher clustering resolution.

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Hotels (except Casino Hotels) and Motels | 67% | 2.7× | -1.6 | 76% | 158,411 |
| Wineries | 35% | 2.5× | -1.2 | 71% | 25,426 |
| Art Dealers | 33% | 2.5× | -1.0 | 70% | 1,451 |
| Environment | 72% | 2.4× | -1.2 | 67% | 17,151 |
| All Other Traveler Accommodation | 51% | 2.3× | -1.0 | 67% | 1,104 |
| Bed-and-Breakfast Inns | 54% | 2.2× | -1.0 | 64% | 1,469 |
| Gift | 63% | 2.2× | -1.3 | 63% | 11,715 |
| Full-Service Restaurants | 77% | 2.2× | -1.6 | 62% | 425,420 |
| Lessors of Other Real Estate Property | 56% | 2.2× | -1.2 | 62% | 2,239 |
| Family Clothing Stores | 56% | 2.1× | -1.3 | 60% | 57,803 |
| Recreational Goods Rental | 37% | 2.1× | -0.7 | 59% | 1,464 |
| Women's Clothing Stores | 51% | 2.0× | -1.6 | 58% | 16,543 |
| Direct Title Insurance Carriers | 56% | 2.0× | -0.4 | 57% | 3,293 |
| Other Social Advocacy Organizations | 42% | 2.0× | -0.9 | 56% | 18,987 |
| Offices of Real Estate Agents and Brokers | 49% | 1.9× | -1.3 | 54% | 36,222 |

**Employment by sector** (top): Health Care & Social Assistance 15% · Professional, Scientific & Technical 13% · Retail Trade 12% · Accommodation & Food Services 12% · Construction 7% · Administrative & Waste Services 6%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Coffee and Tea Manufacturing (PCI 0.1), Limousine Service (PCI 0.1), Textile Bag and Canvas Mills (PCI -0.1), Automobile Driving Schools (PCI -0.1), Reupholstery and Furniture Repair (PCI -0.1), Commercial Photography (PCI -0.2)

<details><summary><b>Member metros</b> (43, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Washington-Arlington-Alexandria | DC-VA-MD-WV | 2,856,029 | $85k | 2.72 | 35.7 |
| Austin-Round Rock-San Marcos | TX | 1,033,811 | $78k | 2.30 | 38.6 |
| Raleigh-Cary | NC | 608,246 | $69k | 1.88 | 32.6 |
| Urban Honolulu | HI | 326,934 | $61k | 1.51 | 33.1 |
| Boise City | ID | 312,419 | $61k | 1.51 | 34.2 |
| Durham-Chapel Hill | NC | 292,614 | $84k | 2.49 | 23.3 |
| Oxnard-Thousand Oaks-Ventura | CA | 266,036 | $66k | 1.91 | 38.9 |
| Portland-South Portland | ME | 240,197 | $63k | 1.16 | 30.5 |
| Trenton-Princeton | NJ | 200,777 | $86k | 2.14 | 23.8 |
| Santa Rosa-Petaluma | CA | 167,256 | $68k | 1.35 | 32.7 |
| Anchorage | AK | 162,266 | $73k | 0.95 | 28.0 |
| Santa Maria-Santa Barbara | CA | 151,686 | $68k | 1.29 | 30.3 |
| Boulder | CO | 150,734 | $83k | 2.09 | 31.4 |
| Naples-Marco Island | FL | 149,199 | $58k | 0.82 | 25.7 |
| Ann Arbor | MI | 147,675 | $70k | 1.77 | 26.1 |
| Modesto | CA | 142,480 | $58k | 0.82 | 26.5 |
| Fort Collins-Loveland | CO | 132,214 | $62k | 0.89 | 25.7 |
| Salinas | CA | 112,673 | $60k | 0.59 | 24.3 |
| Vallejo | CA | 112,211 | $62k | 0.79 | 23.7 |
| Kennewick-Richland | WA | 91,470 | $61k | 0.33 | 20.5 |
| Burlington-South Burlington | VT | 88,172 | $60k | 0.79 | 27.2 |
| Bend | OR | 83,158 | $57k | 0.57 | 24.6 |
| Lebanon-Claremont | NH-VT | 83,019 | $61k | 0.89 | 23.9 |
| Billings | MT | 75,435 | $56k | 0.40 | 21.6 |
| Charleston | WV | 74,006 | $56k | 0.59 | 21.7 |
| Santa Cruz-Watsonville | CA | 73,634 | $61k | 0.78 | 26.9 |
| Charlottesville | VA | 73,600 | $60k | 0.86 | 25.8 |
| Medford | OR | 73,251 | $54k | 0.44 | 22.5 |
| Topeka | KS | 73,000 | $54k | 0.28 | 18.2 |
| Barnstable Town | MA | 71,241 | $60k | 0.55 | 24.6 |
| Norwich-New London-Willimantic | CT | 70,722 | $55k | 0.30 | 20.1 |
| Bellingham | WA | 69,490 | $56k | 0.53 | 25.5 |
| St. George | UT | 62,999 | $44k | 0.66 | 24.1 |
| Idaho Falls | ID | 62,985 | $60k | 0.51 | 17.9 |
| Kahului-Wailuku | HI | 59,205 | $53k | 0.79 | 22.9 |
| Napa | CA | 56,602 | $65k | 0.68 | 21.1 |
| Concord | NH | 53,881 | $60k | 0.60 | 23.4 |
| Traverse City | MI | 53,220 | $56k | 0.57 | 23.5 |
| Bozeman | MT | 52,362 | $60k | 0.65 | 24.5 |
| Grand Junction | CO | 51,909 | $55k | 0.19 | 19.0 |
| Hilo-Kailua | HI | 51,564 | $51k | 0.60 | 22.4 |
| Missoula | MT | 50,879 | $51k | 0.48 | 23.4 |
| Logan | UT-ID | 50,852 | $50k | 0.46 | 18.8 |

</details>

---

## 0. Upper-Midwest Paper, Dairy & Food Machinery

*Renamed from “Upper-Midwest paper / insurance / food processing”.* Wisconsin's Fox Valley paper-and-food cluster plus kindred small metros.

**6 metros · 673,797 jobs · $57k avg wage · mean ECI 0.96 · mean niche 24.0 · basket PCI -0.77**

States: WI (4), PA (1), GA (1)

**What binds these cities.** Green Bay, Appleton, Oshkosh and Wausau — with Lancaster, PA and Gainesville, GA — specialize in paper mills, sanitary-paper and converted-paper products, sawmills, cheese manufacturing, food-product machinery and lawn-and-garden equipment, with paper and food-processing lifts of 8-10x.

**Reading.** 6 metros, 0.7M jobs, ECI 0.96. A resource-processing cluster (forests to paper, dairy to cheese) plus the machinery that serves it; Gainesville (poultry) and Lancaster (food/ag) ride the same food-processing axis.

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Lawn and Garden Tractor and Home Lawn and Garden Equipment Manufacturing | 33% | 10.1× | 0.9 | 40% | 635 |
| Sanitary Paper Product Manufacturing | 33% | 10.1× | 0.0 | 40% | 2,881 |
| Paper (except Newsprint) Mills | 33% | 8.4× | 0.5 | 33% | 3,544 |
| Sawmill | 67% | 5.9× | 0.4 | 24% | 1,689 |
| Cheese Manufacturing | 67% | 5.3× | -0.7 | 21% | 7,050 |
| Copper Rolling | 33% | 4.6× | 0.4 | 18% | 513 |
| Poultry and Poultry Product Merchant Wholesalers | 33% | 3.9× | 0.6 | 15% | 317 |
| Food Product Machinery Manufacturing | 67% | 3.7× | 0.6 | 15% | 1,269 |
| Other Animal Food Manufacturing | 67% | 3.5× | -1.1 | 14% | 1,873 |
| Paper Bag and Coated and Treated Paper Manufacturing | 83% | 3.2× | 0.5 | 13% | 3,218 |
| Plate Work Manufacturing | 100% | 2.6× | -0.3 | 10% | 1,464 |
| Other Commercial and Service Industry Machinery Manufacturing | 67% | 2.6× | 0.3 | 10% | 1,063 |
| Other Millwork (including Flooring) | 67% | 2.6× | -0.3 | 10% | 773 |
| Refrigerated Warehousing and Storage | 67% | 2.6× | -0.3 | 10% | 708 |
| Wood Kitchen Cabinet and Countertop Manufacturing | 100% | 2.6× | -1.1 | 10% | 3,054 |

**Employment by sector** (top): Health Care & Social Assistance 16% · Manufacturing 15% · Retail Trade 13% · Accommodation & Food Services 9% · Construction 8% · Transportation & Warehousing 6%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Printing and Writing Paper Merchant Wholesalers (PCI 1.1), Plastics Packaging Film and Sheet (including Laminated) Manufacturing (PCI 1.1), All Other Converted Paper Product Manufacturing (PCI 1.0), Polystyrene Foam Product Manufacturing (PCI 0.9), Lawn and Garden Tractor and Home Lawn and Garden Equipment Manufacturing (PCI 0.9), Support Activities for Printing (PCI 0.7)

<details><summary><b>Member metros</b> (6, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Lancaster | PA | 235,229 | $55k | 1.59 | 36.2 |
| Green Bay | WI | 144,355 | $58k | 1.30 | 27.1 |
| Appleton | WI | 102,097 | $58k | 0.91 | 23.6 |
| Oshkosh-Neenah | WI | 72,228 | $60k | 0.90 | 19.0 |
| Gainesville | GA | 67,641 | $60k | 0.59 | 19.5 |
| Wausau | WI | 52,247 | $57k | 0.45 | 18.6 |

</details>

---

## 1. Plains Agribusiness, Grain Trade & Insurance

*Renamed from “Plains ag / insurance / university-healthcare”.* The grain-belt agribusiness-and-finance complex.

**12 metros · 1,368,086 jobs · $61k avg wage · mean ECI 0.62 · mean niche 20.1 · basket PCI -0.89**

States: IL (3), MN (2), WI (2), IA (1), SD-MN (1), ND-MN (1), WI-MN (1), IA-NE-SD (1)

**What binds these cities.** Des Moines, Sioux Falls, Peoria, Fargo, Sioux City and others specialize in farm machinery, grain and field-bean wholesaling, commodity-contract brokerage, farm-product warehousing, animal slaughtering, soil-prep services and nondepository credit — primary agriculture plus the trading and finance layer that monetizes it. Insurance/finance is a leading employment sector (State Farm in Bloomington, Principal in Des Moines).

**Reading.** 12 metros, 1.4M jobs, lowest complexity in the network (ECI 0.62, basket PCI -0.89). Rochester, MN (Mayo) and Bloomington, IL pull health and insurance into an otherwise agribusiness core; the low PCI reflects that primary agriculture and its logistics score low on complexity even where incomes are stable.

**Defining specializations** (highest lift; the industries that thread through the cluster):

| Industry | % metros | Lift | PCI | Exclusivity | Cluster jobs |
|----------|---------:|-----:|----:|------------:|-------------:|
| Farm Machinery and Equipment Manufacturing | 50% | 5.0× | -1.2 | 40% | 5,472 |
| Commodity Contracts Brokerage | 42% | 4.2× | 0.3 | 33% | 280 |
| Grain and Field Bean Merchant Wholesalers | 75% | 3.7× | -1.6 | 29% | 2,123 |
| Farm Product Warehousing and Storage | 33% | 3.6× | -0.7 | 29% | 213 |
| All Other Nondepository Credit Intermediation | 67% | 3.5× | -1.5 | 28% | 1,539 |
| Animal (except Poultry) Slaughtering | 33% | 3.4× | -1.0 | 27% | 13,174 |
| Offices of Bank Holding Companies | 33% | 3.0× | 0.1 | 24% | 284 |
| Soil Preparation | 58% | 2.8× | -1.3 | 22% | 212 |
| Cheese Manufacturing | 33% | 2.6× | -0.7 | 21% | 1,662 |
| Farm and Garden Machinery and Equipment Merchant Wholesalers | 100% | 2.5× | -1.5 | 20% | 3,383 |
| Farm Supplies Merchant Wholesalers | 100% | 2.5× | -1.5 | 20% | 4,988 |
| Other Gambling Industries | 50% | 2.4× | -1.0 | 19% | 1,220 |
| Other Animal Food Manufacturing | 42% | 2.2× | -1.1 | 17% | 532 |
| Automobile and Other Motor Vehicle Merchant Wholesalers | 92% | 1.9× | -0.8 | 15% | 3,833 |
| Telecommunications Resellers | 33% | 1.9× | -0.6 | 15% | 440 |

**Employment by sector** (top): Health Care & Social Assistance 19% · Retail Trade 13% · Accommodation & Food Services 10% · Finance & Insurance 9% · Professional, Scientific & Technical 7% · Manufacturing 7%

**Most knowledge-intensive niches** (highest-PCI of the defining specializations): Commodity Contracts Brokerage (PCI 0.3), Other Commercial Equipment Merchant Wholesalers (PCI 0.1), Offices of Bank Holding Companies (PCI 0.1), Construction Machinery Manufacturing (PCI 0.1), Commercial Bakeries (PCI 0.0), Industrial Launderers (PCI 0.0)

<details><summary><b>Member metros</b> (12, by employment)</summary>

| Metro | State | Jobs | Wage | ECI | Niche |
|-------|-------|-----:|-----:|----:|------:|
| Des Moines-West Des Moines | IA | 355,339 | $66k | 1.51 | 27.4 |
| Sioux Falls | SD-MN | 153,350 | $58k | 0.79 | 24.0 |
| Peoria | IL | 146,241 | $63k | 1.01 | 22.3 |
| Fargo | ND-MN | 121,185 | $60k | 0.69 | 22.4 |
| Rochester | MN | 115,203 | $74k | 0.70 | 15.1 |
| St. Cloud | MN | 92,102 | $57k | 0.59 | 20.7 |
| Champaign-Urbana | IL | 71,067 | $55k | 0.33 | 18.6 |
| La Crosse-Onalaska | WI-MN | 70,382 | $54k | 0.50 | 20.1 |
| Eau Claire | WI | 66,625 | $54k | 0.54 | 21.5 |
| Bloomington | IL | 63,719 | $63k | 0.35 | 14.8 |
| Sioux City | IA-NE-SD | 60,904 | $54k | 0.35 | 18.9 |
| Janesville-Beloit | WI | 51,969 | $57k | 0.15 | 15.1 |

</details>

---

## Cross-cluster synthesis

**A complexity gradient, not a ladder.** Mean ECI runs from 3.06 (cluster 6) down to 0.62 (cluster 1). The top is held by the two service-and-production giants (clusters 6 and 7, together ~68M jobs); the middle by coherent tradable-goods districts (metalworking 2, textiles 3, hydrocarbons 5, New England hardware 9); the bottom by resource-processing and amenity economies (0, 1, 8) where the defining activities — agriculture, paper, tourism — score low on complexity regardless of income.

**Two giants vs. eight specialists.** Clusters 6 and 7 are defined by *breadth* (their distinctive industries are faint tells layered on diversified service bases), while the other eight are defined by *depth* in one tradable value chain. The starkest are textiles (cluster 3, lifts to 16×) and hydrocarbons (cluster 5, lifts to 15×) — true Marshallian districts.

**Geography largely follows industry.** Great Lakes + upstate NY = metalworking (2); Carolinas Piedmont = textiles (3); Gulf Coast = hydrocarbons (5); Fox Valley Wisconsin = paper/dairy (0); Upper-Plains = agribusiness (1); Southern New England = hardware/instruments (9). The exceptions are the two giants (national) and the amenity cluster (8), which is bound by economic *function* (high-end services, light manufacturing) rather than place.

**Methodological caveats.** (1) RCA-of-payroll surfaces rare manufacturing and resource tells but understates ubiquitous high-value services, so finance/tech barely register as 'distinctive' in cluster 7. (2) Resource and consumer-service specializations carry low PCI, dragging basket-PCI negative even for high-wage clusters (5, 8). (3) The smallest clusters (4 with 2 metros, 0/9 with 5-6) are the least robust — consistent with the validation finding that only ~42/151 metros are robustly placed. (4) Cluster 8 visibly bundles two types (knowledge/government vs. tourism/lifestyle) and would split at higher Louvain resolution.

## Naming crosswalk

| # | Old name | New name |
|---|----------|----------|
| 6 | Large diversified metros | **Diversified Industrial & Logistics Powerhouses** |
| 7 | Superstar tech / finance / knowledge | **Coastal Superstar & Tech-Finance Metros** |
| 9 | Southern New England mid-size (mfg + eds/meds) | **Southern New England Hardware & Instruments** |
| 3 | SE Piedmont textiles / furniture / carpet | **Carolina Piedmont Textile & Fiber Belt** |
| 2 | Rust Belt durable-goods manufacturing | **Great Lakes Precision Metalworking Belt** |
| 5 | Gulf/SW oil, gas & petrochemicals | **Gulf Coast Oil, Gas & Petrochemicals** |
| 4 | Pennsylvania logistics / warehousing | **Central Pennsylvania Logistics & Capital Services** |
| 8 | University / govt-research / amenity-tourism / specialty | **High-Amenity, Knowledge & Tourism Economies** |
| 0 | Upper-Midwest paper / insurance / food processing | **Upper-Midwest Paper, Dairy & Food Machinery** |
| 1 | Plains ag / insurance / university-healthcare | **Plains Agribusiness, Grain Trade & Insurance** |

*Short labels for the viewer legend are in `CLUSTER_NAMES` in `index_cities.html`.*
