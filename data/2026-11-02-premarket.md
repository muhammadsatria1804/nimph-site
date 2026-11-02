# Pre-market intel — Monday 2026-11-02 (IDX trading day)

Run: cloud night shift, 06:13 WIB (tools/clock.py: trading_day=true, before_open=true, last completed session 2026-10-30, next session 2026-11-02).
Paper holdings: none (desk/paper/portfolio.json: cash Rp150,000,000, no positions; desk/watchlist.json empty). **intel/alerts.md: no change.**
This run also covers Friday's close and the weekend: there was no 2026-10-30 evening run (see intel/weekly/2026-10-31.md).

## Data access — read first
- `tools/prices.py ^JKSE` and `tools/idx.py disclosures --hours 72` still return `unavailable` (proxy 403 on query1.finance.yahoo.com and www.idx.id, 06:14 WIB). **Thirteenth cloud run in a row.** No tool-checked disclosures, OHLCV, volume ratio, gap, ARA/ARB or flow numbers here: all figures come from news pages.
- Refused or failed fetches: Bisnis (ICBP results page), bbntimes, WTOP. Those stories are **headline-only** unless another outlet is cited.
- Asian markets had not opened at run time. Nickel was not refreshed.

## Read first: today is a heavy day
1. **HSC stocks leave the IHSG calculation from today (11-02).** Also from November: BEI's short-selling list is emptied (5 names dropped incl. ASII, BBCA, BUMI, INDF) and 11 stocks leave the margin list (CNBC Indonesia, "November Baru Mulai, RI Langsung Diguncang 10 Kabar Panas Pekan ini!", 11-02 05:55 WIB). The list of the 11 margin names was not in the article.
2. **Domestic data today (BPS / S&P Global):** October manufacturing PMI (September 52.48), October CPI (consensus 0.24% m/m, **3.25% y/y** vs 3.28% in September), September trade balance (August surplus US$3.55 bn). Same CNBC source.
3. **US sold off hard on Friday:** Nasdaq −2.86%, S&P 500 −1.82% (worst day since June), Intel −29%. Gold −3.3% to about US$3,899. Brent US$117.64 (Dec contract expiry). Details below.
4. **MSCI's November review results are due 11-11, effective 12-01** (investor.id, "BERITA POPULER: Arah Saham BMRI hingga Target Harga Baru GOTO", 11-02 05:00 WIB). Not yet in intel/calendar.json: the evening run should add it.

## Friday 2026-10-30 close (press, not tool-checked)
- **IHSG 5,057.05, −0.80% (−41.01 pts); intraday low 4,979.34.** Week −7.03% (from 5,439.26); October −16.70% (from 6,071.14); YTD −41.52%. Value Rp11.65 tn, volume 37.62 bn shares. Breadth **187 up / 523 down / 81 flat** (Kontan, "IHSG Turun 16,70% Sepanjang Oktober 2026, Ditutup 5.057 Pada Jumat (30/10)", 10-30 19:31 WIB). Five outlets agree on the close (weekly review).
- **Foreign flow 10-30: net SELL Rp140.27 bn all markets; Rp172.43 bn regular** (net buy Rp32.16 bn in cash and negotiated) (Kontan, same). investor.id gives Rp176 bn regular (11-02 05:00 WIB): small gap, same direction. **Week: Rp3.06 tn net sell** (Rp6.67 tn the week before) (CNBC Indonesia, 11-02 05:55 WIB; legawa, "Kilas Ekonomi Sepekan #3", 11-01). YTD: Rp97.92 tn (legawa) vs Rp126 tn (investor.id): different basis, unreconciled.

| Net buy (Rp bn) | | Net sell (Rp bn) | |
|---|---|---|---|
| **GOTO** | 54.5 | **BBRI** | 206.5 |
| BUMI | 40.4 | **TLKM** | 119.5 |
| MDKA | 39.5 | AMMN | 59.3 |

Source: Kontan, 10-30 19:31 WIB (top 3 each side only; the full top 20 was not found).

