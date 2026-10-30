# Pre-market intel — Thursday 2026-10-29 (IDX trading day)

Run: cloud night shift, 06:11 WIB (tools/clock.py: trading_day=true, before_open=true, last session 2026-10-28).
Paper holdings: none (desk/paper/portfolio.json: cash Rp150,000,000, no positions; desk/watchlist.json empty). intel/alerts.md: no change.

## Data access — read first
- `tools/idx.py`, `tools/prices.py` and `tools/flow.py` still return `unavailable`: the proxy refuses CONNECT to www.idx.id and query1.finance.yahoo.com (403, 2026-10-29 06:12 WIB). Tenth run in a row with this block.
- So there are **no tool-checked disclosures, OHLCV, volume ratio, gap, ARA/ARB or flow numbers** here. All figures come from news pages and search results.
- Refused or failed fetches: Bisnis (all pages, incl. "Pergerakan IHSG dan Rekomendasi Saham Hari Ini, Kamis 29 Oktober 2026" and the ASII/AUTO results pages), CNN (Fed live page, robots), periskop, investortrust (ASII page), EnergyNow. Their stories are **headline-only** unless another outlet is cited.

## Read first: ASII reported a profit DROP after rallying +8%
- **ASII 9M 2026: attributable net profit Rp21.60 tn, −11.73%** (Rp24.47 tn); revenue Rp243.8–243.9 tn, +0.1%; EPS Rp541 (Rp605); pre-tax profit Rp30.01 tn, −18.5%. Selling expenses +22.5% to Rp10.41 tn, G&A +10.3% to Rp16.94 tn, "other" swung to a Rp2.43 tn net expense (from +Rp1.84 tn income); JV/associate income +20% to Rp8.13 tn. Sources: Kontan, "Laba Bersih Astra (ASII) Anjlok 11,73% Menjadi Rp 21,6 Triliun per Kuartal III-2026", 19:24 WIB; CNBC Indonesia, "Laba Astra International (ASII) Rp21,6 Triliun di Kuartal III-2026", 17:47 WIB (says the FS was filed with BEI on 10-28).
- Segments (Kontan, "Penjualan Mobil Astra (ASII) Naik 13%, Laba Bisnis Otomotif Tembus Rp 9,8 Triliun", 18:48 WIB): **automotive +8% to Rp9.8 tn** (Astra car sales +13%, market +21% to 679k units, share 49%); **financial services +6% to Rp7.2 tn**; **mining solutions & heavy equipment −28% to Rp5.1 tn** (lower Martabe gold sales, weaker heavy-equipment demand on the national coal quota). Agribusiness and infrastructure not given.
- **Conflict (headline-only):** tirto ("Laba Bersih Astra International Kuartal III 2026 Tembus Rp24,6 T"), investortrust and Pikiran Rakyat headline Rp24.6 tn and "improving". CNBC gives profit for the period (incl. non-controlling interests) as Rp24.07 tn. Kontan and CNBC agree on Rp21.6 tn attributable, −11.73%; treat that as the figure.
- **Why it matters:** ASII closed **+7.99% at Rp5,000** on 10-28 on no results story and was the top LQ45 gainer (evening note). The release came after the move. The 8% pop looks like flow (foreign net buy Rp53 bn, below), not earnings. Expect a test of the move at the open.
- **EARNINGS-CHANGE pre-flag — ASII, down, low-medium.** Mechanism: opex growth and a Rp4.3 tn swing in other items against flat revenue; mining/heavy equipment −28%. Size: next-4-quarter attributable profit **−5% to −15%** vs the trailing four quarters, depending on Q4 (Q3-alone not available). Confidence: **low-medium** — "other" may hold one-offs (FX, fair value). Catalyst should read the FS notes.
- **UNTR read-across:** the ASII mining/heavy-equipment segment (mostly UNTR) fell 28% in 9M. This sits awkwardly with the "UNTR Q3 recovery" story in the 10-27 evening note; catalyst should reconcile (Q3-alone vs 9M). UNTR Rp430 dividend cum 11-05 is unchanged.

## Last IDX session (2026-10-28) — full-day flow
- IHSG **5,282.31, +0.31%**; intraday low **5,167.34** (Kontan 18:22 WIB). Benchmark since paper inception (5,328.36): **−0.86%**.
- **Full-day foreign flow: net BUY Rp664.24 bn** (Kontan, "Asing Kembali Masuk Bursa Saham RI, Cermati Saham Net Buy Terbesar, Rabu (28/10)", 22:50 WIB; also "Saat IHSG Rebound ke 5.282, Cermati Saham Net Sell Terbesar Asing, Rabu (28/10)", 22:56 WIB; investortrust 18:02 WIB agrees). **Conflict:** a periskop headline has "Asing Net Buy Rp257,26 Miliar Hari Ini" (headline-only; likely regular market only). Either way the first net-buy day in the desk's notes since setup. Session I was a net sell of Rp172 bn, so the afternoon brought ~Rp0.84 tn of net buying.

