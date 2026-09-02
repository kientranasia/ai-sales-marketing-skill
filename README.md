# AI cho Sales & Marketing — Hệ thống AI thực dụng cho doanh nghiệp tăng trưởng

## Bộ tài sản tiếng Việt

Bộ này gồm 21 tutorial Markdown độc lập, 21 skill production-ready và README kiến trúc. Mỗi tutorial có mục đích, đầu vào, setup, hướng dẫn từng bước, system instructions, prompt mẫu, output schema, test case, checklist, lỗi thường gặp, tùy chỉnh, mở rộng và kịch bản quay video.

Các skill vẫn giữ mã gọi tiếng Anh như `$smos-01-icp-builder` để dễ dùng trong mọi workspace; phần giải thích, instructions, prompt và metadata đã chuyển sang tiếng Việt.

## Kiến trúc OS

~~~text
NỀN TẢNG                 CHIẾN LƯỢC              TẠO NHU CẦU               VẬN HÀNH DOANH THU
01 ICP Builder ──────┐   05 Positioning ─────┐   07 Content Strategy ──┐  12 Lead Research
02 Market Research ─┼──▶06 Offer Builder ───┼──▶08 Content Creator     ├─▶13–15 Qualify/Engage
03 Competitors ─────┤                         │   09 Repurposing         │  16–19 Sell/Advance
04 Customer/VOC ────┘                         └──▶10 Campaign ──────────┤  20 Pipeline Review
                                                  11 Lead Magnet ───────┘  21 Sales Manager
~~~

Luồng không hoàn toàn tuyến tính. Research làm mới strategy; sales call tạo VOC mới; pipeline có thể khiến ICP và offer thay đổi. Handoff Packet giúp mỗi chat không phải bắt đầu từ số 0.

## Năm object dùng chung

1. **Business Context Card (BCC):** công ty, sản phẩm, economics, thị trường, ICP, mục tiêu, giới hạn, voice, proof đã duyệt và claim cấm.
2. **Evidence Ledger (EL):** source ID, loại, tiêu đề, owner, ngày, link/vị trí, excerpt/field, độ tin cậy và ghi chú bảo mật.
3. **Assumption Log (AL):** assumption ID, lý do, rủi ro nếu sai, cách kiểm chứng, owner, hạn và trạng thái.
4. **Decision Record (DR):** quyết định, phương án, bằng chứng, lý do, người duyệt, ngày và trigger review.
5. **Handoff Packet (HP):** context ngắn đã duyệt để chuyển sang skill kế tiếp; không thêm phân tích mới.

## Quy ước đặt tên

- Skill: `SMOS-## Tên skill`
- Artifact: `SMOS-##-short-name-YYYY-MM-DD-v#`
- Evidence: `EL-[source]-###`
- Assumption: `AL-###`
- Decision: `DR-YYYYMMDD-##`
- Test: `T-SMOS-##-A/B`

## Thứ tự triển khai

### MVP

01 ICP Builder → 04 Customer/VOC → 05 Positioning → 06 Offer → sau đó chọn 07–10 cho marketing hoặc 12–18 cho sales. Thêm 20–21 khi đã có pipeline thật.

### Lộ trình đầy đủ

- **Giai đoạn 1 — Hiểu:** 01–04.
- **Giai đoạn 2 — Quyết định:** 05–06.
- **Giai đoạn 3 — Tạo nhu cầu:** 07–11.
- **Giai đoạn 4 — Chuyển đổi:** 12–19.
- **Giai đoạn 5 — Điều hành:** 20–21.

## Cách dùng

1. Đọc phần mục đích và xác nhận skill phù hợp với quyết định hiện tại.
2. Chuẩn bị đầu vào tối thiểu và Handoff Packet upstream.
3. Gọi skill bằng `$smos-...` hoặc dán instructions vào chat mới.
4. Chạy prompt ví dụ trước khi dùng dữ liệu thật.
5. Chạy hai test case.
6. Review Quality Checklist và duyệt artifact.
7. Lưu Handoff Packet có ngày và phiên bản.

## Danh sách 21 tutorial

