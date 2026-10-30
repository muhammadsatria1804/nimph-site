# Pre-market intel — Wednesday 2026-10-28 (IDX trading day)

Run: cloud night shift, 06:11 WIB (tools/clock.py: trading_day=true, before_open=true, last session 2026-10-27).
Paper holdings: none (desk/paper/portfolio.json: cash Rp150,000,000, no positions; desk/watchlist.json empty). intel/alerts.md: no change.

## Data access — read first
- `tools/prices.py`, `tools/idx.py` and `tools/flow.py` still return `unavailable`: the proxy refuses CONNECT to www.idx.id and query1.finance.yahoo.com (403, 2026-10-28 06:12 WIB). Eighth run in a row with this block.
- So there are **no tool-checked disclosures, OHLCV, volume ratio, gap, ARA/ARB or flow numbers** here. All figures come from news pages and search results.
- Refused or failed fetches: Bisnis (morning outlook), Kontan net-buy page, CNBC oil, Detroit News, Fortune, mediakompeten, mediakampung, periskop. Their stories are **headline-only** unless another outlet is cited.

## Last IDX session (2026-10-27) — flow update
- IHSG 5,266.13, −1.99%; intraday low 5,182 (evening note; investor.id 18:30 WIB agrees).
- **Full-day foreign net sell: about Rp0.65–0.69 tn, all markets** — much smaller than the intraday headlines suggested.
  - Kontan, "IHSG Ambruk 1,99% ke 5.266, Cermati Saham Net Sell Terbesar Asing, Selasa (27/10)", 20:10 WIB: **Rp668.26 bn**.
  - investor.id, "Tiga Raksasa Bursa Terempas, Asing Belum juga Puas", 20:01 WIB: Rp651.2 bn; **YTD net sell Rp97.3 tn**.
  - periskop headline: "Asing Jual Bersih Sekitar Rp688,16 Miliar Hari Ini, BMRI Paling Banyak Dilepas" (headline-only).
  - **Conflict:** Kompas's 15:38 WIB headline had "Asing Cabut Rp 2,24 Triliun" (headline-only). Three later full-day sources agree on ~Rp0.65–0.69 tn, so the Kompas figure was probably wrong or included negotiated trades that later reversed. **Check with tools/flow.py.**
- So the "third day ≥ Rp1.85 tn" from the evening note did **not** happen. Foreign selling slowed sharply while the index fell 2%: the late-day fall was mostly domestic selling, led by the conglomerate stocks.

| Net sell (full day, all markets) | Rp bn | Close (investor.id) |
|---|---|---|
| BMRI | 266.31 | 3,870 (−1.0%) |
| TLKM | 234.45 | **2,140 (−4.89%)** |
| BBNI | 119.57 | 3,310 (−4.6%) |
| BRIS | 80.97 | — |
| BBCA | 59.75 | — |
| PGAS | 48.85 | — |
| DSSA | 34.60 | — |
| ANTM | 32.58 | 2,770 (investor.id 05:45 WIB) |
| ITMG | 31.64 | — |
| TPIA | 30.83 | — |

Source: Kontan, 20:10 WIB (top 10); closes from investor.id 20:01 WIB. **Net buy:** CPIN Rp60.6 bn, the largest, which investor.id calls "relatively insignificant"; the full net-buy list was not read (Kontan, "IHSG Turun 2 Hari Beruntun, Cek Saham yang Banyak Diborong Asing", is headline-only).
- BRIS stayed a net sell all day (Rp81 bn; Monday it was a net buy). **PGAS** was in the top-10 net sell on the day of the Singapore gas story (below).
- Rupiah closed at **18,156 per US$, −0.12%** (investor.id, "Rupiah Tenggelam Makin Dalam", 15:29 WIB). Kontan's headline calls it the weakest since June ("Rupiah Ditutup Turun ke Rp 18.156 Per Dolar AS Hari Ini (27/10), Terlemah Sejak Juni"; headline-only).

