# EL-DEMO — Evidence Ledger

> **Synthetic demo data.** Các record dưới đây là bằng chứng giả lập để luyện cách truy vết; không phải nghiên cứu thị trường hoặc testimonial thật.

```yaml
object_type: evidence_ledger
ledger_id: EL-DEMO
version: 1.0
status: synthetic-demo
last_updated: 2026-09-02
```

| Source ID | Type | Date | Synthetic evidence / excerpt | Reliability | Allowed use |
|---|---|---:|---|---|---|
| EL-DEMO-001 | Founder interview | 2026-08-18 | “Nhiều công ty chỉ nhận ra lệch tồn kho khi đã giao thiếu hoặc kiểm kê cuối tháng.” | Medium | pain hypothesis, not a market statistic |
| EL-DEMO-002 | Support theme summary | 2026-08-20 | 12 ticket giả lập: SKU trùng mã, hàng trả về, không biết đơn đang ở kho nào. | Medium | VOC coding, content angles |
| EL-DEMO-003 | Win/loss notes | 2026-08-21 | Deal giả lập thắng vì cần nhiều kho; deal thua vì chỉ so giá với spreadsheet. | Low–Medium | ICP and objection hypotheses |
| EL-DEMO-004 | Product walkthrough | 2026-08-22 | Demo có các màn hình receiving, picking, cycle count, dashboard. | High for demo capability | describe demonstrated workflow only |
| EL-DEMO-005 | Pricing draft | 2026-08-25 | Starter/Growth/Scale và phí triển khai như BCC-DEMO-001. | High for demo price card | offer/proposal practice |
| EL-DEMO-006 | Synthetic customer profile | 2026-08-26 | “An Phú Distribution” giả lập có 2 kho, khoảng 60 nhân sự, nhiều SKU. | Low | lead-research practice only |
| EL-DEMO-007 | Synthetic call note | 2026-08-28 | Buyer nói: “Tôi sợ triển khai làm gián đoạn giao hàng.” | Medium | discovery and objection practice |
| EL-DEMO-008 | Synthetic pipeline export | 2026-09-01 | 5 cơ hội giả lập, có stage, amount, next step, risk. | High for arithmetic exercise | pipeline review practice |

## Source handling rules

- `synthetic-demo` không được trình bày như fact ngoài project demo.
- Quote chỉ được dùng trong phạm vi excerpt; không kéo dài hoặc làm đẹp câu chữ.
- Nếu cần market size, competitor fact hoặc company fact thật, phải research lại với nguồn và ngày.
- Mỗi artifact downstream nên dẫn lại `source_id` đã dùng.
