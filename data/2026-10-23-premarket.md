# Pre-market intel — Friday 2026-10-23 (IDX trading day)

Run: cloud night shift, 06:11 WIB (tools/clock.py: trading_day=true, before_open=true, last session 2026-10-22).
Paper holdings: none (desk/paper/portfolio.json, cash Rp150,000,000). alerts.md: no change.

## Data access — read first
- `tools/idx.py` and `tools/prices.py` both returned `unavailable`: the cloud egress proxy refuses CONNECT to **www.idx.id** and **query1.finance.yahoo.com** (403 policy denial, 2026-10-22 23:11 UTC). This is the cloud sandbox's allow-list, not the sites.
- So this note has **no IDX disclosures from the tool, no volume ratio, gap, ARA/ARB or flow data from the tools**. Everything below comes from web search and news pages. Attention scores are partial (outlets only); the morning desk must recompute volume ratio, gap, ARA/ARB and flow from the tools.
- Several sites refused the fetch (Bloomberg, investor.id, mediakompeten, some kontan and bisnis pages). Stories from those are marked **headline-only**.

## Last IDX session (2026-10-22)
- IHSG closed at **5,387.90, +1.11%** (third gain in a row). Range 5,185 to 5,422. Value Rp16.20 tn, breadth 467 up / 204 down. Source: Kontan, "Asing Net Sell Rp 1,49 Triliun Saat IHSG Menguat 1,11%, Cek Saham yang Banyak Dilepas", 2026-10-22 22:44 WIB.
- Benchmark since paper inception: 5,328.36 (close 2026-10-21) → 5,387.90 = **+1.12%**.
- Foreign flow: **net sell Rp1.49 tn**. Top net sells: BBCA Rp624.61 bn, TLKM Rp332.23 bn, BBRI Rp257.92 bn, BRIS Rp82.12 bn, ASII Rp77.72 bn, BBNI Rp75.53 bn, TINS Rp43.83 bn, BRMS Rp40.81 bn, ANTM Rp34.69 bn, PTBA Rp31.20 bn (Kontan, as above). Top net buys: BMRI Rp152.31 bn, DMAS Rp52.48 bn, AMMN Rp51.26 bn, GOTO Rp42.99 bn, SINI Rp22.91 bn (InvestorTrust, "Net Sell Berlanjut Rp 1,49 Triliun, Terbanyak Landa BBCA hingga TLKM", 2026-10-22 18:02 WIB). Estimates by the press, not tools/flow.py.
- Big-cap movers: BREN +7.41% (Rp2,320), BBRI +3.20% (Rp2,900), BMRI +4.05% (Rp3,850), BBNI +4.92% (Rp3,410), AMMN +5.61% (Rp3,950). Tech sector −0.66%. ASMI +35% (Rp27) and ENAK +34.81% (Rp182), both probably at ARA (unverified, no tool data). Source: InvestorTrust, as above.
- Context: foreign selling continues despite a three-day rebound. The background is the MSCI overhang on Indonesia (Bisnis, "Wacana MSCI Tekan IHSG, Investor Asing Asyik Borong Saham BBCA-ASII", 2026-10-17; Kontan pusatdata, "Net Sell Asing Mencapai Rp 335 Triliun Saat IHSG Longsor 1157 pada 16 Oktober 2026"). The MSCI details are **headline-only** this run; read in full.

## Overnight global (US session 2026-10-22, closed ~04:00 WIB 2026-10-23)
| Driver | Move | IHSG read-across | Source / time |
|---|---|---|---|
| S&P 500 | −1.2% (CFD 7,663) | risk-off; pressure on foreign flow | Trading Economics, US stock market page, 2026-10-22 close |
| Nasdaq | −2.9%; Dow +0.02% (52,868) | AI-capex worries (Meta −7%, Lam −11.8%, Nvidia −4.4%, AMD −8.1%); tech and data-centre names (DCII) face sentiment pressure | same |
| Nikkei 225 | −2.60% to 62,942 (3-month low); Shanghai −1.48%; ASX −0.43% | weak Asian lead | Trading Economics, Japan page, 2026-10-22 |
| Brent | ~US$112.9, about +4% (highest since early May); WTI ~US$99.0, +2.3% | + oil and gas upstream (MEDC, ENRG); − fuel-cost users (GIAA, logistics); fuel subsidy pressure on the rupiah and the budget | Trading Economics, Brent page, 2026-10-22. Cause: Houthi attacks in Saudi Arabia (Dammam airport), US staff ordered out, reports that US strikes on Iran may resume |
| Gold | ~US$4,024/oz, about −2.8% (lowest since early August) | − gold miners (ANTM, MDKA, EMAS, BRMS, PSAB); ANTM and BRMS were already on the foreign net-sell list | Trading Economics, gold page, 2026-10-22 |
| Coal (Newcastle) | 151.15, +0.4% | neutral for PTBA, ADRO/AADI, ITMG | same |
| Nickel, CPO | **unverified** (fetch refused) | — | — |
| USD/IDR | 18,022 at the 2026-10-21 close (−0.17%, above 18,000) | weak rupiah plus oil = imported inflation | Bisnis, "Nilai Tukar Rupiah Terhadap Dolar AS Hari Ini Kamis 22 Oktober 2026", 2026-10-22 06:15 WIB |
| BI | BI rate held at 5.75% on 2026-10-21; only the deposit facility rate was raised | rate-sensitive sectors (property, banks) neutral to slightly negative | same |
| Fed | FOMC 27–28 Oct expected to hold; markets price a high chance of a December hike; PCE due next week | foreign outflow risk persists | Trading Economics, gold page, 2026-10-22 |

