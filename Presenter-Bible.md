# Is AI a Bubble? — Presenter's Bible
*One document: the thesis · the talk (slide-by-slide) · every question they'll ask · all the numbers + sources · what flips the call · the data caveat. Teza lunch talk, 2026-06-25.*

---

## 0 · The 30-second version
- **Not a 1999 bubble. A leveraged bet on demand _duration_.** Real FCF + committed orders, not a narrative.
- Trailing multiples scream bubble; **forward multiples don't** — the gap closes *if* the earnings ramp arrives. So "bubble?" = "does the ramp arrive?"
- It's a **semiconductor** bet (AVGO/NVDA/TSM gap; GOOGL/AMZN don't). Micron is the live proof: trailing screamed bubble, earnings showed up, ~9× forward.
- **Our model:** consensus is demand-**funded through 2027, conditional in 2028** (the crack). Bull case is coherent; the bear needs two contradictory things at once.
- The real froth is in **positioning/flows** (levered ETFs), not the fundamentals.
- **Watch:** hyperscaler capex guidance + realized $/token. **Not the P/E.**

---

## 1 · The talk — slide by slide (what to say)
*Deliver off the bold; don't read it. ~12 min. Full verbatim script in `Speech.md`; this is the current 11-slide arc.*

**1. Title / "The wrong question."** "Bubble or not" is a vibe — untradeable. The price already embeds a demand path; the real question is whether that demand is *achievable*. I'm not calling a top, I'm stress-testing that one expectation.

**2. The underlying is demand.** Past bubbles had a *physical* underlying — fiber, houses, tulips. AI's is **demand**: a forecast, not an asset. "Overpriced" just means the demand assumption is too rich. That's why "looks like 1999" chart overlays miss.

**3. Trailing vs forward multiples.** Trailing looks insane — AVGO **64×**, NVDA 31×. Forward is normal — AVGO **24×**, NVDA **20×**. The gap closes if earnings show, and it's only the **semis** — GOOGL/AMZN are ~27× either way, fair not cheap. *(Micron is held back — it's the next slide's reveal.)* "The cleanest live proof comes next."

**4. "Name this stock." (INTERACTIVE)** Show the anonymous 5-day chart. *Let the room guess* — what is it, what just happened? Take 2–3 guesses. Don't name it. Then advance.

**5. Micron (the reveal).** It's **Micron.** Trailing screamed bubble — ~**49×**, the bears' exhibit A. Then the earnings arrived: HBM **sold out through 2026**, HBM4 ramping 2×, blowout quarter. Multiple collapsed to **single-digit forward** — because earnings *rose into the price*, not because price fell. **A rich trailing multiple is a bubble only if the forward earnings never show. Micron's just did.** *(Honesty: I quote the multiple, not the dollars — the public $ feeds on MU are unreliable; see §5.)*

**6. AI 2026 vs dotcom.** Dotcom leaders didn't earn; ours do (real FCF). They ran on equity; we run on cash + booked orders. **The uncomfortable cell:** capex/sales is already **at-or-above dotcom** (~34% '26 → 39% '27). But it's funded by cash, so the risk is **duration, not solvency.**