| # | Tutorial | Lớp | Kết quả chính |
|---:|---|---|---|
| 01 | [ICP Builder — Xây dựng ICP](01-icp-builder.md) | Nền tảng | thẻ ICP chính và phụ |
| 02 | [Market Research — Nghiên cứu thị trường](02-market-research.md) | Nền tảng | bản đồ thị trường và động lực |
| 03 | [Competitor Research — Nghiên cứu đối thủ](03-competitor-research.md) | Nền tảng | bản đồ lựa chọn thay thế |
| 04 | [Customer Research & VOC — Nghiên cứu khách hàng](04-customer-research-voc.md) | Nền tảng | chủ đề đã mã hóa và tần suất |
| 05 | [Positioning & Messaging — Định vị và thông điệp](05-positioning-messaging.md) | Chiến lược | positioning statement |
| 06 | [Offer Builder — Xây dựng offer](06-offer-builder.md) | Chiến lược | kiến trúc và phạm vi offer |
| 07 | [Content Strategy — Chiến lược nội dung](07-content-strategy.md) | Tạo nhu cầu | content thesis, pillar và hành trình audience |
| 08 | [Content Creator — Sáng tạo nội dung](08-content-creator.md) | Tạo nhu cầu | các angle và lý do chọn |
| 09 | [Content Repurposing — Tái sử dụng nội dung](09-content-repurposing.md) | Tạo nhu cầu | bản đồ insight nguồn |
| 10 | [Campaign Builder — Xây dựng chiến dịch](10-campaign-builder.md) | Tạo nhu cầu | campaign brief và customer journey |
| 11 | [Lead Magnet Builder — Xây dựng lead magnet](11-lead-magnet-builder.md) | Tạo nhu cầu | khái niệm và promise lead magnet |
| 12 | [Lead Research — Nghiên cứu lead](12-lead-research.md) | Vận hành doanh thu | fact về account và source log |
| 13 | [Lead Qualification — Đánh giá lead](13-lead-qualification.md) | Vận hành doanh thu | điểm theo chiều kèm bằng chứng |
| 14 | [Outreach — Tiếp cận](14-outreach.md) | Vận hành doanh thu | lý do chọn angle |
| 15 | [Follow-up — Theo đuổi cơ hội](15-follow-up.md) | Vận hành doanh thu | chẩn đoán trạng thái |
| 16 | [Sales Call Prep — Chuẩn bị cuộc gọi sales](16-sales-call-prep.md) | Vận hành doanh thu | call brief một trang |
| 17 | [Discovery Analysis — Phân tích discovery](17-discovery-analysis.md) | Vận hành doanh thu | tóm tắt fact/evidence |
| 18 | [Proposal Builder — Xây dựng proposal](18-proposal-builder.md) | Vận hành doanh thu | narrative và executive summary |
| 19 | [Objection Handling — Xử lý phản đối](19-objection-handling.md) | Vận hành doanh thu | chẩn đoán objection và độ tin cậy |
| 20 | [Pipeline Review — Rà soát pipeline](20-pipeline-review.md) | Vận hành doanh thu | tóm tắt pipeline và weighted view |
| 21 | [Sales Manager — Điều hành đội sales](21-sales-manager.md) | Vận hành doanh thu | narrative performance cho lãnh đạo |

## Nguyên tắc vận hành

- Bằng chứng trước văn phong.
- Quyết định trước deliverable.
- Một nguồn sự thật có version.
- Con người duyệt claim, message, giá, proposal, forecast và external action.
- Chỉ dùng dữ liệu cá nhân ở mức cần thiết.
- Ổn định workflow thủ công trước khi tự động hóa.
- Đưa win, loss, reply, conversion và objection quay lại Research, ICP, Positioning và Offer.

## Mức mở rộng integration

1. Chat + file native.
2. Web research có nguồn và ngày.
3. App/plugin được duyệt.
4. n8n/no-code cho intake, routing và review queue.
5. API/product workflow có permission, logging, eval và monitoring.

External write, gửi message, đặt lịch, sửa CRM và automation phải có approval gate rõ ràng.

## Tách Tutorial và Production

Project tutorial dùng công ty giả và dữ liệu mẫu. Project production dùng Business Context Card thật và chat theo từng công việc cụ thể. Không đưa dữ liệu khách hàng thật vào project quay video.