| Net buy (full day) | Rp bn | Net sell (full day) | Rp bn |
|---|---|---|---|
| **BBCA** | **1,170** | **TLKM** | **433.51** |
| **ENRG** | **300.25** | BMRI | 276.46 |
| BRMS | 114.6 | BBNI | 85.91 |
| ASII | 53.33 | AADI | 60.06 |
| GOTO | 49.19 | TPIA | 48.58 |
| DEWA | 43.73 | PTBA | 47.85 |
| BBRI | 43.66 | TINS | 32.88 |
| MBMA | 27.11 | ADRO | 29.41 |
| KLBF | 23.34 | BRIS | 27.55 |
| AMMN | 23.31 | INDF | 21.79 |

Source: Kontan, as above (22:50 and 22:56 WIB).
- **BBCA: Rp1.17 tn foreign net buy** (Rp491 bn in session I), closing **+7.65% at Rp5,275** (investortrust, "Investor Asing "Ngamuk" Borong Saham BBCA Rp 1,17 Triliun hingga Dorong Rebound IHSG", 18:02 WIB). **No catalyst is named by any outlet.** Analysts cite positioning before the **November MSCI rebalancing** (investor.id, Kontan 18:22). Unverified.
- **ENRG: Rp300 bn foreign net buy**, the second largest, on the day of its 9M results (below). Trimegah Sekuritas was also a buyer on 10-23 (CNBC Indonesia, "Trimegah Sekuritas Borong Saham Grup Bakrie (ENRG), Ada Apa?", 2026-10-23, headline-only) and Bakrie Kalila Investment bought 174.39 m shares (idnfinancials headline, date not read).
- **TLKM: Rp434 bn net sell**, the largest, a third day in the top-2 (10-27: Rp234 bn). BMRI top-2 net sell for a fifth day. State-bank selling continues; BBRI flipped to a small net buy.
- Coal names sold (AADI, PTBA, ADRO) on a day the mining/heavy-equipment segment at ASII reported −28%.

## Overnight global (US session 2026-10-28, closed 04:00 WIB 10-29)
| Driver | Move | IHSG read-across | Source / time |
|---|---|---|---|
| **FOMC** | **Hold at 3.75–4.00%, 10–2; Cook and Hammack dissented for a hike.** Statement: economy upgraded, inflation "remains elevated". Warsh: 2% is the overriding priority; last month's hike "marked the start of action"; offered little against a December hike. No dot plot. | **Hawkish hold.** CME FedWatch: **85% chance of a 25 bp hike in December.** Supports the dollar and US yields into year end: a headwind for the rupiah (record low 18,183) and SUN yields (10-yr 7.61%) | investingLive, "Recap: Fed holds at 3.75%-4% in 10-2 vote as Cook dissents for a hike, December move in focus", 2026-10-28 22:02 ET; Star-Advertiser/AP, "Wall Street rises as Fed holds rates steady, earnings in focus", 11:28 HST |
| S&P 500 | **7,743.97, +0.28%** (third up day) | mild risk-on; Fed outcome was priced | AP via Star-Advertiser, as above |
| Dow / Nasdaq | 52,475.10 +0.19% / 26,549.85 +0.27% | — | same |
| After hours | **Microsoft +4%+, Alphabet −7%+** | Nasdaq futures mixed; little direct IHSG link (GOTO/BUKA sentiment at most) | AP via Virginia Business, 16:31 ET |
| Brent | **~US$113.75, −0.1%** (Wednesday Asian high ~US$115.6 on an unconfirmed Houthi missile claim against Ras Tanura) | stays >US$100: supports ENRG, MEDC, ELSA, AKRA; a cost for importers and the fuel-subsidy bill | ABC News markets blog, 2026-10-29 07:15 AEDT; FinanceFeeds, "Brent Crude Oil Price: $115.59 on Fed Decision Day After Houthi Ras Tanura Claim" |
| Gold | **US$4,070/oz, +0.3%** | supports ANTM, MDKA, BRMS, EMAS, ARCI | ABC News, as above |
| Coal (Newcastle CFD) | **US$150/t, +0.17%** (10-27), near a 3-year high; LNG shock and Indonesian export curbs | supports coal revenue, but AADI/PTBA/ADRO were foreign-sold | Trading Economics, page updated 10-28 |
| Nickel (LME) | **~US$15,560/t, +0.15%** (10-28); oversupply narrative | flat for INCO, MBMA, NCKL | Trading Economics, 10-28 |
| CPO (FCPO) | **MYR 4,700, −0.02%** (10-28) after a near two-week low; record Malaysian stocks | neutral-to-soft for AALI, DSNG, LSIP | Trading Economics, "Palm Oil Bounces Back After Recent Losses", 10-28 |
| AUD | +0.5% to 70.57 US cents; ASX 200 futures +0.2% | the dollar did **not** rally on the hawkish hold overnight; regional FX may get a breather | ABC News, as above |
| Asia | Nikkei/Kospi open after this run (07:00 WIB) | check before the open | — |
| USD/IDR NDF | not found | — | — |

