# Pre-market intel — Tuesday 2026-10-27 (IDX trading day)

Run: cloud night shift, 06:11 WIB (tools/clock.py: trading_day=true, before_open=true, last session 2026-10-26).
Paper holdings: none (desk/paper/portfolio.json, cash Rp150,000,000; desk/watchlist.json empty). intel/alerts.md: no change.

## Data access — read first
- `tools/prices.py`, `tools/idx.py` and `tools/flow.py` still return `unavailable`: the proxy refuses CONNECT to www.idx.id and query1.finance.yahoo.com (403, 2026-10-27 06:12 WIB). Sixth run in a row with this block.
- So there are **no tool-checked disclosures, OHLCV, volume ratio, gap, ARA/ARB or tools/flow.py numbers** here. All figures come from news pages and search results.
- Kontan (investasi, pusatdata, industri; keuangan.kontan.co.id worked), Bisnis (rupiah page), demokratis.co.id and mediakompeten refused the fetch: their stories are **headline-only**.

## Last IDX session (2026-10-26) — flow update
- IHSG 5,373.09, −1.22%; value about Rp14.7 tn; breadth 174/542/247 (evening note; investor.id agrees).
- **Full-day net foreign sell: Rp1.85 tn** (InvestorTrust, "Net Sell Kembali Jumbo Rp 1,85 Triliun, Saham Bank Dipimpin BMRI Dilepas Pemodal Asing", 2026-10-26 18:40 WIB; investor.id, "Lima Raksasa Bursa di Tengah Prahara, BMRI Melawan", 2026-10-27 05:45 WIB; Kontan pusatdata headline, headline-only). Kontan keuangan ("Asing Net Sell Rp 2,03 Triliun di Awal Pekan Ini, BMRI Paling Banyak Dilepas", 17:41 WIB) has **Rp2.03 tn**, probably all markets incl. negotiated; the regular-market figure is likely Rp1.85 tn. **YTD net sell Rp96.7 tn** (investor.id).
- This closes the evening note's gap (it had session I only, Rp1.14 tn).

| Net sell (full day) | Rp bn | Close | Net buy (full day) | Rp bn |
|---|---|---|---|---|
| BMRI | 400.03 | 3,910 (+0.2%) | NATO | 80.39 (InvestorTrust only) |
| TLKM | 329.39 | 2,250 (+0.45%) | BRIS | 40.80 (investor.id calls it the largest net buy) |
| BBCA | 235.53 | 4,940 (−1.69%) | CASA | 35.10 |
| BBRI | 150.25 | 2,910 (0%) | BRMS | 31.14 |
| ANTM | 107.31 | 2,760 (−3.5%) | BRPT | 16.73 |
| BBNI | 42.55 (Kontan) | — | | |

Sources: InvestorTrust 18:40 WIB and investor.id 05:45 WIB as above; closes from investor.id. NATO's Rp80 bn net buy appears only in InvestorTrust and is not explained (investor.id lists BRIS first), so it may be a negotiated-market cross: **check with tools/flow.py**.
- Read: BMRI and TLKM absorbed heavy foreign selling and still closed green, so domestic buyers are defending them. BBCA (results today) and ANTM did not hold.

