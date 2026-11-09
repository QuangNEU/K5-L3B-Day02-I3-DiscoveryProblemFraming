# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

```text
    HIỆN TẠI — riêng thời gian chờ khoảng 20 phút/lượt (ước lượng)

    [1 Đến điểm đón E03: ? phút]

    → [2 Chờ xe, lướt điện thoại: khoảng 20 phút] ← BOTTLENECK: chưa biết mức đông
    
    → [3 Quan sát khi xe đến và lên xe: ? phút]

    ? phút = chưa đo riêng; 20 phút không phải tổng thời gian của toàn bộ hành trình.
    Chưa xác nhận việc bỏ chuyến đông để chờ chuyến sau.
```

| Bước | Actor                    | Input                                              | Output                                    | Thời gian / tần suất | Ghi chú                                                       |
| ---- | ------------------------ | -------------------------------------------------- | ----------------------------------------- | -------------------- | ------------------------------------------------------------- |
| 1    | Hành khách               | Đến điểm đón E03                                   | Có mặt tại điểm đón, sẵn sàng chờ xe      | Ngay khi đến         | Cần xác định đúng vị trí đón                                  |
| 2    | Hành khách               | Thời gian chờ xe, điện thoại cá nhân               | Tiếp tục chờ xe, theo dõi thời gian       | Khoảng 20 phút       | Bottleneck: Chưa biết mức độ đông đúc và thời gian xe đến     |
| 3    | Hành khách               | Xe đã đến, xác nhận đúng tuyến                     | Lên xe thành công                         | ? phút               | Phụ thuộc vào số lượng người lên xe và tình trạng xếp hàng    |

**Bottleneck**: Hành khách thiếu thông tin theo thời gian thực về thời gian xe đến và mức độ đông đúc tại điểm đón E03, dẫn đến thời gian chờ không chắc chắn và trải nghiệm di chuyển kém thuận tiện.

### 4.2. Quy trình tương lai

```text
    TƯƠNG LAI — 5 bước, khoảng 5 phút, 2/5 bước thủ công

    [1 Hành khách mở ứng dụng, chọn điểm đón E03: 1 phút] ← RULE (GPS / định vị)

    → [2 AI dự đoán thời gian xe đến (ETA): 5 giây] ← AI (GPS + dữ liệu giao thông)

    → [3 AI dự đoán mức độ đông đúc tại điểm đón: 2 phút] ← AI (dữ liệu hành khách + lịch sử)

    → [4 Ứng dụng hiển thị ETA, mức độ đông đúc và gửi thông báo: 1 phút] ← AI + RULE (cập nhật thông tin, thông báo tự động)

    → [5 Hành khách xác nhận đúng xe và lên xe: ? phút] ← CON NGƯỜI

    BOUNDARY: AI chỉ dự đoán thời gian xe đến và mức độ đông đúc dựa trên dữ liệu được cung cấp. AI không điều khiển xe, không đảm bảo còn chỗ và không tự quyết định việc lên xe thay hành khách.

    PHƯƠNG ÁN QUAY VỀ: Nếu AI không dự đoán được hoặc dữ liệu không chính xác → Ứng dụng hiển thị lịch trình xe và thông tin thời gian dự kiến theo phương pháp truyền thống; hành khách tự quan sát và chờ xe.

    Lưu ý: Tổng thời gian trên là mục tiêu thiết kế sơ bộ, chưa phải số liệu đo lường thực tế.
```

### 4.3. Before / after

| Chỉ số               | Trước                                                     | Sau (kỳ vọng)                                                        | Ghi chú                                                               |
| -------------------- | --------------------------------------------------------- | -------------------------------------------------------------------- | --------------------------------------------------------------------- |
| Số bước              | 3                                                         | 5                                                                    | Quy trình được bổ sung các bước dự đoán và cung cấp thông tin bằng AI |
| Tổng thời gian       | Khoảng 20 phút chờ xe + thời gian di chuyển đến và lên xe | Khoảng 6 phút xử lý trên ứng dụng + thời gian di chuyển và lên xe    | Thời gian chờ thực tế có thể giảm nhờ chủ động lựa chọn thời điểm     |
| Số bước thủ công     | 3/3                                                       | 1/5                                                                  | Hành khách vẫn tự xác nhận xe và lên xe                               |
| Bottleneck chính     | Không biết thời gian xe đến và mức độ đông đúc            | Độ chính xác của dữ liệu GPS và mô hình dự đoán                      | Phụ thuộc vào chất lượng và tính cập nhật của dữ liệu                 |
| Rủi ro mới phát sinh | Chờ xe lâu, không biết tình trạng đông đúc                | AI dự đoán sai ETA hoặc mức độ đông đúc, dữ liệu GPS không chính xác | Cần có phương án dự phòng khi AI hoạt động không hiệu quả             |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Hành khách đi E03 buổi sáng |
| **Quy trình** | [1 Đến điểm đón E03: ? phút] → [2 Chờ xe, lướt điện thoại: khoảng 20 phút] ← BOTTLENECK: chưa biết mức đông → [3 Quan sát khi xe đến và lên xe: ? phút] |
| **Bottleneck** | Không biết thời gian xe đến và mức độ đông đúc |
| **Impact** | Đứng chờ xe mất 20 phút |
| **Success Metric** (baseline → target, cách đo) | Thời gian chờ 20 phút, mong muốn đạt 5 phút, đo bằng cách bắt đầu từ thời điểm chờ xe |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI chỉ dự đoán thời gian xe đến và mức độ đông đúc dựa trên dữ liệu được cung cấp. AI không điều khiển xe, không đảm bảo còn chỗ và không tự quyết định việc lên xe thay hành khách. |

**Phản biện nhận được**: Tại sao phải sử dụng AI thay vì thuật toán tính toán ETA thông thường? Nhóm không đồng ý, AI có thể xem được rất nhiều yếu tố để có thể đưa ra tính toán gần chính xác hơn

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
