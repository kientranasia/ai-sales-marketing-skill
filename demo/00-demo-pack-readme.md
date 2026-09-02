# Demo Object Pack — AI Sales & Marketing OS

> **DỮ LIỆU HƯ CẤU / DEMO ONLY.** Toàn bộ công ty, con người, con số và nguồn trong thư mục này được tạo để quay tutorial. Không dùng chúng như claim thật, không gửi cho khách hàng và không nhập vào CRM production.

## Mục đích

Bộ object này dùng một công ty giả lập duy nhất để chạy thử toàn bộ 21 skill mà không phải tự nghĩ dữ liệu mới cho từng video.

**Công ty demo:** FlowNest Systems  
**Sản phẩm demo:** FlowNest WMS — phần mềm quản lý kho cho nhà phân phối và 3PL tại Việt Nam.

## Thứ tự nạp vào Project

1. [Business Context Card](01-business-context-card.md) — nguồn bối cảnh chung.
2. [Evidence Ledger](02-evidence-ledger.md) — dữ kiện, quote và giới hạn độ tin cậy.
3. [Assumption Log](03-assumption-log.md) — điều đang giả định, chưa phải sự thật.
4. [Decision Records](04-decision-records.md) — quyết định đã duyệt cho demo.
5. [Handoff Packets](05-handoff-packets.md) — cách chuyển đầu ra giữa các skill.
6. [Lead Account](06-lead-account.md) — input cho Lead Research đến Proposal.
7. [Sales Call Transcript](07-sales-call-transcript.md) — input cho Discovery và Objection Handling.
8. [Pipeline Snapshot](08-pipeline-snapshot.md) — input cho Pipeline Review và Sales Manager.
9. [Content & Campaign Brief](09-content-campaign-brief.md) — input cho Content và Campaign skills.

## Cách dùng trong từng chat

Mở một chat mới theo đúng một công việc, rồi dán prompt sau và thay mã skill:

```text
Dùng $smos-XX-ten-skill.

Đây là dữ liệu DEMO ONLY. Dùng các object sau làm nguồn:
- BCC: demo/01-business-context-card.md
- EL: demo/02-evidence-ledger.md
- AL: demo/03-assumption-log.md
- DR/HP: [chọn object liên quan]

Quyết định cần hỗ trợ: [một câu hỏi cụ thể]
Đầu ra mong muốn: [artifact + định dạng]
Không bịa nguồn hoặc số liệu ngoài các object. Tách Fact / Evidence / Hypothesis / Recommendation.
```

## Luồng demo đề xuất

```text
01 ICP → 04 VOC → 05 Positioning → 06 Offer
       → 07 Content Strategy → 10 Campaign → 11 Lead Magnet
       → 12 Lead Research → 13 Qualification → 14 Outreach
       → 16 Call Prep → 17 Discovery → 19 Objection
       → 18 Proposal → 20 Pipeline → 21 Sales Manager
```

Có thể dùng 02 Market Research và 03 Competitor Research trước 05; dùng 08 Content Creator và 09 Repurposing sau 07.

## Quy tắc object

- Giữ nguyên `object_id`, ngày và version khi quay lại cùng một demo.
- Nếu sửa dữ liệu, tạo version mới; không âm thầm ghi đè.
- `synthetic` nghĩa là dữ liệu sinh để demo, không phải bằng chứng thị trường.
- Khi skill thiếu dữ liệu, để **Chưa biết** và ghi cách kiểm chứng.
