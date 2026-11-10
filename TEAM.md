# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: I3
- Candidate problem nhóm chọn (1 câu): Tối ưu việc chọn xe bus theo
- Quyết định cuối (Go / Not Yet / No-Go):

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 |Nguyễn Minh Quang |2A202603791 |Phụ trách research, ghi chép |https://github.com/QuangNEU |
| 2 |Nguyễn Nhật Minh |2A202603745 |phụ trách kiểm chứng (phỏng vấn/survey), ghi chép  |https://github.com/NhMinh-2610 |
| 3 |Hoàng Đức An |2A202603800 |phụ trách kiểm chứng (phỏng vấn/survey), ghi chép |https://github.com/katogithub2701 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm |Minh |Quang | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng |Minh |An | Assumption map, snapshot hoặc survey |
| CP4 — Research |Quang |Minh | Bảng research có link |
| CP5 — Quy trình trước/sau |An |Minh | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 |An |Quang | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 |Quang |An | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định |Quang |Minh | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### Nguyễn Minh Quang - 2A202603791

**Phần việc phụ trách:**
Phân tích và chọn candidate (mục 2.2 - 2.4), research giải pháp đã có (mục 3.3),
và xác định mức can thiệp AI cho bài toán E03 (mục 6 - 8). [Xóa dòng nào bạn không làm]

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Gom 9 candidate thành 3 cluster (Tóm tắt & Rút trích / Đưa ra quyết định & So sánh /
  Đối chiếu & Phân loại dữ liệu) và chỉ ra pattern chung của từng cluster.
- Chấm điểm shortlist theo 7 tiêu chí (thang 1-5). Bài E03, Thủ quỹ và Tóm tắt tài liệu
  cùng đạt 34 điểm; nhóm chọn E03 và mình viết phần lý do chọn/loại.
- Đề xuất hướng dùng Mock Data (dữ liệu tap-in giả lập) để giải rủi ro Feasibility
  khi nhóm e ngại thiếu API dữ liệu thật.
- Research 3 giải pháp hiện có (Google Maps/Moovit, VinBus/Tìm Buýt, ML ước lượng
  khách xuống xe) và rút kết luận: thị trường đã giải GPS, còn thiếu khâu đo đếm
  và dự đoán độ đông.
- So sánh 4 mức No AI / Rule / Workflow / Agent, chọn Workflow (Rule gom log
  + ML nội suy số khách xuống), và viết AI Canvas.
- Viết Problem Statement v1, 3 tiêu chí đánh giá đầu ra, đánh giá 4 rủi ro,
  quyết định Go (pilot nhỏ) kèm ngưỡng dừng quay về Rule.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- `group_report.md`: mục 2.2, 2.4, 3.3, 6.1 - 6.4, 7, 8, 9, 10


**Điều mình học được từ phần nhóm:**
- Học được cách làm việc nhóm và quản lý git
- Cách trao đổi phản biện và đưa ra ý tưởng