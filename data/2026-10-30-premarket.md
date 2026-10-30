# Pre-market intel — Friday 2026-10-30 (IDX trading day)

Run: cloud night shift, 06:12 WIB (tools/clock.py: trading_day=true, before_open=true, last session 2026-10-29).
Paper holdings: none (desk/paper/portfolio.json: cash Rp150,000,000, no positions; desk/watchlist.json empty). intel/alerts.md: no change.

## Data access — read first
- `tools/idx.py` and `tools/prices.py` still return `unavailable`: the proxy refuses CONNECT to www.idx.id and query1.finance.yahoo.com (403, 2026-10-30 06:13 WIB). **Twelfth run in a row** with this block.
- So there are **no tool-checked disclosures, OHLCV, volume ratio, gap, ARA/ARB or flow numbers** here. All figures come from news pages and search results.
- Refused or failed fetches: Bisnis (rupiah page for 10-30, PGEO results page), Kontan (GOTO treasury-share page). Their stories are **headline-only** unless another outlet is cited.
- **Commodity prices were not refreshed**: no dated coal, nickel or CPO print for 10-29 was found. Last readable figures are in the global table below with their dates.

## Read first: foreigners sold Rp1.07 tn on 10-29; BBCA −6.35% to Rp4,940
- **Full-day foreign flow 10-29: net SELL ~Rp1.07–1.08 tn** (investortrust, "Net Sell Jumbo Rp 1,07 Triliun, Pemodal Asing Obral BBCA hingga BUMN Ini", 18:05 WIB; investor.id, "Asing Ngamuk Lagi, BUMI Justru Curi Perhatian", 21:20 WIB; Kontan 19:14 WIB says Rp1.08 tn). **Conflict:** Kontan's bank piece (18:14 WIB) says Rp1.52 tn; take ~Rp1.07 tn (three outlets) and treat the larger figure as unverified (likely all markets incl. negotiated).
- Year to date: ~Rp97.7 tn foreign net sell (investor.id; Kontan Rp97.78 tn). IDX Channel (12:34 WIB) gives Rp124.67 tn YTD and Rp13.91 tn since the MSCI announcement on 10-16: different basis, unreconciled.

| Net sell (regular) | Rp bn | Net buy (regular) | Rp bn |
|---|---|---|---|
| **BBCA** | **503.49** | **ENRG** | **321.81** |
| BBRI | 164.50 | CASA | 65.23 |
| BMRI | 155.86 | DNET | 49.86 |
| ANTM | 103.27 | AMRT | 43.65 |
| TLKM | 76.53 | BUMI | 34.85 |
| BBNI | 36.68 | CUAN | 30.2 |

Sources: investortrust 18:05 WIB (top 5 each side); investor.id 21:20 WIB (BUMI, CUAN); Kontan, "Saham Big Banks Kompak Melemah (29/10), Asing Ramai-ramai Jual Saham, BBCA Terparah", 18:14 WIB (BBNI).

- **Big-bank closes 10-29** (Kontan 18:14 WIB): **BBCA Rp4,940 (−6.35%)**, BBRI Rp2,810 (−3.77%), BMRI Rp3,720 (−3.12%), BBNI Rp3,240 (−3.28%). This settles the evening note's "Rp4,940–4,975, unverified": **BBCA closed at Rp4,940**, below the Rp5,000 round number and inside CGS's earlier Rp4,713–4,807 support zone only if it falls another ~3%.
- **ENRG: second day as the top foreign net buy (Rp322 bn after Rp300 bn on 10-28)** although it was at ARB in the first hour on 10-29 (evening note). Close not found. Foreign buying into an ARB is unusual: the morning desk should check the close, the volume and whether the buyer is one broker (Trimegah was a buyer on 10-23; Bakrie Kalila bought 174.39 m shares). Treat as **unverified flow signal**, not a value call.
- **ANTM: Rp103 bn net sell** despite 9M profit +36% (IDX Channel, below). Gold fell 0.5% overnight.
- Sectors (investor.id 21:20 WIB): industrials −4.6%, basic materials −4.5%, infrastructure −4.2%, energy −3.29%. Value Rp11.03 tn. Breadth 104 up / 653 down / 206 flat.
- **ARA at the close:** ALKA +24.86% to Rp4,420 and YPAS +24.85% to Rp1,055 (investor.id, "IHSG Ambles 3% Lebih, 2 Saham Malah ARA", 16:22 WIB). **Closing ARB list: still not found** (25 names in the first hour; only ENRG and MORA named). Morning desk: run `tools/prices.py scan`.

