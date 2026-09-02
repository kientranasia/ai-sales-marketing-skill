# DR-DEMO — Decision Records

> Các quyết định này chỉ phục vụ demo. Khi dùng production, thay bằng người duyệt, nguồn và ngày thật.

## DR-20260902-01 — Chọn ICP cho demo

```yaml
object_type: decision_record
decision_id: DR-20260902-01
date: 2026-09-02
status: approved-for-demo
owner: Demo Operator
```

- **Decision:** ưu tiên nhà phân phối/3PL tại Việt Nam có 1–5 kho, 20–150 nhân sự và nhiều SKU.
- **Evidence:** `EL-DEMO-001`, `EL-DEMO-002`, `EL-DEMO-003`, `BCC-DEMO-001`.
- **Why:** pain vận hành có thể quan sát; product fit tốt hơn nhóm kho rất nhỏ.
- **Rejected:** “mọi doanh nghiệp cần quản lý kho” vì quá rộng; “chỉ công ty enterprise” vì vượt scope demo.
- **Open question:** ngưỡng order line và trigger nào dự báo conversion tốt nhất?

## DR-20260902-02 — Message house

```yaml
decision_id: DR-20260902-02
date: 2026-09-02
status: approved-for-demo
```

- **Core message:** FlowNest giúp đội vận hành nhìn thấy và chuẩn hóa luồng nhập–xuất–tồn trước khi lỗi nhỏ thành vấn đề giao hàng.
- **Proof boundary:** chỉ mô tả workflow đã demo; không hứa ROI hoặc phần trăm cải thiện.
- **Evidence:** `EL-DEMO-002`, `EL-DEMO-004`.
- **Rejected:** “AI tự động hóa toàn bộ kho” vì capability chưa được chứng minh.

## DR-20260902-03 — Offer để luyện proposal

```yaml
decision_id: DR-20260902-03
date: 2026-09-02
status: approved-for-demo
```

- **Decision:** dùng Growth package làm phương án mặc định cho account có 2–3 kho.
- **Scope:** receiving, picking/packing, cycle count, dashboard, migration workshop.
- **Price reference:** `EL-DEMO-005` và `BCC-DEMO-001`.
- **Commercial guardrail:** proposal phải ghi assumptions, exclusions, implementation milestones và điều kiện thay đổi scope.