- **Selling pressure eased sharply** from Rp1.07 tn on 10-29 to ~Rp0.17 tn: the first day in a week below Rp0.5 tn. One day is not a trend.
- Sectors: transport −3.13%, basic materials −2.84%, infrastructure −1.96%, industrials −1.49%, property −1.43%, energy −0.91%; health +0.76%, financials +0.16% (Kontan).
- **LQ45 top gainers:** PGAS +8.64%, PTBA +5.88%, EXCL +5.85%. **Top losers:** BRPT −6.96%, CUAN −6.83%, ISAT −6.83% (Kontan). BRPT at −6.96% is **probably at the 7% ARB** (tick rounding); unverified. No closing ARA/ARB list found: morning desk, run `tools/prices.py scan`.
- BBCA last price **Rp4,980** (investor.id and Suara, both citing Samuel Sekuritas; date of close not stated, likely 10-30): up from Rp4,940 on 10-29.

## Results released since the last intel (Indonesian issuers)

| Ticker | Period | Revenue | Net profit (attrib.) | Read | Source / time |
|---|---|---|---|---|---|
| **AMMN** | 9M 2026 | US$3.238 bn, +494% | **US$880 m vs loss of US$175 m**; Bisnis headline Rp15.56 tn | EBITDA US$1.833 bn (57% margin); copper +129% to 332 m lb, gold +616% to 541,337 oz; smelter at design capacity; net debt −13% YTD to ~US$5 bn (1.9x EBITDA); "on track to meet or beat" 2026 guidance; Rp1 tn buyback announced 10-22 | investortrust, "Laba Bersih Amman (AMMN) Meroket Jadi US$ 880 Juta hingga Kuartal III-2026", 10-30 15:22 WIB; CNBC Indonesia 10-30 13:04 WIB; Bisnis headline 10-30 |
| **INCO** | 9M 2026 | US$896.07 m, +27% | **US$147.12 m, +180.5%** | EBITDA US$297 m (+78.9%). Driven by **nickel ore sales** (Bahodopi 2.38 m wmt, +285%; Pomalaa 1.90 m wmt, +582%), not price. **Q3 alone weaker: profit US$42.75 m, −29.7% q/q**; realized matte price −4.8% q/q to US$14,053/t; cash cost +4% to US$10,404/t; 9M matte output −12.5% | Kontan, "Penjualan Bijih Nikel Dongkrak Laba Vale Indonesia (INCO) Melonjak 180,5%", 10-30 06:27 WIB |
| **TLKM** | 9M 2026 | Rp113.50 tn, +3.55% | **Rp14.44 tn, −3.73%** (total incl. minorities Rp19.46 tn, −1.92%) | Opex +5.94%, faster than revenue; EPS Rp146.31 (−3.57%); operating profit Rp27.99 tn. Not material (<10%). Q3 alone not given | investor.id, "Telkom (TLKM) Raup Laba Rp 14 Triliun hingga Kuartal III-2026", 11-02 05:10 WIB; Liputan6, "Pendapatan Tumbuh 3,54%, Telkom Kantongi Laba Rp 19,46 Triliun", 10-31 18:20 WIB |
| **ICBP** | 9M 2026 | Rp64.4 tn, +14.54% | **−13.26%** (level not read) | headline-only (Bisnis refused). H1 was −33% on FX losses on loans, so 9M is an improvement in the rate of decline | Bisnis, "Penjualan ICBP Tumbuh 14,54% Jadi Rp64,4 Triliun, Laba Bersih Turun 13,26%", 10-31 |
| **BBCA** | Q3 / 9M 2026 | — | Q3 Rp15.7 tn (+9% y/y, +5.6% q/q); 9M Rp45.2 tn (+4.2%) | Samuel Sekuritas: Buy, TP Rp5,800 (2.3x FY26 PBV) | investor.id 11-02 05:00 WIB; Suara, "Target Harga Saham BBCA di Tengah Koreksi Ekstrem", 11-01 22:11 WIB |
| **GOTO** | Q3 2026 | — | **Rp557 bn, +46.8% q/q** per KB Valbury (Buy, TP cut from Rp61; new TP not in text) | **Conflict** with the Rp441 bn in the 10-30 intel (investor.id, tirto, detik, Okezone). Likely total vs attributable, or a different line; unverified | investor.id 11-02 05:00 WIB |
| BMRI | — | — | — | Kiwoom: Buy, TP cut from Rp5,400 (new TP not in text; ~Rp4,800 implied by "29% upside" from Rp3,720) | investor.id 11-02 05:00 WIB |
| DSNG | Q3 2026 | — | Rp1.46 tn | headline-only | Kontan headline "Dharma Satya (DSNG) Bukukan Laba Rp 1,46 Triliun pada Kuartal III-2026" |
| JSMR | Q3 2026 | — | Rp2.66 tn | headline-only | IDN Times headline |
| MPMX | Q3 2026 | — | Rp539 bn | headline-only | Suara headline, 10-30 17:16 WIB |
| KAEF | 9M 2026 | — | net loss −94.5% | headline-only | Kontan headline "Kimia Farma (KAEF) Pangkas Rugi Bersih 94,5% hingga September 2026" |