## Overnight results (Indonesian issuers)

| Ticker | Period | Revenue | Net profit (attrib.) | Read | Source |
|---|---|---|---|---|---|
| **GOTO** | 9M 2026 | Rp16.54 tn, +24.47% (Rp13.29 tn) | **Rp1.16 tn vs a loss of Rp775.55 bn** | Operating profit Rp864.17 bn (loss Rp222.36 bn); costs +14.04%, slower than revenue | Kontan, "GOTO Cetak Laba Bersih Rp 1,16 Triliun Per Kuartal III 2026", 17:31 WIB |
| **GOTO** | Q3 2026 | Rp5.6 tn, +17% | **Rp441 bn vs a loss of Rp255 bn** | Adjusted EBITDA Rp950 bn (+84%); operating profit Rp351 bn; core GTV Rp194 tn (+89%); adjusted FCF Rp1.209 tn (+389%). **2026 adjusted EBITDA guidance raised to Rp3.5–3.7 tn** (prior target not stated in the article) | investor.id, "GOTO Cetak Laba Bersih Rp 441 Miliar, Target EBITDA Naik", 21:50 WIB; tirto, detik, Okezone agree on Rp441 bn |
| BTPS | 9M 2026 | — | Rp1.01 tn; financing +13% | headline-only; yoy not read; release date not confirmed as 10-29 | Kontan / Liputan6 / Fortune IDN headlines |
| BDMN | 9M 2026 | — | ~Rp3.5 tn, +19% | headline-only (Kontan related link) | Kontan sidebar |
| PGEO | 9M 2026 | — | Rp2.29 tn | headline-only; yoy not read (Bisnis refused) | Bisnis headline, 10-29 |
| AGII | 9M 2026 | — | Rp114.3 bn, +79% | small cap; headline-only | Kontan headline |
| FORE | 9M 2026 | — | Rp90 bn, +85% | headline-only | Katadata Databoks headline |

- **CDIA conflict resolved:** IDX Channel (via RCTI+, "Oktober Biasanya Hijau, tapi IHSG Dihantam Badai MSCI...", 12:34 WIB) gives **US$32.2 m ≈ Rp579.6 bn** net profit, revenue +16%, EBITDA +65%. The Rp898 bn headline is likely total incl. minorities; unverified.
- Same IDX Channel roundup (9M yoy, for reference): BMRI +20.7% to Rp45.5 tn (Q3 +14%); AALI +76.9%; HMSP +44.4%; ANTM +36%; MCOL +68.3%; TOTL +51.9%; CBPE +72%; JARR +55.9%; SIDO −24.4%; HEAL −14.8%; BANK −63.1%; BNLI −10.9%. BBCA +4.2% and BBNI +6.6% as already noted.
- **Still not out (search, 06:30 WIB):** BBRI, TLKM, BRIS, ICBP/INDF, AADI/ADRO/ITMG, MEDC, INCO/MDKA/AMMN, EXCL/ISAT. The 10-31 deadline is a Saturday, so expect a heavy flow of filings today. (Search results showing TLKM −10.69% and ICBP −12.77% are **Q3 2025**, not 2026.)

### EARNINGS-CHANGE pre-flags (night shift, for catalyst to confirm)
- **GOTO — pre-flag, up, medium.** Mechanism: revenue +17–24% with costs +14% turned a loss into Rp1.16 tn 9M profit; Q3 alone Rp441 bn; EBITDA guidance raised. Size: next-4-quarter net profit vs the trailing four quarters is **far above +10%** because the trailing base includes loss quarters (exact size depends on Q4 2025, not read). Confidence: **medium** — check how much is fair-value or other income (operating profit Rp351 bn in Q3 is below net Rp441 bn, so ~Rp90 bn is non-operating). Foreigners net bought GOTO Rp49 bn on 10-28.
- Carried from the 10-29 evening note, unchanged: **PTBA up (medium)**, ERAA up (medium-low), BRMS down (medium-low), UNTR down (already priced?), ASII down (low-medium), AALI up, ELSA up, LTLS up, ANTM up.