**7. The demand is already booked.** Hyperscaler capex is **guided**, not hoped: ~$410B ('25) → ~**$725B ('26 guide)** → >$1T ('27), ~75% AI. That spend **is** the complex's revenue (NVDA DC $194B → ~$343B). The bear case isn't "demand is fake" — it's "the cycle rolls over." Watch the **capex guide**; the first cut is the signal.

**8. Our demand model: forecast vs. required demand.** *(The centerpiece.)* Bottom-up: token demand + disclosed capex → AI-compute $ envelope → our company graph → per-name EPS → **inverted** to the token growth the price *requires*. Left chart: our forecast vs the required bar — **funded '26, funded '27, the 2028 crack.** Two knobs (token volume × $/token deflation) are negatively correlated → bull coherent, bear needs two contradictions at once. Right chart: per-name overshoot — TSM/NVDA defensible, CRDO/MRVL need the aggressive case.

**9. Demand evidence — and the trap.** "AI adopters outperform" shows **nothing** across ~2,000 names; Goldman's basket is *capex-winners*, not adopters. The real soft spot: enterprise ROI — MIT/NANDA, **~95% of corporate gen-AI pilots show no measurable P&L.** Sell-side is structurally long → silence isn't the all-clear; the "1999" calls are **buy-side** (Acadian's Lamont).

**10. Levered-ETF positioning (the froth).** US levered/inverse ETF exposure **$464B** (record); **$185B** net inflow in two months (record); ~205 single-stock underliers, AUM piled into MU/NVDA/TSLA. The froth is real — but it's in **positioning & flows**, a flows-unwind risk, *not* the fundamentals.

**11. Verdict.** Not 1999 — a bet on demand **duration**. Bull: cheap on forward. Base: fair. Bear: hyperscalers cut → the air-pocket, and that's where the bubble lives, **in the semis.** Ride it if you want — the risk is **timing the exit, not the valuation.** Watch capex guidance + $/token, not the P/E.

---

## 2 · Q&A — every question they'll throw
*Crisp answer · the number · the honest caveat. Default tone: concede the real points, hold the line on the structural ones.*

### Valuation / multiples
- **"Forward multiples assume consensus EPS — what if consensus is a sell-side fantasy?"** Fair, and it's why I built our own bottom-up EPS (slide 8) as an independent check. Our model funds consensus through 2027; 2028 is where it's conditional. If you don't believe consensus *or* our model, you're making a pure demand-pessimism bet — which is a view, not a valuation argument.
- **"AVGO forward is low-30s on FY2, not 24× — your gap shrinks."** True for FY2 vendors (GuruFocus/Finbox). I quote FY1/NTM (stockanalysis). Even at low-30s the compression vs 64× trailing holds; the *direction* is the point, not the decimal.
- **"Trailing 64× is just a bubble with extra steps."** Only if forward earnings never arrive. Micron is the existence proof that they can — and the table shows GOOGL/AMZN aren't even stretched. This isn't "everything's cheap," it's "the semis price a ramp."

### The demand model & the 2028 crack
- **"Walk me through the model."** Token demand × realized $/token, reconciled to disclosed capex → AI-compute $ envelope by layer → graph attribution to companies → per-name EPS → invert to required token growth. Output: is consensus demand-funded, and where does it break? (Reproduce: `semiconductor-flow-graph/research/token_eps/build_eps_projection.py`, re-run 06-25.)
- **"Why do you trust 2026/27 but flag 2028?"** Forecast token path **×6.7 vs ×5.3 required** in '26 (funded with room); **×4.0 = ×4.0** in '27 (funds consensus exactly); **×2.6 vs ×3.7** in '28 — the forecast falls short *unless* $/token deflation stays slow. That's the crack.
- **"Isn't the bull case just hand-waving?"** No — it's structurally constrained. The two drivers (token volume ↑, $/token deflation δ) are *negatively correlated*: heavy reasoning/agentic tokens deflate slowly. So the bull is internally coherent and the bear needs **two contradictory things at once** (high deflation *and* slowing volume).
- **"What's your central deflation assumption?"** δ = **−65%** realized $/token. At −50% the required bar drops (consensus needs only ×2.8); at the headline **−85% "LLMflation"** it balloons to ×9.3 — unreachable. The evidence says realized δ is −40 to −65% as demand mixes up into pricier reasoning tokens, not −85%.

### Enterprise ROI (the strongest bear point)
- **"95% of gen-AI pilots fail — isn't that the whole bear case?"** It's the strongest bear point and I won't dodge it (MIT/NANDA 2025). But it's a **2028 / enterprise-ROI** risk, not a near-term revenue risk — near-term is backed by committed hyperscaler capex. If ROI doesn't show by ~2028, the capex cycle rolls and the bear scenario hits. It's exactly why 2028 is conditional.
- **"'No measurable P&L' — is that the same as 'no value'?"** No. The study is 150 interviews + 350-person survey + 300 deployments; "no measurable P&L impact" ≠ "useless." But for *funding the capex* what matters is measurable return, and that's the gap.

### Circular financing / capex durability
- **"Isn't this circular — hyperscalers funding their own suppliers' revenue?"** Partly yes — that *is* the duration risk in one sentence. The check is **end-AI ROI**: real end-demand has to validate the spend or the loop breaks. That's why the watch-item is the first capex-guide cut, and why enterprise ROI (above) is the soft spot.
- **"What if a hyperscaler cuts capex?"** That's the single highest-signal bear event — the "first cut is the signal." Near-term it would hit the semis hardest (they price the ramp). It's #1 on the watch-list.
- **"$725B / >$1T — is that real or analyst fantasy?"** 2026 ~$725B is **company-guided** (MSFT $190B, Meta $125–145B, Alphabet $180–190B, etc.) and being spent — hard evidence. The >$1T for 2027 is an **analyst projection (Morgan Stanley), not guidance** — I flag it as such.

### Froth / positioning
- **"You admit there's froth — so it IS a bubble?"** The froth is real but **located**: it's in levered-ETF positioning ($464B, record $185B 2-month inflow, ~205 single-stock underliers piled into MU/NVDA/TSLA). That's a **flows-unwind** risk — mechanically different from the demand risk. A crowded-trade problem, not a "these companies don't earn" problem.
- **"Couldn't a flows unwind crash the names anyway?"** Yes — short-term, a levered-ETF deleveraging can overshoot fundamentals. That's a *timing/risk-management* point, not a valuation verdict. It's why the practical advice is "the risk is timing the exit."

### Micron & the data caveat (see §5)
- **"Did Micron really do $41.5B in a quarter / trade at $1,200?"** The public $ feeds are **unreliable** — $41.5B would be ~4.5× Micron's entire prior fiscal year and ~the whole global memory market in a quarter; impossible to 4× fab output in nine months. So I quote the **ratio** (~9× forward), which is robust to the scaling, plus the qualitatively-confirmed HBM-sold-out story. If someone has a Bloomberg print, I'll take the exact figure — the *thesis* (multiple collapses as earnings arrive) doesn't depend on the dollars.
- **"81% gross margin on memory?"** Also a data-quality flag — real Micron peaks ~35–45%. Same lineage; same answer: trust the ratio and the sold-out order book, not the absolute prints.

### Dotcom comparison
- **"How is this different from 1999?"** Two ways: leaders earn real cash (dotcom mostly didn't), and it's funded by cash + booked orders (dotcom by equity + narrative). The **honest** similarity: on capex/sales *intensity* we're at-or-above dotcom peak. So the risk rhymes on *intensity/duration*, not on *solvency*.
- **"The .ai / Anguilla thing?"** A fun edge-echo — Anguilla earns ~$93M (~47% of govt revenue) off .ai domains in 2025, up from ~$3M in 2018. Froth at the edges, real earnings at the core. (History rhymes; it's color, not the argument.)

### Methodology / "why believe you"
- **"Where do your numbers come from?"** Five parallel verification agents swept the web per claim, then I direct-fetched the contested ones and re-ran the model locally. Default stance: unverifiable if no credible source. Full audit in `Reasoning Log & Sources.md`. (The Micron catch — §5 — is the case study: the web consensus was internally consistent *and wrong*; the fix was an economic-impossibility check, not majority vote.)
- **"What would change your mind?"** Bearish: (1) a hyperscaler cuts capex guidance; (2) realized $/token deflates at −85% while volume slows; (3) enterprise ROI stays ~5% and bites budgets; (4) NVDA DC misses consensus. Bullish: capex guidance raised again + reasoning/agentic mix accelerating.

### Trading / positioning
- **"So how do you trade it?"** Long the **irreplaceables** (TSM, NVDA — capture the volume if it comes), short/underweight the **high-overshoot replaceables** (MRVL, CRDO, AMD — need the aggressive token path *and* can't hold share). The 2028 token-bar shortfall + replaceability = the short; coverage + irreplaceability = the long.
- **"If you're so sure, why not just be long?"** I'm scoping risk, not selling a direction. Base/bull says cheap on forward; the live risks are a flows unwind (slide 10) and a 2028 demand air-pocket. Both are *timing* problems — which is why the watch-item is capex guidance, not the multiple.

### Macro
- **"What about rates / a recession?"** Orthogonal to the thesis but real: a demand shock would show up first as a **capex-guide cut** (the watch-item already covers it). The model is a demand-duration model, not a macro call.

---

## 3 · Facts & figures (with source)
*All verified 2026-06-24/25 unless noted. Full trail: `Reasoning Log & Sources.md`.*

| # | Fact | Source |
|---|---|---|
| Multiples | NVDA 30.5×→20.0× · AVGO 63.6×→24.3× · TSM 32.7×→22.7× · MSFT 21.8×→19.7× · META 20.3×→17.0× · GOOGL 26.3×→27.6× (no gap) · AMZN 28.0×→28.1× (no gap) · MU 23.7×→8.9× (*$ corrupt, ratio ok) | stockanalysis.com /statistics |
| Capex | $226B('24) → $410B('25) → ~$725B('26 guided) → >$1T('27, MS projection); ~75% AI; Goldman **$5.3T** cumulative '25–'30 | CNBC 02-06; MSFT Q3; Goldman (Sedaily 06-04); MS (FXStreet 05-04) |
| Hyperscaler '26 | MSFT ~$190B · Alphabet ~$180–190B · Meta ~$125–145B · Oracle ~$56B | CNBC 04-29; company guidance |
| NVDA | DC rev **$194B** (FY26 actual) → ~**$343B** (FY27 consensus); ~56% net margin | NVIDIA newsroom; Visible Alpha/S&P |
| Accel. TAM | ~$150–160B (2025) → ~**$440B by 2030** (~25% CAGR) | Mordor/Yole |
| Capex/sales | ~32% (dotcom peak) vs **~34% ('26) → 39% ('27)** | Morgan Stanley / Castagno 02-26 |
| Enterprise ROI | **~95%** of corporate gen-AI pilots show no measurable P&L | MIT NANDA 2025 |
| Froth | levered/inverse ETF exposure **$464B**; record **$185B** 2-mo inflow; **~205** single-stock underliers (MU $8B/NVDA $6B/TSLA $5B) | Goldman (Artem) |
| Model | accel. $ envelope 197/218/228('26) → 213/255/319('27) → 223/286/414('28); required token bar ×2.8/×4.0/×9.3; **funded '26–'27, conditional '28** | `build_eps_projection.py`, re-run 06-25 |
| .ai/Anguilla | ~$93M = ~47% of govt revenue (2025), up from ~$3M (2018) | Anguilla Focus 09-12 |
| Cautious voices | "euphoric" = Wells Fargo (still bullish); **"2026 = 1999" = Owen Lamont, Acadian (buy-side)** | Fortune 05-13, 06-08 |

---

## 4 · What flips the call
- **Bearish triggers:** hyperscaler cuts capex guidance · realized $/token at −85% while volume slows · enterprise ROI stuck ~5% and biting budgets · NVDA DC misses consensus.
- **Bullish triggers:** capex guidance raised again · reasoning/agentic token mix accelerating (slow deflation + high volume).
- **The one watch-item:** realized blended **$/token** (provider revenue ÷ tokens) + reasoning-mix share, and the next **capex guide**. Not the headline P/E.

---

## 5 · ⚠ The Micron data caveat (must-know before you stand up)
The public feeds print Micron at **~$1,200, ~$41.5B quarterly revenue, ~81% GM** — **treat the absolute dollars as corrupt.** $41.5B is ~4.5× MU's *entire* prior fiscal year and ~the whole global memory market in one quarter; you can't 4× fab output in nine months, and Micron is the #3 memory maker (~20–25% share). The 52-week range ($103 → $1,213) with the low at the *real* price is the fingerprint of unadjusted/scaled data.
- **What's real:** HBM sold out through 2026, HBM4 ramping, a genuine memory super-cycle.
- **What to say:** quote the **forward multiple (~9×)** — robust because price and EPS are scaled together, so the ratio survives — and the sold-out order book. *Not* the dollar prints.
- **If pressed for the exact number:** "The public feeds are unreliable on Micron's absolute dollars; I'm quoting the ratio. Hand me a Bloomberg print and I'll use the exact figure — the thesis doesn't depend on it."

---

## 6 · The interactive game (slide 4)
Slide 4 is an **anonymous** 5-day price chart — no ticker, no name, no price level. Show it, ask *"what stock, and what just happened?"*, take 2–3 guesses, **then** advance to slide 5 to reveal it's Micron. The setup: the trailing multiple was pricing exactly this earnings ramp, and it just arrived. (Slides 1–3 are Micron-free so nothing spoils it; the answer is in the speaker notes only, stripped from the public copy.)

---
*Companions in this folder: `Speech.md` (full verbatim script) · `Cue Card.pdf` (lectern one-pager) · `Model — How It Works….md` (model deep-dive) · `Reasoning Log & Sources.md` (full audit trail).*