- **Still not found (search, 06:15 WIB): BBRI, BRIS, INDF, ADRO/AADI, ITMG, MEDC, MDKA, EXCL.** BBRI disclosed a **limited review by a public accountant of its 30 September 2026 accounts**, "tied to corporate action plans and/or shareholder aspirations" (Kontan, "BRI Jalani Limited Review Laporan September Ini, Penjelasan Manajemen", 2026-09-28 20:10 WIB). Its Q3 release may therefore come later than the 10-31 deadline: catalyst should check IDX for the filing and the reason. 8M 2026 bank-only profit Rp34.77 tn, +6.63% (same source).
- BEI suspended or warned **62 issuers that missed the June 2026 interim report and fine** (Written Warning III and Rp150 m fine; regular-market names include ALTO, ARKA, BEBS, BHAT, CPRI, INDX, JMAS, MREI, PMMP, RAFI, SWAT, TAYS; all-market list includes BTEL, COAL, SRIL, TDPM, TELE) (Katadata, "BEI Denda 62 Emiten yang Telat Laporan Keuangan Rp150 Juta, Ada BEBS hingga BTEL", 10-30 12:00 WIB). Treat as BOARD flags.

### EARNINGS-CHANGE pre-flags (night shift, for catalyst to confirm)
- **AMMN — up, high.** Mechanism: smelter at capacity plus much higher copper and gold output turned a US$175 m 9M loss into a US$880 m profit. Next-4-quarter profit vs trailing four quarters: **far above +10%** (trailing base includes loss quarters). Confidence high on direction; size depends on Q4 2025, not read. **Offset:** gold −3.3% on Friday; foreigners net sold Rp59.3 bn on 10-30.
- **INCO — up, medium.** 9M +180.5% on ore sales; but **Q3 fell 29.7% q/q** and the matte price is falling. Trailing growth is not the same as forward momentum: catalyst should size Q4 on ore volumes vs matte price.
- **ICBP — down, low-medium.** 9M −13.26% on what H1 showed were FX losses on loans; with the rupiah at ~Rp18,150 (weaker than at 6-30), Q3/Q4 FX losses may persist. Operating business is growing (sales +14.5%). headline-only.
- **GOTO — up, medium (unchanged).** Now with a profit-level conflict (Rp441 bn vs Rp557 bn for Q3): catalyst must read the release.
- TLKM: −3.7% attributable, **below the 10% threshold**, no flag.
- Carried from earlier notes, unchanged: PTBA up (medium), ERAA up (medium-low), BRMS down (medium-low), UNTR down, ASII down (low-medium), AALI up, ELSA up, LTLS up, ANTM up (but see gold below).

## Overnight global (US session Friday 10-30; weekend)