## Policy and market structure
- **Hashim Djojohadikusumo (chair of Kadin's advisory council) on "saham gorengan":** at Kadin's Rapimnas he said stock manipulation and thin free float make P/E ratios "gila-gilaan", that MSCI has raised this, and that continued foreign outflows could push the rupiah to **Rp20,000–21,000/US$** (other outlets headline Rp22,000). He said the government will act firmly (no specifics) and cited Turkey's 94 arrests. Sources: CNBC Indonesia, "Hashim: Praktik Goreng Saham Bikin Rupiah Bisa Tembus Rp 21.000/US$", 10-29 15:59 WIB; investor.id, "Hashim Peringatkan Pengusaha: Stop Goreng-goreng Saham, Pemerintah akan Tindak Tegas", 10-29 (headline-only); Suara / Liputan6 (Rp22,000 headlines). **Read:** a political signal of enforcement against conglomerate/low-float names; it adds to the headline risk on HSC and thin-float stocks into the 11-02 IHSG exclusion. Not a policy act yet.
- Analyst framing (Kontan, "IHSG Anjlok 3,49% ke 5.098, Waspadai Jika Sentuh Support di Level 4.980 Jumat (30/10)", 19:14 WIB): Hendra Wardana (Republik Investor) — loss of confidence, not valuation, is the core issue (MSCI review, ownership transparency, governance, trading-mechanism credibility); support **4,980**, then 4,900; resistance 5,200, rebound zone 5,150–5,200 "short-term only". Herditya Wicaksana (MNC Sekuritas) — support **5,046**, resistance **5,155**; picks BBNI, INDY, ISAT (no rationale read).
- MSCI Standalone consultation (decision by 2027-06-30) and the HSC exclusion from IHSG on **11-02** are unchanged. IDX Channel puts IHSG at −15.31% in October and −12.26% since the 10-16 MSCI announcement.

## Overnight global (US session 10-29, closed 04:00 WIB 10-30)

| Driver | Move | IHSG read-across | Source / time |
|---|---|---|---|
| US equities | Dow −0.25% (52,342), **S&P 500 −0.31% (7,720), Nasdaq −1.38% (26,184)**; Russell 2000 +1.01%; 8 of 11 S&P sectors up | Tech-led (Alphabet −12% on a revenue/search miss); breadth was fine. Neutral to mildly negative for EM risk appetite | Investrade, "Market Review: October 29, 2026"; TradingKey, 20:12 ET |
| After hours | **Amazon −5.4%** (fell as much as −11%; AWS beat, revenue and ads missed); **Intel −21%** on Q4 guidance | Nasdaq futures likely soft at the Asian open; little direct IDX read-across | TradingKey, as above |
| US data | Q3 GDP **+3.4%** annualized (3.1% expected); Q3 core PCE price index 2.5% (2.4% expected), headline 2.1% (2.6%); September PCE m/m headline +0.5%, core +0.3% (in line) | Firm growth and sticky core keep December-hike odds alive (~80–85% before the data, per the 10-29 note) | Investrade, as above |
| US 10-yr | **4.988%, −5.6 bp**, ending a four-day rise | Slight relief for EM bonds and the rupiah | Investrade |
| ECB | Held; flagged energy as upside inflation risk. Euro to a 17-month low near US$1.11 | Stronger USD vs EUR; mixed for IDR | Investrade |
| Oil | **WTI US$102.00 (−0.76%)**; Brent ~US$110.6–114.9 (source inconsistent) | Still very high: supports MEDC, ELSA, AKRA, PGAS margins; hurts the trade balance and IDR | Investrade |
| Gold | Dec futures **US$4,031.4 (−0.50%)** | Mild negative for ANTM, MDKA, BRMS, EMAS, ARCI | Investrade |
| Coal | Not refreshed. Last read: Newcastle Nov US$150.00, Dec US$153.00 (10-27 session) | PTBA/ITMG/AADI read-across unchanged | investor.id, "Harga Batu Bara Anjlok, Stok India Masih Jadi Sorotan", 10-28 08:22 WIB |
| Nickel / CPO | Not refreshed. Last read: LME nickel US$16,234 (10-21/22), CPO MYR4,747 (10-22) | Stale; morning desk should refresh | kumparan, 10-22 08:06 WIB |
| Asia (10-30 open) | Not available at 06:30 WIB | — | — |

### Rupiah
- **10-29 close Rp18,137/US$, +0.26%; JISDOR Rp18,128 (+0.30% from Rp18,183).** Off the 10-28 record low. Rahma Gafmi (Universitas Airlangga) sees **Rp18,100–18,230** today; cites BI triple intervention (spot, DNDF, SBN), foreign equity outflows, MSCI, and oil's pressure on FX demand (Kontan, "Rupiah Menguat Hari Ini, Cek Sentimen dan Proyeksi Jumat (30/10)", 16:19 WIB). CNBC's 15:10 figure (Rp18,125) differs by Rp12: different snapshot.
- Bisnis' 10-30 morning rupiah page was refused: **headline-only**.

## Attention scores (partial; press-based)
Disclosure (+3), volume ratio (+2) and gap (+2) components cannot be computed without IDX/Yahoo access. Scores below use outlets (cap 5), the ARA/ARB point where the press confirms it, and the top-20 foreign-flow point. **Read them as lower bounds.**

| Ticker | Outlets (24 h) | ARA/ARB | Flow top 20 | Partial score | Story |
|---|---|---|---|---|---|
| BBCA | 5 | 0 (−6.35%, inside the 7% band) | +1 | **6+** | DBS merger rumour denied; largest foreign net sell; −6.35% |
| GOTO | 5 | 0 | 0 (not read for 10-29) | **5+** | 9M profit Rp1.16 tn vs loss; EBITDA guidance up |
| ENRG | 3 | +1 (ARB in session I; close not confirmed) | +1 | **5+** | Top foreign net buy two days running despite ARB |
| PTBA | 5 | 0 | 0 | **5+** | 9M profit +216% (10-29) |
| BBRI | 3 | 0 | +1 | 4+ | −3.77%, Rp164.5 bn net sell; results due |
| BMRI | 3 | 0 | +1 | 4+ | −3.12%, Rp155.9 bn net sell (7th day) |
| ANTM | 2 | 0 | +1 | 3+ | Rp103 bn net sell; gold −0.5% |
| ALKA, YPAS | 2 | +1 | 0 | 3+ | ARA, no story; illiquid |

## Board
- No new suspension or UMA notice found overnight. Open from earlier notes: ARKO (suspended 10-28), MSIN and BSWD (suspended since 10-21), LUCY and VKTR (UMA). HSC exclusion from IHSG and LQ45/IDX30/IDX80 from **11-02**; BEI is moving to account freezes instead of UMA flags (detik, "Pasar Modal Dibersihkan, Kepercayaan Investor Dipulihkan", 10-29 08:00 WIB, citing Hans Kwee).

## Corporate actions due in the window (from intel/calendar.json; not updated by this run)
- **TSPC cum dividend today (10-30)**, Rp75. SIDO cum 11-02 (conflict with an earlier 10-28 date). UNTR cum 11-05 (Rp430). BRIS RUPSLB on rights issue 11-06. TPIA buyback up to Rp2 tn, max Rp3,000, running from 10-29.

## For the morning desk (2026-10-30)
1. **IHSG 5,098 after a −3.49% day on a Rp1.07 tn foreign net sell.** Analyst supports: 5,046 and 4,980; the 10-19 intraday low was 4,907. US was mixed overnight (Nasdaq −1.4%, 10-yr yield down), rupiah firmer: no fresh global shock, so today hinges on foreign flow into the banks.
2. **GOTO** is the cleanest new results story: profit swing, EBITDA guidance raised. Catalyst should read the release for the non-operating line and the prior guidance.
3. **ENRG**: foreigners bought Rp322 bn into an ARB day. Check the close, broker concentration and whether rights-issue holders are the sellers before reading anything into it.
4. **BBCA closed Rp4,940**: below Rp5,000 with the rumour gone. Watch whether foreign selling (Rp503 bn) continues.
5. Expect many Q3 filings today (BBRI, TLKM, BRIS, Indofood group, coal and metal names) before the Saturday deadline.
6. Run `tools/prices.py scan` for the 10-29 ARB list and refresh coal, nickel and CPO; the cloud could not.
7. Hashim's "goreng saham" warning raises headline risk on thin-float and HSC names ahead of the 11-02 exclusion.
