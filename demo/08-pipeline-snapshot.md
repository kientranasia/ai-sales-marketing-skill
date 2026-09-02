# PIPE-DEMO-001 — Pipeline Snapshot

> **Synthetic demo data.** Dùng cho `20 Pipeline Review` và `21 Sales Manager`; tất cả số tiền là VND giả lập.

```yaml
object_type: pipeline_snapshot
snapshot_id: PIPE-DEMO-001
as_of: 2026-09-01
quarter: Q3-2026-demo
target_new_revenue_vnd: 240000000
currency: VND
```

| Opportunity ID | Account | Stage | Amount VND | Close date | Last activity | Next step | Stage evidence | Risk |
|---|---|---|---:|---:|---|---|---|---|
| OPP-DEMO-001 | An Phú Distribution | Discovery complete | 237.000.000 | 2026-09-25 | 2026-08-28 call | gửi phased proposal 10/09 | pain, outcome, stakeholder partly known | budget và timeline chưa biết |
| OPP-DEMO-002 | Nam Việt 3PL | Demo scheduled | 192.000.000 | 2026-09-30 | 2026-08-30 email | demo với Ops Lead 06/09 | problem stated, no economic buyer | champion only |
| OPP-DEMO-003 | Đông Á Parts | Proposal sent | 237.000.000 | 2026-09-12 | 2026-08-26 proposal | confirm review meeting | scope and price sent | no reply 6 days |
| OPP-DEMO-004 | Minh Long Retail | Qualified | 141.000.000 | 2026-10-15 | 2026-08-22 call | verify 3-warehouse scope | fit and trigger plausible | close date is placeholder |
| OPP-DEMO-005 | Hưng Phát Trading | Negotiation | 300.000.000 | 2026-09-08 | 2026-08-29 meeting | resolve implementation concern | buyer and price discussed | security requirement open |

## Stage exit criteria for this demo

- **Qualified:** ICP fit + problem + trigger + next meeting agreed.
- **Discovery complete:** quantified or explicitly unquantified impact, desired outcome, stakeholders, buying process and next step recorded.
- **Proposal sent:** scope, assumptions, price, proof boundary and review date sent.
- **Negotiation:** commercial or implementation issue identified, owner and resolution date set.

## Data quality notes

- Weighted forecast probabilities are **not supplied**; the skill must state assumptions before calculating.
- `Amount VND` is potential contract value, not booked revenue.
- Any opportunity without a dated next step should be flagged as at risk.
