# HP-DEMO — Handoff Packets

> Handoff Packet là “gói chuyển giao” giữa các chat. Nó truyền context đã duyệt, không tự thêm phân tích mới.

## HP-01-to-04 — ICP → VOC

```yaml
packet_id: HP-01-to-04-DEMO
from_skill: smos-01-icp-builder
to_skill: smos-04-customer-research-voc
artifact_id: SMOS-01-icp-demo-v1
artifact_version: 1.0
source_ids: [EL-DEMO-001, EL-DEMO-002, EL-DEMO-003, BCC-DEMO-001]
```

- **Approved conclusion:** ưu tiên nhà phân phối/3PL 1–5 kho, 20–150 nhân sự, nhiều SKU.
- **Assumptions:** `AL-001`, `AL-002`, `AL-005`.
- **Rejected option:** mọi doanh nghiệp có kho.
- **Open questions:** pain nào lặp lại nhiều nhất; trigger nào làm buyer hành động?
- **Next owner/action/date:** Customer Success — tag 20 ticket/call thật — 2026-09-09.

## HP-04-to-05 — VOC → Positioning

```yaml
packet_id: HP-04-to-05-DEMO
from_skill: smos-04-customer-research-voc
to_skill: smos-05-positioning-messaging
artifact_id: SMOS-04-voc-demo-v1
artifact_version: 1.0
source_ids: [EL-DEMO-001, EL-DEMO-002, EL-DEMO-007]
```

- **Approved themes:** visibility, SKU/return complexity, fear of implementation disruption.
- **Do not infer:** frequency ngoài dữ liệu synthetic; ROI; buyer personality.
- **Next owner/action/date:** Marketing — tạo message house và proof boundary — 2026-09-05.

## HP-06-to-12 — Offer → Lead Research

```yaml
packet_id: HP-06-to-12-DEMO
from_skill: smos-06-offer-builder
to_skill: smos-12-lead-research
artifact_id: SMOS-06-growth-offer-demo-v1
artifact_version: 1.0
source_ids: [EL-DEMO-004, EL-DEMO-005, DR-20260902-03]
```

- **Approved offer:** Growth — tối đa 3 kho, 40 user, scope receiving/picking/cycle count/dashboard.
- **Price boundary:** chỉ dùng giá khi scope được xác nhận.
- **Open question:** account có ERP/migration/integration nào cần estimate?
- **Next owner/action/date:** Sales — research account và map stakeholder — 2026-09-06.

## HP-17-to-18 — Discovery → Proposal

```yaml
packet_id: HP-17-to-18-DEMO
from_skill: smos-17-discovery-analysis
to_skill: smos-18-proposal-builder
artifact_id: SMOS-17-an-phu-discovery-demo-v1
artifact_version: 1.0
source_ids: [EL-DEMO-006, EL-DEMO-007]
```

- **Approved buyer outcome:** giảm rủi ro gián đoạn giao hàng khi chuẩn hóa 2 kho.
- **Evidence:** buyer đã xác nhận 2 kho và lo ngại triển khai; các con số tiết kiệm vẫn là **Chưa biết**.
- **Open question:** ai duyệt ngân sách và timeline go-live mong muốn?
- **Next owner/action/date:** Sales — tạo proposal có phased rollout và assumptions — 2026-09-10.
