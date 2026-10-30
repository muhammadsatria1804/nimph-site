# Pre-market intel — Monday 2026-10-26 (IDX trading day)

Run: cloud night shift, 06:12 WIB (tools/clock.py: trading_day=true, before_open=true, last session 2026-10-23).
Paper holdings: none (desk/paper/portfolio.json, cash Rp150,000,000). intel/alerts.md: no change.

## Data access — read first
- `tools/idx.py` and `tools/prices.py` still return `unavailable`. The cloud proxy refuses CONNECT to www.idx.id and query1.finance.yahoo.com (403, 2026-10-26 06:12 WIB). This is the same sandbox allow-list issue as in the last three runs.
- So this note has **no tool-checked disclosures, OHLCV, volume ratio, gap, ARA/ARB or tools/flow.py numbers**. All figures come from news pages and search results.
- These pages refused the fetch: Kontan (pusatdata, investasi), Kompas, Mediakompeten, Bloomberg, CNBC.com and FXLeaders. Stories from them are marked **headline-only**.

## Last IDX session (2026-10-23) and the week
- IHSG closed at **5,439.26, +0.95%**, its fourth gain in a row. Weekly change **+4.90%** (from 5,185.10); the week's range was 4,907.37 to 5,455.21. Source: Katadata, "Net Sell Asing Tembus Rp 6,67 T Sepekan, BBCA hingga BBRI Ramai Ditransaksikan", 2026-10-25 08:52.
- Benchmark since paper inception: 5,328.36 (close 2026-10-21) → 5,439.26 = **+2.08%**.
- Weekly IHSG contributors: BMRI +40.65 pts (+15.04% on the week), BBRI +39.76 pts (+10.23%), TLKM +31.31 pts (+17.89%). BBCA was the main drag at −13.66 pts (−2.9%). Katadata, as above.
- Technical read from InvestorTrust: IHSG is above 5,400 but below its MA20 (~5,813), and MACD is still negative. They call it a technical rebound, not a confirmed reversal. Analysts' range for today is 5,400–5,544; Phintraco sees 5,500–5,600 this week. Sources: InvestorTrust, "IHSG Bisa Menguat Uji 5.540 Hari Ini, Tiga Saham Dipimpin HRUM Layak Dilirik", 2026-10-26 05:45 WIB; Bisnis, "Rekomendasi Saham dan Pergerakan IHSG Hari Ini, Senin 26 Oktober 2026", 2026-10-26 04:58 WIB.

### Net foreign flow (press estimates, not tools/flow.py)
- **2026-10-23 full day: net sell Rp1.29 tn**, concentrated in banks: BBCA Rp766.98 bn, BBRI Rp346.82 bn, BBNI Rp101.25 bn (InvestorTrust, as above). The Kontan pusatdata headline gives the same Rp1.29 tn ("IHSG Menguat Hari Keempat, Asing Tetap Net Sell Rp 1,29 Triliun pada Jumat (23/10)"; headline-only). Kompas's headline says Rp1.28 tn (headline-only). This closes the gap in the evening note, which had session I only.
- **Week of 19–23 Oct: net sell Rp6.67 tn** (sell Rp43.62 tn, buy Rp36.95 tn), up from Rp3.19 tn the week before (Katadata, as above). The IHSG rose 4.9% against this, so the rebound is domestic money (JawaPos, "IHSG Rebound 4,9 Persen Sepekan, OJK Sebut Investor Domestik jadi Penopang", 2026-10-25; headline-only).
- Net buy leaders for the full day: **not found**. The morning desk should run tools/flow.py.

### ARA (press, not tool-checked)
- WMUU +33.33% (Rp36), TOBA +25% (Rp520), FAST +25% (Rp380), PTSP +25% (Rp2,250), KONI +24.91% (Rp1,680). No stories found for any of them. Source: InvestorTrust, 2026-10-26 05:45 WIB. This matches the evening note.