## Domestic market structure
- **ARKO (Arkora Hydro) suspended from session I on 10-28** for an unusual cumulative fall (−62.7% in a month, −77% YTD). BOARD flag. Source: investor.id, "Saham Anjlok 77% Kena Suspensi BEI", 2026-10-28 08:25 WIB. This is despite BEI's plan to replace stock suspensions with account freezes from November (Tempo, "BEI Rombak Pengawasan, Tak Lagi Suspensi Saham"; Ajaib, "BEI Rombak Aturan Suspensi dan UMA Saham Mulai November 2026").
- MSIN and BSWD suspended since 10-21; LUCY and VKTR on UMA (emitennews, "BEI Umumkan 2 Saham Suspensi & 2 Saham Masuk Daftar Pantau UMA", 2026-10-21 13:38 WIB). VKTR also hit ARB in session I on 10-28. BOARD flags.
- Broker views for today: Phintraco sideways **5,150–5,350**; BRI Danareksa support **5,118–5,182**, resistance 5,360–5,400, main trend still bearish; MNC a possible test of 5,116–5,180 then 5,456–5,564 (investor.id, "Prediksi IHSG dan Rekomendasi Saham Kamis, 29 Oktober 2026", 18:30 WIB; Kontan, "IHSG Menguat ke Level 5.282, Simak Proyeksi dan Rekomendasi Saham untuk Kamis (29/10)", 18:22 WIB). Picks without levels: BRPT, EMAS, JPFA, TINS (MNC); AADI, ANTM, DSNG (BRI Danareksa).

## Results released since the evening note (9M 2026 vs 9M 2025)

| Ticker | Revenue | Net profit | Read | Source |
|---|---|---|---|---|
| **ASII** | Rp243.8 tn, +0.1% | **Rp21.6 tn, −11.73%** | see top | Kontan 19:24; CNBC 17:47 WIB |
| **ENRG** | US$426.1 m, +17.9% | **US$72.81 m, +30.8%** (US$55.65 m) | Operating profit +44% to US$157.6 m, op. margin 37% (30%); oil ASP +33.1% to US$94.92/bbl, oil output +6% to 8,894 bopd; **gas output −13.8%** to 190.4 mmscfd, gas ASP +4.3%. Rp300 bn foreign net buy the same day | Kontan, "Energi Mega Persada (ENRG) Catat Laba Bersih US$ 72,81 Juta hingga September 2026", 21:30 WIB |
| **ARTO** | NII Rp2.30 tn, +29.6% | **Rp298.1 bn, +49.7%** (Rp199.1 bn) | Impairment up to Rp883 bn (Rp623 bn) | CNBC Indonesia, "Laba Bank Jago (ARTO) Naik 49,7% di Kuartal III-2026, Ini Faktornya", 11:06 WIB |
| **TOTL** | Rp3.51 tn, +26.1% | **+51.9%** (amount behind paywall) | contractor; small cap | Kontan, "Per September 2026, Laba Bersih TOTL Melonjak 51,9%", 09:11 WIB |
| AUTO | — | Rp1.8 tn | **headline-only** (Bisnis blocked); yoy not read | Bisnis, "Astra Otoparts (AUTO) Raup Laba Bersih Rp1,8 Triliun Kuartal III/2026" |
| BNGA | — | **Rp4.51 tn** | headline (yoy not read) | Kontan, "CIMB Niaga Catat Laba Bersih Rp 4,51 Triliun Pada September 2026" |
| ERAL | — | +55% | headline-only | Kontan insight headline |
| PGUN | — | "record" | headline-only (Haji Isam group) | Katadata databoks headline |
| BPFI | — | +88.79% | headline-only; small | Kontan headline |
| JECX | — | −37.6% | confirmed headline (Kontan) | Kontan headline |

