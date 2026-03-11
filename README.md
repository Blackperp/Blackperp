<p align="center">
  <img src="https://blackperp.com/logo.png" alt="Blackperp" width="120" />
</p>

<h1 align="center">Blackperp Engine</h1>

<p align="center">
  <strong>AI-Powered Perpetual Futures Intelligence</strong><br/>
  <em>173 signals. 25 categories. 7-step pipeline. One trade setup.</em>
</p>

<p align="center">
  <a href="https://blackperp.com">Website</a> •
  <a href="https://blackperp.com/pricing">Pricing</a> •
  <a href="https://blackperp.com/academy">Academy</a> •
</p>

---

## What is Blackperp?

Blackperp is an AI trading intelligence engine for crypto perpetual futures. It does not execute trades. It does not connect to your exchange. It processes **173 real-time derivatives signals** and synthesizes them into confluence-scored **trading zones** with directional bias, entry levels, stop-loss placement, and tiered take-profit targets.

Most platforms show you the data. **[Blackperp](https://blackperp.com) tells you what to do with it.**

---

## Architecture Overview

```
                         ┌─────────────────────────┐
                         │     REAL-TIME INGEST     │
                         │   Funding · OI · Liq ·   │
                         │  Flow · GEX · Sentiment  │
                         └────────────┬────────────┘
                                      │
                                      ▼
                    ┌─────────────────────────────────┐
                    │      SIGNAL CLASSIFICATION       │
                    │     25 categories · 173 signals  │
                    │      [see below ▼]               │
                    └────────────────┬────────────────┘
                                     │
                                     ▼
                         ┌───────────────────────┐
                         │    ZONE ENGINE (7-STEP)│
                         │                       │
                         │  ┌───────────────┐    │
                         │  │ 1. ██████████ │    │
                         │  │ 2. ██████████ │    │
                         │  │ 3. ██████████ │    │
                         │  │ 4. ██████████ │    │
                         │  │ 5. ██████████ │    │
                         │  │ 6. ██████████ │    │
                         │  │ 7. ██████████ │    │
                         │  └───────────────┘    │
                         │                       │
                         └───────────┬───────────┘
                                     │
                                     ▼
                         ┌───────────────────────┐
                         │   ZONE GRADING (S-C)   │
                         │                       │
                         │  S — Maximum confluence│
                         │  A — Strong confluence │
                         │  B — Moderate signal   │
                         │  C — Early formation   │
                         │                       │
                         └───────────┬───────────┘
                                     │
                                     ▼
                    ┌─────────────────────────────────┐
                    │        AI SYNTHESIS (LLM)        │
                    │   Contextual analysis · Regime   │
                    │   detection · Natural language    │
                    │   trade thesis generation         │
                    └────────────────┬────────────────┘
                                     │
                                     ▼
                         ┌───────────────────────┐
                         │     TRADE SETUP        │
                         │                       │
                         │  Bias: LONG / SHORT   │
                         │  Entry: ████████       │
                         │  Stop:  ████████       │
                         │  TP1:   ████████       │
                         │  TP2:   ████████       │
                         │  TP3:   ████████       │
                         │  Confidence: S-tier    │
                         │                       │
                         └───────────┬───────────┘
                                     │
                                     ▼
                    ┌─────────────────────────────────┐
                    │     FEEDBACK / LEARNING LOOP     │
                    │   MFE · MAE · Excursion Tracking │
                    │   Zone parameter optimization    │
                    └─────────────────────────────────┘
```

The redacted blocks (`██████`) represent proprietary pipeline logic. The engine runs live at **[blackperp.com](https://blackperp.com)**.

---

## Signal Categories

The engine ingests and classifies **173 real-time signals** across **25 categories**:

| # | Category | What It Captures |
|---|----------|-----------------|
| 1 | **Funding Rate Regime** | Cross-exchange funding rates, regime classification, extremes |
| 2 | **Open Interest Flow** | OI changes, delta, divergence from price action |
| 3 | **Liquidation Topology** | Cluster mapping, cascade probability, magnet levels |
| 4 | **Order Flow Imbalance** | Buy/sell pressure, aggressive taker flow, absorption |
| 5 | **Smart Money Positioning** | Top trader long/short ratios, account vs. position sizing |
| 6 | **Options Gamma Exposure** | GEX levels, dealer hedging flows, pin risk zones |
| 7 | **Volatility Regime** | IV/RV ratio, term structure, vol-of-vol |
| 8 | **Whale Activity** | Large transaction detection, exchange inflow/outflow |
| 9 | **Exchange Flow** | Net deposits/withdrawals, stablecoin movements |
| 10 | **Market Microstructure** | Spread analysis, depth imbalance, order book shape |
| 11 | **Correlation Matrix** | BTC dominance, alt correlation shifts, regime breaks |
| 12 | **Sentiment Analysis** | Fear & Greed derivatives, social momentum |
| 13 | **Basis & Spread** | Futures basis, cross-exchange spread anomalies |
| 14 | **Leverage Indicators** | Estimated leverage ratio, margin distribution |
| 15 | **CVD (Cumulative Volume Delta)** | Cumulative aggressive buying vs. selling |
| 16 | **Market Maker Fingerprinting** | Algorithmic footprint detection, spoofing signals |
| 17 | **Cross-Exchange Arbitrage** | Price discrepancies, latency signals |
| 18 | **Macro Overlay** | DXY, yields, SPX correlation, macro regime |
| 19 | **On-Chain Metrics** | Active addresses, hash rate, miner flows |
| 20 | **Stablecoin Dynamics** | USDT/USDC supply shifts, minting/burning |
| 21 | **Derivatives Structure** | Term structure, contango/backwardation |
| 22 | **Liquidation Heatmap** | Price levels with highest liquidation density |
| 23 | **Position Crowding** | Overcrowded trade detection, pain trade probability |
| 24 | **Time & Session Analysis** | Session-based behavior, kill zone detection |
| 25 | **Confluence Scoring** | Meta-signal: how many categories align at a zone |

Each signal is weighted dynamically based on current market regime. The weighting logic is proprietary.

---

## Trading Modes

| Mode | Timeframe | Target Distance | Signal Weighting |
|------|-----------|----------------|-----------------|
| **Scalp** | Minutes to hours | Tight | Microstructure-heavy |
| **Day** | Hours to end-of-day | Medium | Balanced flow + structure |
| **Swing** | Days to weeks | Wide | Macro + regime dominant |

The engine adapts its entire analysis pipeline based on the selected mode. A scalp setup and a swing setup on the same asset at the same time can have **opposite directional bias** — and both can be correct for their timeframe.

---

## Self-Learning System

Every trade setup generated by the engine enters a feedback loop:

```
Setup Generated → Price Action Tracked → Outcome Recorded
       ↑                                        │
       │          MFE (Maximum Favorable)        │
       │          MAE (Maximum Adverse)          │
       │          Exit State (TP / SL / Expire)  │
       │                                        │
       └──────── Parameter Optimization ◄────────┘
```

- **MFE** — How far did price move in the setup's favor?
- **MAE** — How far did price move against before resolution?
- **Exit State** — Did it hit TP1/TP2/TP3, get stopped out, or expire?

This data feeds back into zone parameter optimization. The engine learns which signal combinations produce the best risk-adjusted outcomes under specific market conditions. No manual curve-fitting. No static parameters.

---

## Example Output Structure

```json
{
  "asset": "BTC-PERP",
  "timestamp": "2026-03-11T14:30:00Z",
  "mode": "day",
  "zone": {
    "grade": "S",
    "type": "████████",
    "confluence_signals": 12,
    "categories_aligned": ["funding", "liquidation", "flow", "gex", "████████"]
  },
  "setup": {
    "bias": "████",
    "entry": "██████",
    "stop_loss": "██████",
    "take_profit": {
      "tp1": "██████",
      "tp2": "██████",
      "tp3": "██████"
    },
    "confidence": 0.87
  },
  "context": "████████████████████████████████████████████████"
}
```

Live outputs available at **[blackperp.com](https://blackperp.com)**.

---

## Free Tools

No account required:

- **[Live Funding Rates](https://blackperp.com/funding)** — Real-time funding data across all major perpetual exchanges
- **[Academy](https://blackperp.com/academy)** — 80+ educational articles on perpetual futures trading

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Engine | Python · FastAPI |
| Frontend | Next.js · SSR |
| Data | Redis · Supabase |
| AI | Claude Opus (Anthropic) |
| Infrastructure | Hetzner · Cloudflare · Nginx · Docker |


---

## Subscription Tiers

| Tier | Price | Per-Credit | Access |
|------|-------|-----------|--------|
| **Core** | €99/mo | €0.99 | Engine outputs + 15 signal categories |
| **Pro** | €199/mo | €0.66 | All 25 categories + AI analyst |
| **Black** | €499/mo | €0.33 | Full access + priority + all modes |

Details at **[blackperp.com/pricing](https://blackperp.com/pricing)**.

---

## This Is Not a Trading Bot

Blackperp does not:
- Connect to your exchange
- Execute trades on your behalf
- Manage your positions or risk
- Promise guaranteed returns

It eliminates the **analytical bottleneck** — the part where you're manually processing 25 data streams and trying to figure out what they collectively mean. You handle execution. You handle risk. You make the final call.

**Intelligence augmentation, not automation.**

---

## Links

| | |
|---|---|
| **Website** | [blackperp.com](https://blackperp.com) |
| **Pricing** | [blackperp.com/pricing](https://blackperp.com/pricing) |
| **Academy** | [blackperp.com/academy](https://blackperp.com/academy) |


---

<p align="center">
  <em>Built by a trader. For traders.</em><br/>
  <a href="https://blackperp.com"><strong>blackperp.com</strong></a>
</p>
