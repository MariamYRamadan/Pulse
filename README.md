# Pulse — Product Metrics Intelligence Dashboard

> A real-time product analytics dashboard for data-driven PMs — DAU/MAU trends, retention cohorts, NPS tracking, A/B test results, RICE prioritization, and sprint health. No API required.

![Version](https://img.shields.io/badge/version-1.0-0ea5e9?style=flat-square) ![Stack](https://img.shields.io/badge/stack-Vanilla%20JS-0ea5e9?style=flat-square) ![Charts](https://img.shields.io/badge/charts-Chart.js-7c3aed?style=flat-square) ![No API](https://img.shields.io/badge/API-none%20required-22c55e?style=flat-square)

**Live demo:** [mariamyramadan.github.io/Pulse](https://mariamyramadan.github.io/Pulse)

---

## Problem Statement

Product managers at FAANG-scale companies make decisions based on dozens of metrics across growth, retention, engagement, and experimentation — but most PM portfolios only show documents and decks. Pulse shows what a PM actually *does* with data: spots trends, runs experiments, prioritizes ruthlessly, and communicates findings to stakeholders.

---

## What's Inside

| Section | Description |
|---|---|
| **Executive Summary** | CPO-level narrative synthesizing all signals into 3 actionable sentences |
| **DAU / MAU Trend** | 30-day daily active and monthly active user chart with segment filtering |
| **NPS Breakdown** | Net Promoter Score with Promoter/Passive/Detractor split and 12-week trend |
| **Retention Cohort Table** | Week-over-week retention by signup cohort, color-coded by health |
| **Feature Adoption Funnel** | 6-step onboarding funnel with drop-off rates at each stage |
| **A/B Test Results** | Live experiment with statistical significance, conversion lift, and revenue impact |
| **Customer Segment Analysis** | Enterprise / SMB / Mobile breakdown with DAU share and key insights |
| **RICE Prioritization** | 6 features scored by Reach × Impact × Confidence ÷ Effort |
| **Sprint Health Dashboard** | Burndown chart, velocity tracking, and P0/P1/P2 task board |
| **PM Insights Engine** | 7 auto-detected signals with HIGH/MED/LOW impact and recommended actions |
| **Segment Filter** | Switch all KPIs between All Users, Enterprise, SMB, and Mobile instantly |
| **Export Report** | One-click markdown report download — ready for Slack or stakeholder email |

---

## Key PM Frameworks Applied

**RICE Scoring**
```
RICE Score = (Reach × Impact × Confidence) ÷ Effort
```
Used to rank 6 Q2 features objectively — removes gut-feel bias from prioritization.

**Stickiness = DAU / MAU**
A Meta/Google-standard engagement metric. Higher stickiness = users return more frequently = stronger product-market fit.

**Retention Cohort Analysis**
Tracks how well each signup week retains users over time. Cohorts that improve signal that product changes are working. Declining cohorts signal churn risk before it shows in aggregate numbers.

**Statistical Significance in A/B Testing**
Variant B shows +18.4% conversion lift at p < 0.01 (99% confidence) — meaning there is less than 1% probability the result is due to chance. Revenue impact calculated at current traffic: +$84K MRR.

---

## Technical Stack

- Vanilla HTML / CSS / JavaScript — zero build step, zero dependencies
- Chart.js 4.4 for all data visualizations
- Syne 800 + DM Sans + DM Mono typography system
- CSS custom properties design system — 8px spacing grid, 6-color semantic palette
- No API calls — works instantly on any device

---

## Agile Process — How This Was Built

### Sprint 1 — Core Analytics

| ID | User Story | Points | Status |
|---|---|---|---|
| US-001 | As a PM, I want DAU/MAU trends with segment filtering, so I can track growth by user type | 8 | Done |
| US-002 | As a PM, I want retention cohort analysis, so I can identify which user groups are churning | 8 | Done |
| US-003 | As a PM, I want NPS breakdown with trend, so I can track satisfaction over time | 5 | Done |

### Sprint 2 — Experimentation & Prioritization

| ID | User Story | Points | Status |
|---|---|---|---|
| US-004 | As a PM, I want A/B test results with statistical significance, so I can make shipping decisions with confidence | 8 | Done |
| US-005 | As a PM, I want RICE prioritization scoring, so I can defend roadmap decisions with data | 5 | Done |
| US-006 | As a PM, I want a feature adoption funnel, so I can identify where users drop off during onboarding | 5 | Done |

### Sprint 3 — Intelligence & Communication

| ID | User Story | Points | Status |
|---|---|---|---|
| US-007 | As a PM, I want an automated insights engine, so I can surface the most critical signals without manual analysis | 8 | Done |
| US-008 | As a PM, I want sprint health tracking, so I can communicate delivery progress to stakeholders | 5 | Done |
| US-009 | As a PM, I want one-click report export, so I can share findings immediately after review | 3 | Done |

---

## Product Learnings

**Revenue impact changes the conversation.** Saying "Variant B has +18.4% conversion" is good. Saying "Variant B has +18.4% conversion — that's +$84K MRR at current traffic" gets the feature shipped immediately. PMs who quantify business impact in dollars get faster decisions.

**Stickiness is more honest than DAU alone.** A product can grow DAU by acquiring more users while existing users churn. DAU/MAU stickiness reveals whether the core experience is compelling — it's the metric that can't be gamed by acquisition spend.

**Cohort analysis reveals what aggregates hide.** Overall retention can look flat while newer cohorts are actually improving significantly. You only see this in cohort view — which is why every growth PM at FAANG looks at cohorts before making product decisions.

**Segment filtering changes every recommendation.** The same metric can tell completely different stories for Enterprise vs SMB vs Mobile. A feature that looks like low priority in aggregate might be critical for the highest-LTV segment.

---

## Roadmap

- Real data integration via CSV upload
- Custom metric builder — define your own KPIs
- Cohort comparison — A vs B cohort on any metric
- Slack/email digest — weekly automated report
- Predictive churn model — flag at-risk accounts

---

## License

MIT — free to use, fork, and build on.

---

*Built by Mariam Elsayed*