- **ELSA conflict:** beritamoneter has +21.15% ("Elnusa (ELSA) Cetak Laba Bersih Rp681,55 Miliar per September 2026, Naik 21,15%"); IDX Channel and the evening note have +29%. Same profit figure, so the base differs; catalyst checks the FS.
- **Due:** GOTO Q3 (date not confirmed; Kontan 17:08 WIB preview: fintech the main driver, two-wheeler commission cut to 8% from 07-01 is a drag; Q2 adj. EBITDA Rp1.01 tn); BRIS is auditing its Q3 FS for the rights issue (StockWatch headline); BBRI ran a limited review (koridor headline). Deadline for unaudited Q3: 10-31.

## Attention scores (partial: no volume ratio, gap only where the press gives the close; disclosure = FS filed per press)

| Ticker | Score | Components | Note |
|---|---|---|---|
| **ASII** | **11** | 5 outlets + 3 FS filed 10-28 + 2 gap (+7.99%) + 1 flow top-20 | Results −11.7% after an 8% pop. EARNINGS-CHANGE pre-flag (down). Top of the list for the morning desk |
| **BBCA** | **8** | 5 outlets + 2 gap (+7.65%) + 1 flow (Rp1.17 tn) | No catalyst found; flow-driven |
| **ELSA** | 7 | 4 outlets + 3 FS | Pre-flag candidate (up) from the evening note; yoy conflict |
| **ENRG** | 6 | 2 outlets + 3 FS + 1 flow (Rp300 bn) | Pre-flag candidate (up) below |
| AALI | 6 | 2–3 outlets + 3 FS | Pre-flag (up, medium) from the evening note |
| ARTO | 4 | 1 + 3 FS | +49.7% on a small base |
| AUTO | 4 | 1 + 3 FS | headline-only |
| BREN | 4+ | 1 + 2 gap (−6.94% session I) + 1 ARB | second day at ARB; close unknown |
| TLKM | 3+ | 2 outlets + 1 flow (−Rp434 bn) | gap unknown |
| BRMS | 2+ | 1 + 1 flow (Rp115 bn) | — |
| ISAT, BRPT | 3 | 1 + 2 gap (−6.8%) | BRPT is an MNC pick today |
| ARKO | — | suspended | BOARD flag, no ticket |

### EARNINGS-CHANGE pre-flags (night shift, for catalyst to confirm)
- **ASII — down, low-medium** (above).
- **ENRG — candidate, up, medium-low.** Mechanism: oil ASP +33% with Brent still ~US$114 holds the 9M margin; gas volume decline is the offset. Size: next-4-quarter net profit **+10% to +25%** vs trailing if Brent stays above US$100. Confidence: medium-low (the gas decline, commodity risk, and USD reporting vs rupiah record low).
- **ARTO — candidate, up, low.** +50% on rising impairments; valuation is the question, not the growth.
- AALI (up, medium), ELSA (up, medium-low), LTLS (up, low), ANTM (up), UNTR (up — now **in question** given the ASII segment −28%), HMSP, MAPI, SIDO: unchanged from the 10-28 notes.

### CORP-ACTION
- Nothing new overnight. Unchanged: PRDA split cutoff **today 10-29**; VISI private-placement listing **today 10-29**; TSPC cum 10-30; ASII Rp98 pays 10-30; SIDO cum 11-02; WIFI RUPSLB and HSC exclusion 11-02 (BREN also leaves IHSG 11-02); UNTR Rp430 cum 11-05; BRIS rights-issue RUPSLB 11-06; DOOH 11-09; PACK 11-30. See intel/calendar.json.

## For the morning desk (2026-10-29)
1. **ASII:** +8% on 10-28, then 9M attributable profit −11.7% filed the same evening. Read the FS (Q3 alone, the Rp2.43 tn "other" line) before rating it; it is the highest-attention name today.
2. **Fed was a hawkish hold** (2 dissents for a hike; 85% December hike priced). The dollar did not rally overnight (AUD +0.5%), but the rupiah sits at a record low and SUN yields are rising: keep bank tickets other than flow leaders on a short leash.
3. **Foreign flow turned to a net buy (Rp664 bn) on BBCA alone (Rp1.17 tn).** Run tools/flow.py to confirm and check whether it persists; positioning before the November MSCI review is the only explanation offered.
4. **ENRG:** results +31% and a Rp300 bn foreign buy on the same day; Bakrie-group stock, check liquidity and board status before any ticket.
5. **UNTR:** reconcile the "Q3 recovery" with ASII's −28% mining/heavy-equipment segment; any ticket from today holds through the 11-05 cum date.
6. Check closes and ARB status for BREN, PTRO, RATU, JARR, TEBE, VKTR, SOSS (prices were session I only) and ARKO (suspended).
7. Asian opens (Nikkei, Kospi) and Alphabet's −7% after hours: check before 09:00 WIB.