| Driver | Move | IHSG read-across | Source / time |
|---|---|---|---|
| US equities | **Dow 51,770.31 (−1.09%), S&P 500 7,580.07 (−1.82%), Nasdaq 25,437 (−2.86%)**, Russell 2000 2,811 (−1.66%) | Broad risk-off into the week; tech/AI-led (Intel −29%, its worst day on record, on Q4 guidance of US$15–16 bn vs ~US$17.3 bn consensus; Amazon capex ~US$220 bn for 2026). Negative for EM flows at the open | Investrade, "Market Review: October 30, 2026"; CNBC Indonesia 11-02 05:55 WIB agrees on the three closes |
| US data | Chicago PMI 55.3 (56.0 expected; 58.8 prior); Q3 ECI +0.8% (in line) | Neutral | Investrade |
| US 10-yr | ~4.91–4.93% (source inconsistent), down ~6 bp | Slight relief for EM bonds | Investrade |
| Fed | Held at 3.75–4.00% on 10-28, **10–2 vote, two dissents for a hike**; market ~75% odds of a December hike | Higher-for-longer keeps pressure on IDR and SBN | legawa, 11-01 |
| **Oil** | **Brent US$117.64 (+2.4%, expiring Dec contract; Jan US$113.43); WTI US$104.12 (+2.1%)**. October: Brent +13.6%, WTI +15.2% | Supports MEDC, ELSA, AKRA, PGAS (PGAS +8.64% on 10-30); hurts the trade balance, subsidies and IDR. 2026 deficit now projected **Rp734 tn (2.85% of GDP)** vs Rp689 tn (2.68%), on disaster spending and energy subsidies | Investrade; legawa |
| **Gold** | **Dec futures US$3,898.90 (−3.29%)**; spot ~US$3,876, about a one-year low; silver −5.93% to US$49.28 | **Negative for ANTM, MDKA, BRMS, EMAS, ARCI, HRTA; partial for AMMN** | Investrade; legawa |
| **Coal** | **Newcastle US$152.45/t (~+1.2% w/w), 24-month high** (CFD series) | Positive for PTBA, ADRO/AADI, ITMG, BUMI (PTBA +5.88% on 10-30) | legawa, citing Trading Economics |
| CPO | ~MYR4,681/t, −3% w/w (CFD series) | Mild negative for AALI, TAPG, DSNG, LSIP; weak rupiah is the offset (Kontan, "Rupiah Tembus Rp 18.100, Saham Emiten Sawit Ini Berpotensi Ketiban Untung", headline-only) | legawa |
| Nickel | not refreshed (last read LME US$16,234, 10-21/22) | INCO realized matte price fell 4.8% q/q in Q3 | — |
| China | **NBS October manufacturing PMI 49.3** (50.1 prior; 50.0 expected), back in contraction; RatingDog PMI due today | Negative for coal and nickel demand at the margin | CNBC Indonesia 11-02 05:55 WIB |
| ECB / BoJ | ECB held deposit rate 2.50% (Lagarde to step down Feb 2027); BoJ held 1.25% | Neutral | legawa |
| Asia (11-02 open) | not available at 06:15 WIB | — | — |
| This week | US midterms **11-03**; JOLTS 11-03; ADP 11-04; **NFP 11-06** (September +29k, unemployment 4.2%); ISM services | Event risk for USD and EM flows mid-week | CNBC Indonesia 11-02 05:55 WIB |

### Rupiah and bonds
- **10-30 close: Rp18,120 (CNBC) / Rp18,147 (legawa, Kontan sidebar) / ~Rp18,158 (Kontan market piece)**: snapshot differences; **JISDOR Rp18,138**. Week −0.37 to −0.44%; October −1.4%. Record weak close Rp18,175 on 10-28.
- **10-yr SBN 7.64%** (touched 7.71% on 10-29, highest since May 2020), +~19 bp on the week. SUN auction 10-27: bids Rp31.1 tn (−52%), awarded Rp20.7 tn vs Rp30 tn target, bid-to-cover 1.04x (legawa, 11-01). **Read:** weak demand for government paper is a fresh stress point; watch for BI action.
- BI-Rate 5.75%, unchanged; BI is offering hedging-cost incentives, SRBI issuance and SBN purchases; FX reserves (September US$146.3 bn) due **11-06**; Q3 GDP due **11-05** (Q2 5.29% y/y).

## Analyst framing for the week
- Herditya Wicaksana (MNC Sekuritas): selling likely to persist; **support 4,907, resistance 5,317**; picks EXCL (1,765–1,990), MEDC (1,430–1,465), TAPG (1,970–2,030), plus SQMI (Kontan, "IHSG Terkoreksi 7,03% Sepekan, Simak Proyeksi dan Rekomendasi Saham Pekan Depan", 10-30 18:57 WIB; investor.id, "Prediksi IHSG dan Rekomendasi Saham Senin, 2 November 2026", 10-30 20:00 WIB). No rationale given.
- Alrich Paskalis Tambolang (Phintraco): IHSG may test **4,900–5,000**; above 5,000, sideways 5,000–5,200 (same sources).
- Positives cited: government mitigation, issuer buybacks without an AGM extended into 2027. Negatives: MSCI, rupiah, possible Fed hike.
- Hendra Wardana: ahead of the MSCI review watch ADRO, PTBA, MEDC (investor.id 11-02 05:00 WIB).