Morning read: a weak external lead (Nasdaq −2.9%, Nikkei −2.6%) after a three-day IHSG rebound that came with heavy foreign selling. Expect profit-taking pressure at the open. Oil names are the relative winners and gold miners the relative losers.

## Issuer stories (24 h), attention (partial: outlets only)
Formula components not computed: disclosure +3, volume ratio, gap, ARA/ARB, top-20 flow. The morning desk adds these from the tools.

| Ticker | Outlets | Story | Status |
|---|---|---|---|
| PTPP | 3 (Bisnis, Kontan, Katadata/Databoks) | Q3 2026 results: 9M net profit **Rp259.96 bn, up about 46-fold yoy** (Databoks/Mediakompeten say +4,576%), while revenue **fell**. | **headline-only**. Titles: "PTPP Cetak Laba Bersih Rp25996 Miliar Kuartal III/2026, Meroket 46 Kali Lipat" (Bisnis 2026-10-22); "Laba PT PP (PTPP) Naik Meski Pendapatan Turun per Kuartal III 2026" (Kontan). A low base or a one-off is likely; read the IDX FS for the source of the profit |
| DCII | 2 (Bisnis, Kontan) | 9M 2026 revenue **Rp2.52 tn, +31.49%** yoy (colocation Rp2.38 tn); net profit **Rp919.8 bn, +11.5%**; cost of revenue +46.6% (margin squeeze); total assets +51% YTD to Rp10.06 tn; liabilities nearly doubled to Rp5.13 tn (capex build-out). | Read in full: Bisnis, "Emiten Data Center Toto Sugiri DCII Cetak Laba Bersih Rp919,8 Miliar Kuartal III/2026", 2026-10-22 19:18 WIB, citing the company FS. Overnight AI-capex sell-off is a sentiment headwind. Check liquidity before any ticket |
| PGUN | 2 (Databoks, Bisnis) | 9M 2026 net sales Rp566.10 bn, +5.26% yoy; net profit **Rp135.44 bn, +33.53%** ("record"). | Databoks, "Emiten Haji Isam PGUN Cetak Rekor Laba pada Kuartal III 2026", 2026-10-22 11:47 WIB; the Bisnis story is headline-only |
| BBCA | 2+ | Largest foreign net sell (Rp624.61 bn) amid the MSCI overhang | Kontan / InvestorTrust, 2026-10-22 |
| BMRI | 2 | Largest foreign net buy (Rp152.31 bn), +4.05% | InvestorTrust, 2026-10-22 |
| AMMN | 1 | +5.61%, foreign net buy Rp51.26 bn; the gold drop overnight works against it | InvestorTrust, 2026-10-22 |
| BREN | 1 | +7.41% to Rp2,320; no story found | InvestorTrust, 2026-10-22 |
| ASMI, ENAK | 1 | +35% / +34.81%, probably ARA; no story found | InvestorTrust, 2026-10-22 |
| ANTM | 2 | Q3 results previewed as "solid" (not yet released); gold −2.8% overnight | Pojokpapua / Mediakompeten, "Kinerja ANTM Kuartal III-2026 Diproyeksi Tetap Solid" — headline-only, preview not results |

### EARNINGS-CHANGE pre-flags (night shift, for catalyst to confirm)
- **PTPP**: net profit change far above 10%, but revenue fell. Mechanism unknown (possible one-off or low base). Next-4-quarter effect is undetermined; confidence **low** until the FS is read.
- **DCII**: revenue +31% and net profit +11.5% on 9M. Run-rate growth from colocation capacity. Next-4-quarter revenue likely +20–30%; confidence **medium** (from the company FS via Bisnis, not yet checked against IDX).
- **PGUN**: net profit +33.5% on revenue +5.3% (margin and CPO price led). Confidence **medium-low**; needs Q3-only figures and the consensus.

## Corporate actions in the next 10 trading days (from news; confirm with tools/idx.py actions)
- CSRA: dividend Rp15; ex (regular) **2026-10-23**, pay 2026-11-13.
- SCMA: dividend Rp8.4; cum (regular) 2026-10-27, ex 2026-10-28, pay 2026-11-18.
- DMAS: dividend Rp29; cum (regular) 2026-10-28, ex 2026-10-29, pay 2026-11-13. It was also #2 foreign net buy on 2026-10-22.
- AXIO: dividend Rp8; cum (regular) 2026-10-28, ex 2026-10-29.
- IMPC: Rp5, already ex 2026-10-22; pay 2026-10-30.
- DOOH: rights issue (up to 95.24% dilution) plus INET acquisition; RUPSLB 2026-11-09.
- AALI: buyback up to Rp400 bn running to 2026-12-28.
Source: Katadata, "Deret Emiten Tebar Dividen Akhir Oktober 2026, IMPC hingga DMAS Mana Menarik?", 2026-10-21; HeyGoTrade, "Aksi Korporasi Emiten (DOOH Rights Issue & Akuisisi INET, Dividen Interim BMRI, Buyback AALI, DADA ARB)", 2026-10-02.

## For the morning desk
1. Recompute attention with the tools (disclosures, volume ratio, gap, ARA/ARB, flow). The cloud could not reach www.idx.id or Yahoo.
2. Read PTPP's IDX FS for the source of the profit before rating it.
3. Read the MSCI story on Indonesia in full: it is the main driver of foreign flow.
4. No evening shift output exists for 2026-10-22 (intel/2026-10-22/evening.md missing), so the Q3 results flow (PTPP, DCII, PGUN) has not been checked against IDX disclosures.