## Overnight global (US session 2026-10-26, closed ~04:00 WIB 2026-10-27)
| Driver | Move | IHSG read-across | Source / time |
|---|---|---|---|
| S&P 500 | **7,676.80, +0.70%** | risk-on start to Fed week; recovers last week's loss | TheStreet, "Stock Market Today (Oct. 26, 2026): Nasdaq, S&P 500 jump after Anthropic IPO announcement"; AP via KSAT, 2026-10-26 |
| Nasdaq / Dow | 26,169.38, +0.82% / 52,361.52, +0.28% | AI and chips led (Nvidia +2.4%) on Anthropic's Nasdaq IPO filing. Mild positive for tech/data-centre names (DCII, DMAS land to data centres), not a direct driver | same |
| Europe | CAC 40 +0.8%, others up | — | AP via KSAT |
| Brazil | Bovespa about −14% after Lula's re-election | EM-fund headline; a fresh EM risk event during Indonesia's MSCI consultation. Possible extra EM-fund redemptions | AP via KSAT |
| Asia, 2026-10-26 | Nikkei 62,189.65, −0.80%; TOPIX +0.18%; Shanghai 3,697.52, +0.19%; Hang Seng 23,211.81, +0.51% | mixed; IHSG was the region's weak spot (−1.22%) | Armenpress, "Asian Stocks - 26-10-26" |
| Brent | **settled US$115.81, −0.8%**; WTI US$101.76, −1.46%. Intraday low about US$114.5 | Talks: Qatari mediators in Tehran in coordination with the US; Saudi, Turkish and Pakistani officials met Iran. The Houthis claim strikes on East-West pipeline pumping stations and Riyadh airport; **Saudi has not confirmed damage**. Oil names (MEDC, ENRG) are headline-driven both ways; the rupiah and the fuel subsidy stay under pressure | Reuters via Investing.com, "Oil settles lower on peace hopes, Saudi attacks limit losses", 2026-10-26. AP prints "Brent US$110.74, −0.9%", which does not match its own change; use Reuters |
| Gold | about **US$4,013–4,025, +0.4%**; back above US$4,000 | small relief for ANTM, MDKA, BRMS, EMAS after Monday's ANTM −3.5%. BRMS was a foreign net buy | Babypips, "Financial & Forex Market Recap: Oct. 26, 2026"; TheStreet (early quote) |
| Copper | LME US$14,323/t, +0.96% (tight Chinese supply) | + AMMN, MDKA, BUMI's new copper-gold asset | SP Angel via Share-Talk, "Today's Market View, Monday 26th October 2026" |
| Nickel | LME US$15,848/t (−0.45% vs 15,920; kumparan has −1.69%) | slightly negative for INCO, NCKL, MBMA (MBMA was an LQ45 loser, −5.85%) | SP Angel, as above; kumparan, "Harga Komoditas: CPO dan Timah Menguat, Batu Bara-Nikel Melemah", 2026-10-26 08:15 WIB |
| Coal | Newcastle 150.70, −0.30% (10-23); Australia FOB swap US$155.0, +0.65% (10-26) | neutral to slightly positive for PTBA, AADI, ITMG, HRUM | kumparan, as above; SP Angel, as above |
| CPO | **MYR 4,818/t, +0.54%** (close of 10-23) | slightly positive for AALI, LSIP, TAPG | kumparan, as above. Monday's close not found |
| Tin | LME US$50,517/t (+0.85% kumparan, 10-23) | TINS neutral | same |
| USD/IDR | **18,127, −0.2%** on 10-26 (InvestorTrust has 18,177) | the weak rupiah plus Brent above US$115 is the main domestic headwind cited for Monday's fall | investor.id, "Prediksi IHSG dan Rekomendasi Saham Selasa, 27 Oktober 2026", 2026-10-26 18:30 WIB |
| US 10-yr / 2-yr / DXY | 4.98% (−0.4 bp) / 4.71% (+3 bp) / 102.0 (+0.2%) | firm dollar keeps EM-flow pressure on | TheStreet (15:10 EDT); Babypips |
| Fed | FOMC Tue–Wed; decision early **Thursday 2026-10-29 WIB**. Hold priced near 90%; the market implies ~10% chance of a hike at this meeting. AP describes September's move as "its recent first rate hike in three years". Chair Warsh's press conference is the risk | foreign outflow risk persists through Thursday | Babypips; TheStreet (Capital.com's Kyle Rodda); AP via KSAT |
| US big-tech results | Alphabet, Microsoft Wed; Amazon Thu (capex guidance) | read-across for data-centre names | AP via KSAT |

Morning read: a positive Wall Street and slightly softer oil give IHSG room to stabilise after Monday's −1.22%, but foreign selling (Rp1.85 tn, mostly banks and TLKM) did not ease, the rupiah is at 18,100+, and the Fed decision comes Thursday morning WIB. BBCA reports today.

### Analysts' IHSG range for 2026-10-27
- Phintraco: **sideways 5,280–5,450**; below 5,400 but above MA5, MACD histogram negative but narrowing (investor.id, 18:30 WIB, as above).
- MNC Sekuritas: correction could extend to **5,181–5,325**; rebound resistance 5,460–5,651. Picks: DOOH, MBMA, MINA, TLKM, XPFT (no levels given) (investor.id, as above).
- Kontan headlines (headline-only): "IHSG Diprediksi Melemah Hari Ini (27/10)"; "IHSG Diprediksi Sideways, Cermati Saham AADI, BBNI, dan TLKM"; "Simak Rekomendasi Saham AMRT, UNTR, dan UNVR untuk Perdagangan Selasa (27/10)".
- Broker picks are opinions, not stories; low weight in attention.

## Market structure
- **BEI ends stock-wide suspensions and issuer-wide UMA from early November 2026**; it will suspend the specific accounts suspected of manipulation, announce investigations and examine the brokers involved. Coordinated with OJK. Jeffrey Hendrik, BEI President Director, at the BEI press conference. Source: ANTARA, "BEI siap berlakukan suspensi ke rekening terindikasi manipulasi harga", 2026-10-26 16:28 WIB (confirms the evening note's Suara and InvestorTrust reports; still no primary BEI document read). The proposal in the evening note stands: an investigation notice naming a stock should become a BOARD flag.
- HSC exclusion from IHSG on **2026-11-02** (82 stocks) and the MSCI Standalone consultation (decision by 2027-06-30) are unchanged; see the 10-26 pre-market note.

## Issuer stories (24 h), attention (partial)
Outlets only, capped at 5; "+1 flow" where the stock was in the full-day top-5 foreign net buy or sell (the press list is top 5, not top 20, so others may also qualify). Not computed: disclosure +3, volume ratio, gap, ARA/ARB. The morning desk adds these with the tools.

| Ticker | Partial score | Story | Status |
|---|---|---|---|
| **BBCA** | 2 + 1 flow = **3** | **Q3/9M 2026 results expected today, 10-27** (Kontan schedule, 10-26). −1.69% to 4,940 on 10-26, foreign net sell Rp235.5 bn; Warta Ekonomi says the stock is down almost 39% YTD ("Saham BCA Jadi Pemberat IHSG, Sahamnya Sudah Anjlok Hampir 39% Tahun Ini"; headline-only). Earlier: 7M 2026 profit +5%, NIM recovering (Pasardana, 2026-08-19) | Results not out by 06:14 WIB. **EARNINGS-CHANGE watch**: if 9M profit growth is far from the ~5% run-rate, catalyst should size it |
| **BMRI** | 2 + 1 flow = **3** | Largest foreign net sell (Rp400 bn) but closed +0.2% at 3,910. 9M profit Rp45.5 tn, +20.7% (InvestorTalk, "Laba Bank Mandiri Kuartal III 2026 Tembus Rp45,5 Triliun, Naik 20,7%"; headline-only); the consolidated vs bank-only question from the evening note is still open | headline-only |
| **TLKM** | 2 + 1 flow = **3** | Foreign net sell Rp329 bn but closed +0.45% at 2,250; MNC and Kontan picks today | no new story |
| **BUMI** | 3 (rmol, Kontan, IDX Channel) = **3** | **Closed the acquisition of 100% of Mount Margaret Mining Pty Ltd** (Queensland; copper-gold; ~13 Mt ore at 0.78% Cu and 0.24 g/t Au; 3,412 ha) for **US$22 m (~Rp394 bn)** via Bumi Resources Australia, completed 2026-10-23, per BUMI's disclosure signed by director R.A. Sri Dharmayanti. Funding not stated. Stock Rp140 (unchanged at 09:31 WIB on 10-26), −61.75% YTD | Read in full: rmol, "BUMI Akuisisi Tambang Australia Rp394 Miliar, Saham Bertahan di Rp140", 2026-10-26 10:01 WIB. Small versus BUMI's size: **no EARNINGS-CHANGE** |
| **ANTM** | 1 + 1 flow = **2** | −3.5% to 2,760, foreign net sell Rp107 bn. Gold back above US$4,000 overnight (+0.4%) | data only |
| **PACK** | 2 (IDX Channel, Kontan) = **2** | Multi-day rally ahead of the Rp8.2 tn rights issue (RUPSLB 11-30; dilution up to ~74.6%). IDX Channel 10-26 10:52 WIB; Kontan, "Segera Right Issue Dana Rp8,2 Triliun, Intip Profil Emiten PACK dan Kinerja Terbaru" (headline-only). **CORP-ACTION** stands; a rally into a heavy-dilution rights issue is a bear point | headline-only |
| **ADHI** | 1 (Kontan) = **1** | "Laba Bersih ADHI Melonjak 247%, Saat Pendapatan Turun 4,96% di Kuartal III-2026" | **headline-only** (Kontan refused). Profit up on lower revenue: in 9M 2024 a similar jump came from joint-venture income (IDX Channel, 2024-10-15), so read the FS for the source before any pre-flag |
| **PTPP** | 1 (Kontan) = **1** | "Laba PT PP (PTPP) Naik Meski Pendapatan Turun per Kuartal III 2026" (the evening note had ~46× from Bisnis) | **headline-only** |
| BRIS | 0 + 1 flow = **1** | Foreign net buy Rp40.8 bn; rights issue RUPSLB 11-06 | no new story |
| NATO, CASA, BRMS, BRPT | 0 + 1 flow = **1** | Top-5 foreign net buys; no story found | check tools/flow.py (NATO above) |
| BUMN Karya (ADHI, PTPP, WIKA, WSKT) | — | Merger talk for the end of 2026 (Kontan, 10-26; headline-only) plus ADHI and PTPP profit jumps on falling revenue | theme to watch |
| ULTJ, WSBP, PTBA | — | IDX Channel "Populer" titles: ULTJ postponed an RUPSLB on an acquisition; WSBP debt conversion and private placement approved; PTBA still reviewing a buyback | **headline-only**, no dates; the morning desk can check with tools/idx.py disclosures |

### EARNINGS-CHANGE pre-flags (night shift, for catalyst to confirm)
- **BBCA**: watch today's release (see table).
- **ADHI, PTPP**: profit up sharply on lower revenue; likely non-operating. **No flag** until the FS is read.
- AKRA, BMRI, DMAS, DEWA, UNVR, BUKA: unchanged from the 10-26 notes.

### CORP-ACTION (dates inside a ticket opened today; news-sourced, unverified)
- **SCMA cum date is today, 10-27** (Rp8.4/sh; ex 10-28).
- DMAS and AXIO cum 10-28; VISI private-placement listing 10-29; WIFI RUPSLB and SIDO cum date 11-02; BRIS RUPSLB 11-06; DOOH RUPSLB 11-09 (unverified; DOOH is also an MNC pick today); PACK RUPSLB 11-30. See intel/calendar.json.

## For the morning desk (2026-10-27)
1. Run tools/flow.py for 10-26: confirm the Rp1.85 tn vs Rp2.03 tn net sell and NATO's Rp80 bn net buy (possible negotiated cross).
2. **BBCA results today**: any bank ticket carries a results date inside the holding period; BBRI, BRIS, BBTN and BDMN are due 10-28 to 10-30 (broker estimates).
3. Fed decision lands before the 2026-10-29 open; Alphabet and Microsoft results the same morning.
4. Read the ADHI and PTPP FS for the source of the profit jumps.
5. Board checks from the evening note (GRPM, SOFA, MGLV, BNLI) are still open.