## Attention scores (partial; press-based)
Disclosure (+3), volume ratio (+2) and ARA/ARB (+1) cannot be tool-checked. The gap point (+2) is given where the press reports a close-to-close move of 3% or more. Flow point (+1) only for the six names in the published top 3 each side. **Read them as lower bounds.**

| Ticker | Outlets (24–72 h) | Gap ≥3% | Flow | Partial score | Story |
|---|---|---|---|---|---|
| **AMMN** | 3 | 0 (not read) | +1 | **4+** | 9M US$880 m vs loss; gold −3.3% |
| **PTBA** | 2 | +2 (+5.88%) | 0 | **4+** | coal at 24-month high; MSCI watch name |
| **EXCL** | 2 | +2 (+5.85%) | 0 | **4+** | MNC pick; results not found |
| **GOTO** | 2 | 0 | +1 | **3+** | top net buy; Q3 profit conflict; TP cut |
| **TLKM** | 3 | 0 | +1 | **4+** | 9M attributable −3.7%; Rp119.5 bn net sell |
| **INCO** | 4 | 0 | 0 | **4+** | 9M +180.5%, Q3 −29.7% q/q |
| PGAS | 1 | +2 (+8.64%) | 0 | **3+** | oil; no story found |
| BRPT | 1 | +2 (−6.96%, likely ARB) | 0 | **3+** | no story found |
| ISAT | 1 | +2 (−6.83%) | 0 | **3+** | no story found (9M profit +37.2% was 10-28) |
| CUAN | 1 | +2 (−6.83%) | 0 | **3+** | no story found |
| BBRI | 1 | 0 | +1 | 2+ | Rp206.5 bn net sell; Q3 release status unclear (limited review) |
| BBCA | 2 | 0 | 0 | 2+ | Samuel TP Rp5,800 |
| ICBP | 1 | 0 | 0 | 1+ | 9M −13.3% (headline-only) |

## Board
- **HSC exclusion from IHSG effective today.** Short-sell list emptied; 11 names off the margin list (names not found).
- 62 issuers at Written Warning III / suspended for the missing June interim report (Katadata, 10-30; names above).
- Open from earlier notes: ARKO (suspended 10-28), MSIN and BSWD (suspended since 10-21), LUCY and VKTR (UMA). No new UMA notice found this weekend.

## Corporate actions in the window (from intel/calendar.json; not updated by this pre-market run)
- **SIDO cum interim dividend today (11-02)**, Rp10; ex 11-03 (CNBC also lists it this week).
- **TSPC ex dividend today (11-02)**, Rp75.
- Prima Globalindo Logistik (PPGL) cum bonus shares this week (date not in the CNBC article): unverified.
- UNTR cum 11-05 (Rp430). BRIS RUPSLB on its rights issue 11-06. TPIA buyback up to Rp2 tn (max Rp3,000) running; AMMN Rp1 tn buyback (from 10-22).
- **To add in the evening calendar update:** MSCI review 11-11 (effective 12-01); Q3 GDP 11-05; FX reserves 11-06.

## For the morning desk (2026-11-02)
1. **Risk-off open likely:** Nasdaq −2.9%, S&P −1.8%, gold −3.3%, China PMI back below 50. Against that, foreign selling on Friday fell to ~Rp0.17 tn and IHSG held 4,979 intraday. Supports 5,000 / 4,907; resistance 5,200 then 5,317.
2. **Today's data (PMI, CPI, trade balance) and the HSC exclusion start** will move the index mid-morning; avoid reading the first hour as a trend.
3. **Commodity split:** coal (24-month high) and oil (Brent US$117) favour PTBA, ADRO/AADI, MEDC, PGAS; gold's −3.3% is a headwind for ANTM, MDKA, BRMS, EMAS.
4. **AMMN** is the strongest new results story (loss to US$880 m, smelter at capacity, guidance on track) but faces gold weakness and foreign selling: catalyst should read the release.
5. **INCO**: 9M looks great, Q3 fell 30% q/q: don't buy the headline.
6. **GOTO**: two different Q3 profit figures (Rp441 bn vs Rp557 bn): read the release before using either.
7. **BBRI** Q3 still not out and under a limited review: check IDX for the filing and any corporate-action disclosure.
8. Run `tools/prices.py scan` for Friday's ARA/ARB list (BRPT likely ARB) and refresh nickel and Asia; the cloud could not.
