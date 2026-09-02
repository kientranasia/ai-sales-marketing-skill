# LEAD-DEMO-001 — Account & Contact Object

> **Synthetic demo data.** Dùng để luyện `12 Lead Research`, `13 Qualification`, `14 Outreach`, `15 Follow-up`, `16 Call Prep` và `18 Proposal`.

```yaml
object_type: lead_account
account_id: ACC-DEMO-001
account_name: An Phú Distribution
contact_id: CON-DEMO-001
contact_name: Minh Nguyễn
contact_title: Operations Manager
contact_email: minh.nguyen@example.invalid
contact_phone: +84-900-000-001
status: synthetic-demo
source_id: EL-DEMO-006
```

## Account facts

- **Industry:** phân phối hàng tiêu dùng và thiết bị gia dụng.
- **Location:** Bình Dương, Việt Nam (demo fact).
- **Employees:** khoảng 60 (synthetic estimate; cần xác minh).
- **Warehouses:** 2 kho; kho chính và kho cross-dock.
- **SKU:** khoảng 6.000 mã (synthetic estimate; cần xác minh).
- **Current workflow:** spreadsheet + phần mềm kế toán; nhiều bước kiểm tra thủ công.
- **Known initiative:** muốn chuẩn hóa barcode và visibility tồn kho trước mùa cao điểm.
- **Likely stakeholders:** Operations Manager (champion), General Manager (economic buyer), kế toán/IT (influencer).

## Research boundaries

- Không suy đoán doanh thu, giới tính, tuổi, tính cách hoặc quyền quyết định ngoài dữ liệu.
- Chưa biết: order lines/month, budget, ERP, go-live date, procurement process, security requirements.
- Không dùng email/phone này để gửi thật; domain `.invalid` chỉ để demo.

## Trigger and pain hypotheses

1. Tăng volume làm spreadsheet khó kiểm soát.
2. Hai kho tạo ra sai khác tồn hoặc khó biết đơn đang ở đâu.
3. Mùa cao điểm làm buyer sợ gián đoạn giao hàng khi triển khai.

## Suggested qualification questions

- Vấn đề nào khiến đội kho mất thời gian hoặc tạo lỗi nhiều nhất?
- Có event/timeline nào khiến dự án phải hoàn tất trong quý này không?
- Ai cùng tham gia chọn hệ thống và ai phê duyệt ngân sách?
- Tiêu chí để gọi pilot hoặc go-live thành công là gì?
