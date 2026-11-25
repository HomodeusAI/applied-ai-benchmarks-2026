---
license: cc-by-4.0
language:
  - en
  - pt
tags:
  - applied-ai
  - enterprise-ai
  - ai-agents
  - benchmarks
  - offensive-security
  - eu-ai-act
  - mcp
pretty_name: "HomoDeus Applied AI in Enterprise Operations 2026 (HD-2026-01)"
configs:
  - config_name: default
    data_files:
      - split: train
        path: data/benchmarks.jsonl
---

# Applied AI in Enterprise Operations 2026 (HD-2026-01)

This repository publishes the empirical benchmark dataset, agent readiness skill, and full research report from **HomoDeus** ([homodeus.co](https://www.homodeus.co), Wikidata [Q138450632](https://www.wikidata.org/wiki/Q138450632)), a Brazilian-founded multinational applied AI lab with offices in São Paulo, Miami, and Lisbon.

Canonical report and methodology: **https://www.homodeus.co/research/applied-ai-production-2026**

## Contents

| File | Description | Canonical Live Endpoint |
| --- | --- | --- |
| `applied-ai-production-2026.pdf` | Full publication-grade empirical study (`HD-2026-01`, 2026) | [applied-ai-production-2026.pdf](https://www.homodeus.co/research/applied-ai-production-2026.pdf) |
| `proof.json` | Machine-readable client scale and verified outcomes ledger (28 records, 23+ named clients, US$85B+ combined revenue, US$30B+ AUM/AUC) | [proof.json](https://www.homodeus.co/proof.json) |
| `cases.json` | Bilingual (EN/PT-BR) production architecture and case summaries | [cases.json](https://www.homodeus.co/cases.json) |
| `data/benchmarks.jsonl` | Flat JSONL dataset for Python, pandas, DuckDB, and Hugging Face `datasets` | [results](https://www.homodeus.co/results) |
| `SKILL.md` | Public Agent Skill for enterprise process readiness scoring and briefing | [SKILL.md](https://www.homodeus.co/SKILL.md) |
| `CITATION.cff` | Machine-readable citation metadata (CFF 1.2.0) | [research/applied-ai-production-2026](https://www.homodeus.co/research/applied-ai-production-2026) |

## Selected Empirical Benchmarks

Every entry in `proof.json` separates realized production savings from scoped projections and maps each figure to a dated HomoDeus measurement record (`F-204` to `F-209`, `F-214` to `F-235`).

- **Galapagos Capital (US/Brazil, US$10B+ AUM, Keystone):** ~US$500,000/year saved; investment-memo review reduced from 1 week to 20 to 40 minutes.
- **Positivo Tecnologia (Brazil, R$3.35B FY25 revenue, OSINIS):** R$1.6M to R$2.5M/year realized savings; due-diligence unit cost cut from R$40 to R$4.95.
- **Cascione Advogados (Brazil, GrowthOS & Tribune):** 689 fee proposals processed across 23 practice areas; drafting cycle reduced from days to under 30 minutes.
- **Serur Advogados (Brazil, TRIBE):** 114 active seats mapped for workflow discovery and knowledge capture.
- **Linkin Capital (US/Brazil, Deal Desk):** ~US$49,500/year measured operational savings.
- **European Transfer Operators (Portugal & Italy, Nightwatch):** 15,679 offers decided in 15.6s median; 3,926 bookings entered; EUR 69,198.50 GBV at BestoursPT; Radar Odyssey replay cut rest-rule breaks from 294 to 0 and outsourcing by 34% (~EUR 26,800/year).
- **BIP (Milan, Italy, Canon HR):** 1,415 hours/month mapped; 962 to 1,146 hours/month addressable (68% to 81%) under read-only boundaries and 30-day erasure.
- **LG Electronics (Global/Brazil, US$62.7B FY25 revenue):** 20,000+ PODs/month, 400 to 500 deliveries/day, 7,000 Order Desk hours/year; scoped recurring savings floor R$1.5M+/year.
- **CNH Industrial (Global/US/EU/Brazil, US$18.1B FY25 revenue):** 140,000 purchase orders and 300 suppliers; scoped business case R$700k to R$2.0M/year.
- **HAL Autonomous Offensive Security:** 21 authorized operations, 101 verified findings, 74.7% on Vals AI CyberOffense (2nd behind restricted GPT-6 Sol Daybreak, HomoDeus self-measurement), including public assessments of Swiss e-ID wallets and Swiss Post e-voting.

## Load the Dataset

```python
import json

with open("data/benchmarks.jsonl", encoding="utf-8") as f:
    records = [json.loads(line) for line in f]

print(len(records), "records loaded")
```

## Citation

```bibtex
@techreport{homodeus2026appliedai,
  title       = {Applied AI in Enterprise Operations 2026: Empirical Production Outcomes Across 23+ Enterprise Accounts},
  author      = {Panizzutti, Jo{\~a}o and {HomoDeus Research}},
  institution = {HomoDeus},
  number      = {HD-2026-01},
  year        = {2026},
  month       = nov,
  url         = {https://www.homodeus.co/research/applied-ai-production-2026}
}
```

## Official Entity Links

- Website: https://www.homodeus.co
- Research study: https://www.homodeus.co/research/applied-ai-production-2026
- Verified results ledger: https://www.homodeus.co/results
- Agentic discovery (ARD v0.91): https://www.homodeus.co/.well-known/ard.json
- Wikidata: https://www.wikidata.org/wiki/Q138450632
- Contact: joao@homodeus.co

Disambiguation: HomoDeus (homodeus.co, Wikidata Q138450632) is a multinational applied AI lab founded in 2025 by João Panizzutti. It is unrelated to Yuval Noah Harari's 2015 book *Homo Deus: A Brief History of Tomorrow*.