## Overnight global (US session 2026-10-27, closed ~04:00 WIB 2026-10-28)
| Driver | Move | IHSG read-across | Source / time |
|---|---|---|---|
| S&P 500 | **7,722.60, +0.60%** | second risk-on day before the Fed | TheStreet, "Stock Market Today (Oct. 27, 2026): Nasdaq and Russell 2000 gain as Anthropic lifts tech sector", 16:19 EDT wrap |
| Nasdaq / Dow / Russell 2000 | 26,477.81, +1.18% / 52,377.57, +0.03% / 2,818.87, +1.16% | chips and AI led again. Small-cap strength is a mild risk-on sign; the local tech names (DCII, WIFI) fell anyway on 10-27 | same |
| Asia, 2026-10-27 | Nikkei +1.78%, Kospi +3.09% (at ~15:09 WIB) | IHSG was the region's outlier on 10-27; the fall was local | Katadata via the evening note; closes not found |
| Brent | **about US$113.7–113.8, −1.8 to −1.9%** (intraday; settlement not found). WTI about **US$99.8–100.0**, below US$100 | The four-party Iran talks (Saudi Arabia, Turkey, Pakistan, Iran) agreed to keep talking; Iran's Security Council chief briefed the Supreme Leader. Houthi strikes on Saudi Arabia continued (a claimed missile strike on Ras Tanura refinery), limiting the fall. UBS raised its year-end Brent view to ~US$110. Mild relief for the rupiah and fuel-subsidy worries; a negative tick for MEDC, ENRG, AKRA margins | Reuters via Euronext, "Oil falls $2 as Middle East talks help ease supply worries", 13:44 EDT; Industry.co.id, "Harga BBM Hari Ini 28 Oktober 2026: Brent Turun ke US$113,84 dan WTI ke US$100,02...", 00:58 WIB |
| Gold | about **US$4,027, −0.3%** (early US session) | flat for ANTM, MDKA, BRMS, EMAS | TheStreet, as above |
| 10-yr UST | 4.986%, unchanged (15:47 EDT) | — | TheStreet |
| Coal / CPO / nickel / tin (10-26 close) | Newcastle Nov US$153.60, −0.9%; CPO MYR 4,789, −0.6%; LME nickel US$15,561, −1.81%; tin US$51,017, +0.99% | slightly negative for coal, CPO and nickel names; 10-27 closes not found | kumparan, "Harga Komoditas: Minyak Mentah Merosot 1,5 Persen, Timah Naik 1 Persen", 2026-10-27 10:05 WIB |
| USD/IDR | **18,156** (10-27 close) | weakest since June per Kontan; still the main domestic headwind | investor.id 15:29 WIB |
| Fed | FOMC began Tuesday; **decision Wednesday US time = early Thursday 2026-10-29 WIB**, then Chair Warsh's press conference. The market is watching for hints of further hikes | foreign flow risk through Thursday | TheStreet; investor.id 15:29 WIB (Ibrahim Assuaibi, Traze Andalan Futures) |
| US big tech | Microsoft and Alphabet report Wednesday after the US close (Thursday morning WIB); Amazon and Apple later | read-across for data-centre names (DCII, DMAS, TLKM's data-centre unit) | TheStreet |
| Macro, Indonesia | **Fitch expects Indonesian growth below 5% in H2 2026**, 5.2% for the full year, versus the government's 5.4% target, as fiscal support fades and consumption slows | negative for consumer and bank sentiment | investor.id, "IHSG Terancam Turun Lagi, 5 Saham Layak Dicermati", 05:56 WIB |

Morning read: Wall Street is up for a second day and oil is about US$2 lower, so the backdrop is better than Tuesday's. The full-day foreign net sell was only ~Rp0.67 tn, which suggests the late collapse to 5,182 was local forced selling, not a fresh foreign exit. Against that: the rupiah is at its weakest since June, the Fitch growth cut, and the Fed decision lands before Thursday's open.

### Analysts' IHSG range for 2026-10-28
- Phintraco: support **5,180**, pivot 5,300, resistance 5,350. A close below 5,180 opens **5,100–5,000**. MACD histogram widening on the negative side; Stochastic RSI may form a death cross. Picks include **UNTR** (the other four not in the article text) (investor.id, 05:56 WIB; investor.id, "Prediksi IHSG dan Rekomendasi Saham Rabu, 28 Oktober 2026", 2026-10-27 18:30 WIB).
- MNC Sekuritas: a limited pullback to **5,116–5,180** before a rebound to 5,456–5,564. Picks: ADRO, BUVA, ERAA, VKTR; no levels in the text (investor.id, 18:30 WIB).
- Kontan headlines (headline-only): "IHSG Melemah 1,99%, Simak Proyeksi dan Rekomendasi Saham untuk Rabu (28/10)"; "IHSG Anjlok 1,99% ke 5.266, Ini Prediksi dan Rekomendasi Saham untuk Rabu (28/10)".
- Broker picks are opinions, not stories; low weight in attention.

## Market structure
- **MSIN (MNC Digital Entertainment, Hary Tanoesoedibjo's group) suspended from session I on 2026-10-27** after an "unusual" cumulative price **fall** (−47.5% in a month, ~−75% YTD per Stockbit). Source: investor.id, "Saham Emiten Hary Tanoe Kena Suspensi BEI", 2026-10-27 08:01 WIB; idnfinancials, "Demi lindungi investor, BEI suspensi saham Hary Tanoe". **BOARD flag: suspended.** BEI is still suspending single stocks until its new account-level regime starts in early November.
- **Indonesia–Singapore:** the foreign ministers (Arrmanatha Nasir and Vivian Balakrishnan) met in Jakarta on 10-27, one-on-one and closed-door, with a joint press statement; no outcome reported. SKK Migas (Djoko Siswanto) confirmed the cut from 10-24: 15 BBtud from Natuna and 16 BBtud from Sumatra. Luhut Binsar Pandjaitan (DEN): "Why would we even fight with Singapore? There is no reason to." Source: ANTARA English, "Indonesia, Singapore FMs meet amid gas export adjustments", 2026-10-27 17:03 WIB. A headline (headtopics, headline-only) says the two countries set up a **task force to trace the finances of forest burners**, which could put plantation names under scrutiny; no companies named. Tone is de-escalating; no market-moving outcome yet.
- HSC exclusion from IHSG on **2026-11-02** and the MSCI consultation are unchanged. **DSSA and MORA are out of the top 10 by market cap**; DNET entered at #10 (Rp138 tn) (investor.id, "Satu Lagi Saham Emiten Grup Sinar Mas Terlempar", 05:15 WIB).

## Issuer stories (24 h), attention (partial)
Outlets only (capped at 5), plus "+1 flow" where the stock is in Kontan's full-day top-10 net sell or is the top net buy (the published list is top 10, not top 20, so others may also qualify). Not computed: disclosure +3, volume ratio, gap, ARA/ARB. The morning desk adds these with the tools.

| Ticker | Partial score | Story | Status |
|---|---|---|---|
| **ANTM** | 2 (investor.id, Emitennews) + 1 flow = **3**; **+3 more if the IDX disclosure is confirmed** (Emitennews says the figures come from an IDX disclosure) | **9M 2026: attributable net profit Rp8.83 tn, +48% (Rp5.97 tn); net sales Rp88.48 tn, +23%; EBITDA Rp13.48 tn, +45%; EPS Rp367.78 vs Rp248.62.** Gold 77% of sales (Rp68.41 tn, +17%); nickel Rp16.98 tn, +52%; bauxite/alumina Rp2.64 tn, +35%. Gross profit +42%, operating profit +53%. Trailing P/E 6.61x (Stockbit). Close Rp2,770, −14.2% in a month. **Conflict:** Emitennews prints total sales Rp83.86 tn and total profit for the period Rp9.66 tn (+46%); the investor.id figures are attributable profit and net sales — check the FS | Read in full: investor.id, "Laba Antam (ANTM) Loncat, Saham Lagi Murah-murahnya", 05:45 WIB; Emitennews, "Laba Bersih ANTAM Naik 46% Rp9,66 T di 9M26, Ini Penunjangnya", 2026-10-28. No Q3-alone figure |
| **TLKM** | 2 (investor.id, Kontan) + 1 flow = **3** | **−4.89% to 2,140** on 10-27 with a Rp234 bn foreign net sell; the biggest index drag. Q3 results not yet out (the deadline is 10-31) | data only; results due this week |
| **BMRI** | 2 + 1 flow = **3** | Largest foreign net sell for a third day (Rp266 bn), close 3,870 (−1.0%); −24.5% YTD (investor.id 13:24 WIB) | no new story |
| **BBNI** | 2 + 1 flow = **3** | −4.6% to 3,310 with a Rp120 bn foreign net sell, a day after in-line 9M results (+7%) | no new story |
| **PGAS** | 1 + 1 flow = **2** | Foreign net sell Rp48.9 bn while the Singapore gas export cut is in the news. **Desk inference, not from an article:** PGAS's link to the Singapore pipeline contracts is unverified; volume is small (31 BBtud) | check exposure |
| **BRIS** | 1 + 1 flow = **2** | Foreign net sell Rp81 bn. A mediakampung headline (headline-only): "BSI Siapkan Buyback Saham Rp 500 Miliar Mulai 27 Oktober 2026". A buyback a week before the rights-issue RUPSLB (11-06) needs the primary disclosure | **headline-only**; tools/idx.py disclosures --ticker BRIS |
| **RATU** | 1 (Suara) = **1** | 9M 2026: revenue US$40.31 m, +7.2%; **attributable net profit US$25.09 m, +113%**; EPS US$0.0092 vs 0.0043 (Suara, "Laba Per Saham Naik, Emiten RATU Layak Dilirik?", 2026-10-27 21:19 WIB, from the interim FS). The article mislabels the comparison period. Was near ARB (−6.83%) on 10-27 with the Hapsoro group | read in full; see pre-flags |
| **CPIN** | 0 + 1 flow = **1** | Largest foreign net buy (Rp60.6 bn) and an LQ45 gainer (+2.58%) on 10-27 | no story |
| **UNTR** | (from the evening note) | Phintraco pick for 10-28 after the Q3 recovery and +6% on 10-27 | carries over |
| **BNGA** | — | CIMB Group denied a delisting rumour (Bisnis, 2026-10-22); the stock jumped 16–19% on the rumour (InvestorTrust). periskop, "CIMB Niaga (BNGA): Belum Ada Keputusan Formal Perubahan Kepemilikan Saham", 10-27 — the bank's reply to a BEI query | **headline-only** (fetch failed). A take-private would be a CORP-ACTION; nothing formal |
| **MSIN** | — | Suspended (see Market structure) | BOARD flag |
| ALII | — | Answered a BEI query: the controller and affiliates have been buying shares (StockWatch, "Jawab BEI, Ancara Logistics (ALII) Sebut Pengendali dan Afiliasi Borong Saham") | **headline-only** |
| Andira Agro (ANDI) | — | "Puncak Jaya Sejahtera Ambil Alih 33 Persen Saham Andira Agro" (mediakompeten) | **headline-only**; check for a tender offer |

### EARNINGS-CHANGE pre-flags (night shift, for catalyst to confirm)
- **ANTM — pre-flag, up, medium.** Mechanism: 9M attributable profit +48%, on gold sales +17% and nickel +52%, and the gold price is still about US$4,000+. If Q4 holds near the 9M run-rate, next-4-quarter profit stays ≥ 10% above the trailing 4 quarters. Size: **+15% to +35%** versus trailing. Confidence: **medium** (gold above US$4,000 is the main driver and could reverse; the revenue figures from the two sources disagree, and no Q3-alone number is available). Foreign investors still net sold it (Rp32.6 bn).
- **RATU — candidate, up, low.** Profit doubled on revenue +7%, so the jump is likely below the operating line or a one-off; small revenue base. No flag until the FS is read.
- **UNTR (up), HMSP (up, low), MAPI (up, candidate), SIDO (down):** unchanged from the 10-27 evening note.
- BBCA, BBNI: no flag. AKRA, BMRI, DMAS, DEWA, UNVR, BUKA, ADHI, PTPP: unchanged from the 10-26 notes.

### CORP-ACTION (dates inside a ticket opened today; news-sourced, unverified)
- **DMAS: cum date today, 10-28** (interim dividend about Rp1.4 tn; InvestorTrust puts the yield at ~16%). KSEI has a "DMAS_DIV_20261030" file, which fits a recording date of 10-30. Expect an ex-date price drop of about the dividend on 10-29. AXIO is also cum 10-28.
- SIDO cum 11-02 (two sources and the latest say 11-02; one says 10-28); TSPC cum 10-30; VISI private-placement listing 10-29; PRDA split cutoff 10-29; WIFI RUPSLB and the HSC exclusion 11-02; BRIS RUPSLB 11-06 (and a possible Rp500 bn buyback, headline-only); DOOH RUPSLB 11-09; PACK RUPSLB 11-30. See intel/calendar.json.
- BYAN: the Jhonlin Baratama (Haji Isam) acquisition of 30.25% at Rp2,588/sh closed on 2026-10-08 (Kontan, Bisnis). It is not new, despite feeds re-running it on 10-27.

## For the morning desk (2026-10-28)
1. Run tools/flow.py for 10-27. The press has a full-day net sell of **~Rp0.67 tn**, against the Kompas intraday headline of Rp2.24 tn; settle which figure is right before using "foreign selling" in any thesis.
2. **ANTM**: read the 9M FS (attributable vs total profit; net sales Rp88.48 tn vs Rp83.86 tn; Q3 alone). It is the only large cap with a fresh ≥ 10% earnings story this morning, at a 6.6x trailing P/E.
3. Check 10-27 closes and ARB status for the conglomerate stocks (BREN, PTRO, DSSA, MORA, CUAN, RATU, BUVA, RAJA, AMMN, BRMS) and TLKM's −4.89%. A bounce off 5,182 into a close of 5,266 is not yet a confirmed low; Phintraco's line is 5,180.
4. FOMC decision and Microsoft/Alphabet results land before Thursday's open: any ticket opened today carries that event.
5. BRIS: confirm whether the Rp500 bn buyback headline is real (tools/idx.py disclosures --ticker BRIS) and how it fits the 11-06 rights-issue RUPSLB.
6. MSIN is suspended: BOARD flag, no ticket.
7. Board checks from the 10-26 notes (GRPM, SOFA, MGLV, BNLI) are still open.