## Overnight global (US session 2026-10-23, closed ~04:00 WIB 2026-10-24; weekend news to 2026-10-25)
| Driver | Move | IHSG read-across | Source / time |
|---|---|---|---|
| S&P 500 | 7,623.68, −0.52% | mild risk-off into Fed week | Capp Notes, "Closing Look — Friday, October 23, 2026" |
| Nasdaq / Dow | 25,955.34, −0.21% / 52,215.16, −1.23% | Tech steadied after Thursday's AI-capex rout; the Dow fell on telecoms and AmEx. Neutral to slightly positive for DCII and tech names versus Thursday | same; Reuters via Spokesman-Review, "Dow, S&P 500 fall, tech steadies to end rocky week", 2026-10-23 |
| US futures, Sunday | "climb as crude oil price dips" | supportive at the open | Bloomberg headline, "US Equity Futures Climb as Crude Oil Price Dips: Markets Wrap", 2026-10-25; **headline-only**, no figures |
| Asia, 2026-10-23 | Nikkei −0.34% (62,693); Shanghai +0.89%; Hang Seng +0.69%; Kospi +0.30% (recovered from −4% intraday); Taiwan closed for a typhoon | Asia recovered intraday on Friday; state funds stepped in in China | Capp Notes, as above |
| Brent | settled **US$116.72, +3.14%** on Friday, the highest since 29 Apr and about +6% on the week. WTI US$103.27, +3.80%. Sunday indication about **US$115.6, about −1%** | + upstream oil and gas (MEDC, ENRG) and energy services; − fuel users (GIAA, logistics), the fuel-subsidy budget and the rupiah | Capp Notes; FinanceFeeds, "Brent Crude Price: $116.72 Into Sunday Open, Bull $120", 2026-10-25; Trading Economics Brent page, 2026-10-25 (its figures conflict: 115.57–115.70) |
| Oil, weekend news | The Houthis **claim** strikes on Aramco's Yanbu facilities, the Rabigh refinery and the East-West Pipeline. The Saudi coalition reports interceptions and has not commented on damage. **No damage confirmed.** The US ordered non-emergency staff out of its Saudi missions; no US strike on Iran as of Sunday morning | If damage is confirmed, Brent could reach US$120+; if not, about US$108. Headline risk for oil names both ways | FinanceFeeds, as above, citing Reuters and Al Jazeera |
| Gold | spot about **US$3,996**, the first close below US$4,000 since mid-July; **−4% on the week**, the worst week since June | − gold miners (ANTM, MDKA, EMAS, BRMS, PSAB, AMMN's gold side). Brokers still recommend ANTM as a buy (target Rp3,000–3,150), against the metal | FinanceFeeds, "Gold Price Sunday: $3,996 Into Fed Week, Bear $3,890", 2026-10-25 15:22 (UTC+3); InvestorTrust, as above |
| Copper | US$6.476/lb, +1.78% | + AMMN, MDKA (copper side) | Capp Notes, as above |
| Coal | 150.70, −0.30% (10-23); +5% over the month | neutral for PTBA, AADI, ITMG, HRUM. HRUM is a broker buy at Rp775–810 with no story | Trading Economics, coal page (id), 2026-10-23 |
| Nickel | 15,865, −0.81% (10-23) | slightly negative for INCO, NCKL, MBMA, ANTM | Trading Economics, as above |
| CPO | **unverified**: the last figure found is MYR 4,747/t, −1.04% (close of 10-21) | — | kumparan, "Harga Komoditas: CPO, Batu Bara dan Nikel Melemah", 2026-10-22 08:06 WIB |
| USD/IDR | **18,067**, −0.01% on Friday | weak rupiah plus Brent near US$117 means imported-inflation pressure | Bisnis, 2026-10-26 04:58 WIB, as above |
| US 10-yr / DXY | 4.999% (+5 bp) / 101.79 (+0.18%) | a firm dollar and US yields near 5% keep pressure on EM flows | Capp Notes, as above |
| Fed | The FOMC decides on Wed 2026-10-28 (early 2026-10-29 WIB). CME FedWatch: 92% hold. A **December hike is priced at 78%** (Yardeni 84%). PCE is due Thursday; US midterms are on 2026-11-03 | foreign outflow risk persists through the week | FinanceFeeds gold story, as above |

Morning read: Wall Street was mixed to soft on Friday, and US futures are higher Sunday night as oil eases. IHSG starts the week on a 4.9% domestic-led rebound with heavy, persistent foreign selling of the big banks. Watch oil names on the Yanbu headlines (unconfirmed). Gold miners are the relative losers. With the Fed on Wednesday and a December hike priced, foreign selling is unlikely to stop this week.

## Market structure
- **MSCI**: on 2026-10-15/16 MSCI opened a consultation on moving Indonesia from Emerging to **Standalone** market status. The consultation closes **2027-04-30** and the decision comes by **2027-06-30**. Estimated passive outflow is US$3–6 bn; one analyst estimate, including active funds, is about US$19 bn. The free-float bar is 15%, and the first BEI deadline for large issuers is 2027-03-31. Source: Ajaib, "MSCI Usulkan Indonesia ke Standalone Market, Menakar Risiko Outflow dan Persoalan Free Float", 2026-10-21. This is a secondary source; the morning desk can read MSCI's own announcement. This is the structural reason for the foreign selling, and it will not resolve inside the 10-day horizon.
- **HSC exclusion from IHSG on 2026-11-02**: the HSC list now has **82** stocks (Bisnis, "Daftar Saham HSC Bertambah Jadi 82 Emiten, Cek Selengkapnya", 2026-10-23; headline-only). The evening note's figure of 80 is out of date. The effective date falls inside any ticket opened today.
- **Buyback wave** (the new AMMN, INDF and ICBP programmes are funded from internal cash; whether a RUPS is needed was not stated):

| Ticker | Size | Window | Source |
|---|---|---|---|
| **AMMN** | up to Rp1 tn (≤0.37% of shares) | 2026-10-22 → 2027-01-22 | Suara, "Siapkan Dana Rp1 Triliun, AMMN Gelar Buyback Saham", 2026-10-25 16:35 WIB; Liputan6 (headline-only) — **new** |
| **INDF** | up to Rp750 bn | 2026-10-26 → 2026-12-31 | Suara, "Dua Emiten Grup Salim INDF dan ICBP Mau Buyback Saham Rp750 Miliar", 2026-10-25 16:11 WIB — **new, starts today** |
| **ICBP** | up to Rp750 bn | 2026-10-26 → 2026-12-31 | same — **new, starts today** |
| BBRI | up to Rp1 tn (phase II, for an employee/management share plan) | 2026-10-22 → 2027-01-21 | CNBC Indonesia, "BRI (BBRI) Umumkan Lanjut Buyback Saham, Siapkan Rp1 Triliun", 2026-10-23 08:10, citing the IDX disclosure of 2026-10-22 |
| BBCA | not stated; extended to 2026-10-23 | part of the 2026-03-12 RUPST programme to 2027-03-11 | JawaPos, "Daftar 8 Emiten Umumkan Buyback Saham, dari Grup Barito hingga BCA", 2026-10-25 17:17 WIB |
| TLKM | 15.96 m shares bought on 2026-10-20 | — | JawaPos, as above |
| BRPT, BREN, DSSA | Rp1 tn each | 10-19 → 12-31 (DSSA to 2027-01-18) | kumparan, "Daftar Saham Buyback Oktober 2026, Cek Nilai dan Jadwalnya", 2026-10-22 09:51 WIB |
| CUAN / PBSA | Rp500 bn / Rp100 bn | 10-19 → 12-31 / 10-20 → 2027-01-19 | same |

Pages 2–3 of the JawaPos list (six more issuers) were not retrieved.

## Issuer stories (24 h), attention (partial: outlets only)
Formula parts not computed: disclosure +3, volume ratio, gap, ARA/ARB, top-20 flow. The morning desk adds these with the tools.

| Ticker | Outlets (24 h) | Story | Status |
|---|---|---|---|
| **AKRA** | 3 (Bisnis, Kontan ×2, Mediakompeten) | 9M 2026 revenue **Rp46.53 tn, +43.6%**; attributable net profit **Rp2.21 tn, +34.0%** (total Rp2.44 tn, +32.3%). Gross profit +30.5% (gross margin about 7.8%, down because cost of revenue rose 44.9%); operating profit +31.7%. Liabilities Rp22.38 tn, equity Rp16.25 tn. LQ45 top gainer on Friday | Read in full: Bisnis, "Pendapatan Melonjak 43,6%, Laba Bersih AKRA Tembus Rp2,21 T hingga Kuartal III/2026", 2026-10-25 22:22 WIB; StockWatch, "Laba Bersih AKRA Tumbuh 32,27% Jadi Rp2,44 Triliun per September 2026, Ini Pemicunya", 2026-10-23. Segment split (fuel trading vs JIIPE land) **not given**. The Kontan stories are headline-only |
| **AMMN** | 2 (Suara, Liputan6) | Rp1 tn buyback (above). Was a foreign net buy on 10-22. The gold drop works against it; copper's rise works for it | as above |
| **DEWA** | 1 (Bisnis) | 9M revenue Rp5.10 tn, +9.7%; attributable net profit **Rp513.08 bn, +114.6%**. Gross profit +53.7%; pre-tax profit +98.2%. **Net other income Rp260.20 bn** (Rp19.86 bn a year earlier) is about 39% of pre-tax profit and is not explained. Finance costs Rp319.43 bn, +79%; G&A +77%. LQ45 top gainer on Friday | Read in full: Bisnis, "Laba Darma Henwa (DEWA) Naik 114,55% Jadi Rp513 Miliar Kuartal III/2026", 2026-10-25 21:21 WIB. It confirms the Kuhuni figures from the evening note |
| **DMAS** | 1 (Bisnis) | 9M revenue **Rp2.65 tn** (about 3.4×); net profit **Rp1.49 tn** vs Rp525 bn. Bisnis prints "+284%", but 1.49/0.525 = 2.84×, which is **+184%**; use +184%. 96% of revenue is industrial land, mostly to **data-centre buyers**. Gross margin 61%, net margin 56%, cash Rp1.8 tn, no debt. The press says the pre-sales target was raised to Rp2.95 tn (headline-only). Dividend cum 10-28 | Read in full: Bisnis, "Emiten Grup Sinarmas, Puradelta (DMAS) Bukukan Pendapatan Rp2,65 T Kuartal III/2026", 2026-10-25 16:10 WIB |
| INDF / ICBP | 1 (Suara) | Rp750 bn buyback each, from today | as above |
| BMRI | 1 (investor.id) | "Ramalan Saham Bank Mandiri (BMRI) Usai Kinerja Kuartal III-2026" | **headline-only** |
| BBCA, BBRI, BBNI | 2+ | Largest foreign net sells on Friday (above). BBRI phase-II buyback | as above |
| BTPS | 2 (EmitenNews, Mediakompeten) | 9M net profit Rp1.01 tn | **headline-only**: "BTPN Syariah (BTPS) Toreh Laba Rp1,01 Triliun hingga Kuartal III 2026"; the date and the yoy change were not read |
| HRUM, ANTM, CUAN | 0 original | Broker buy calls only (BRI Danareksa): HRUM Rp775–810, ANTM Rp3,000–3,150, CUAN Rp590–620 | InvestorTrust, 2026-10-26 05:45 WIB. Not a story; low weight |
| BUMN Karya (PTPP, ADHI, WIKA, WSKT) | 1 (Kontan) | "Menakar Prospek Kinerja Emiten BUMN Karya Jelang Wacana Merger Akhir 2026": merger talk for the end of 2026 | **headline-only** |

### EARNINGS-CHANGE pre-flags (night shift, for catalyst to confirm)
- **AKRA**: revenue +44% and attributable profit +34% on 9M. A next-4-quarter net profit change of +15–30% is plausible. The mechanism is not yet known: it may be fuel-trading volume and price (Brent is high) or JIIPE land sales (lumpy). Confidence **medium-low** until the segment note in the FS is read. Liquid LQ45 name; it was a top gainer on Friday, so check the gap and ATR before any ticket.
- **DMAS**: upgraded from the evening note's +30% to +150%. Bisnis confirms the data-centre land demand and the raised pre-sales target. Profit still depends on handover timing, so the size stays **+30% to +150%** with confidence **low to medium**. CORP-ACTION: dividend cum **2026-10-28** (Rp29, unverified) falls inside any holding period.
- **DEWA**: profit +115%, but about 39% of pre-tax profit is unexplained other income. Underlying profit (gross profit +54%) is still up strongly. Confidence **low** until the other-income note is read.

## Corporate actions in the next 10 trading days (news; confirm with tools/idx.py actions)
- New: **INDF and ICBP buybacks start 2026-10-26**; AMMN's buyback runs to 2027-01-22.
- Carried over: SCMA cum **10-27**; DMAS and AXIO cum **10-28**; VISI private placement **10-28**; HSC exclusion from IHSG **11-02**; DOOH RUPSLB **11-09** (rights issue); AALI buyback to 12-28.
- intel/calendar.json is not changed in this run; the evening run rebuilds it.

## For the morning desk
1. Recompute attention with the tools (disclosures, volume ratio, gap, ARA/ARB, flow) and get the net-buy leaders for 10-23 from tools/flow.py.
2. AKRA is the cleanest liquid EARNINGS-CHANGE candidate. Read the segment split in the IDX FS (fuel vs JIIPE land).
3. Read DEWA's other-income note and DMAS's land-handover schedule before rating either.
4. Buyback names (AMMN, INDF, ICBP, BBRI) offer price support. A buyback is not an earnings change; rate it as a flow catalyst only.
5. Oil: check whether the Yanbu/Rabigh damage was confirmed overnight before rating any energy name.
6. Fed on Wednesday (early Thursday WIB): avoid sizing up into it; check the event-date rule for any ticket.
