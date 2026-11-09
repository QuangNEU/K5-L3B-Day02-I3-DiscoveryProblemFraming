# Báo cáo cá nhân — MSSV_HoTen

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Hoàng Đức An
- MSSV: 2A202603800
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: K3
- Link repo nhóm: https://github.com/QuangNEU/K5-L3B-Day02-K3-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Lặp lại |Khi hoàn thành buổi họp, tôi muốn hệ thống tự động tổng hợp toàn bộ buổi họp để tôi không bị quên nội dung và tiết kiếm thời gian xem lại buổi họp |CEO, Nhân viên văn phòng |Khảo sát 20 nhân viên, có 13 nhân viên chỉ nhớ 50% nội dung buổi họp, tốn khoảng 40 phút để xem lại nội dung họp |
| 2 |Tốn thời gian |Khi hoàn thành xong bài tập, tôi muốn hệ thống tổng hợp các câu hỏi sai và đưa ra các kiến thức liên quan để tôi củng cố lại kiến thức |Học sinh, sinh viên |Mất 15 phút để xem câu sai và tìm kiến thức |
| 3 |Lặp lại |Khi tìm quán ăn, tôi muốn hệ thống tổng hợp các đánh giá của quán ăn đó để tôi biết quán nào nên ăn |Người dùng muốn tìm quán ăn |Mất 10 phút/quán |
| 4 |Lặp lại |Khi có khách hàng gửi yêu cầu hỗ trợ, tôi muốn hệ thống tự phân loại và chuyển đúng bộ phận, để giảm thời gian xử lý thủ công |CSKH, quản lý dịch vụ |Kiểm tra 100 ticket gần nhất, có 40 ticket phải chuyển bộ phận thủ công |
| 5 |Tốn thời gian |Khi cần tìm căn hộ phù hợp với khách hàng, tôi muốn hệ thống đề xuất các căn đáp ứng vị trí, giá tiền và tiện ích, để không phải lọc thủ công từng căn |Người muốn tìm căn hộ |Mất 5 phút để lọc và tìm ra 3 căn phù hợp |
| 6 |Cần đọc và tổng hợp nhiều thông tin |Khi cần đánh giá hiệu quả kinh doanh, tôi muốn hệ thống tổng hợp doanh thu, chi phí, khách hàng và hiệu suất từ nhiều nguồn dữ liệu, để nhanh chóng xác định vấn đề |Giám đốc kinh doanh, chuyên viên phân tích |Kiểm tra 10 báo cáo gần nhất, thống kê có 2 báo cáo phải chỉnh sửa hoặc yêu cầu bổ sung |


**Nếu có dùng AI để gợi ý thêm:** Sau khi tự scan 5 ý, mình hỏi AI và giữ lại ý 6

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |Tóm tắt nội dung họp (#1) |Tốn thời gian, nhiều người gặp |Chi phí triển khai và tính bảo mật |
| 2 |Phân loại yêu cầu người dùng (#4) |Pain thật, tính ứng dụng cao |Chi phí so với quy trình thông thường |
| 3 |Tìm căn hộ (#5) |Pain thật, nhiều người gặp |Chi phí triển khai |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi hoàn thành buổi họp, tôi muốn hệ thống tự động tổng hợp toàn bộ buổi họp để tôi không bị quên nội dung và tiết kiếm thời gian xem lại buổi họp |
| Actor |CEO, Nhân viên văn phòng |
| Thời điểm / bối cảnh |Sau các cuộc họp dự án, họp sprint, họp giao ban hoặc họp với khách hàng. |
| Quy trình hiện tại (3–7 bước) |Ghi âm buổi họp -> Mở lại bản ghi -> Nghe và tổng hợp nội dung |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2-3 Nghe lại bản ghi, đọc ghi chú và xác định action item. Ước tính 30–60 phút cho mỗi cuộc họp.|
| Impact (nếu không giải thì sao) |Tốn thời gian của nhân viên; bỏ sót đầu việc; nhầm người phụ trách; chậm tiến độ do các thành viên không nắm rõ quyết định sau cuộc họp. |
| Success metric (baseline → target) |Thời gian làm biên bản: 30–60 phút → dưới 10 phút. Tỷ lệ đầu việc được ghi nhận đầy đủ: đo baseline → mục tiêu trên 95%. |
| Phương án không dùng AI |	Sử dụng mẫu biên bản họp chuẩn; phân công một người ghi chép; sử dụng công cụ ghi âm và checklist action item. |
| Giả thuyết về AI (nếu có) |Sử dụng Speech-to-Text để chuyển giọng nói thành văn bản, kết hợp LLM để tóm tắt nội dung, trích xuất quyết định, người phụ trách và deadline; tự động tạo biên bản họp. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
    Ghi âm buổi họp -> Sử dụng AI Speech-to-text để lấy nội dung -> Dùng LLM để tổng hợp nội dung
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi có khách hàng gửi yêu cầu hỗ trợ, tôi muốn hệ thống tự phân loại và chuyển đúng bộ phận, để giảm thời gian xử lý thủ công |
| Actor |CSKH, quản lý dịch vụ   |
| Thời điểm / bối cảnh |Khi khách hàng gửi yêu cầu qua hotline, email, chatbot, website hoặc ứng dụng chăm sóc khách hàng. |
| Quy trình hiện tại (3–7 bước) |Tiếp nhận yêu cầu từ khách hàng. -> Đọc nội dung và xác định vấn đề. -> Phân loại yêu cầu (kỹ thuật, thanh toán, bảo hành, khiếu nại...). -> Chuyển yêu cầu đến bộ phận phụ trách. |
| Bottleneck (bước nào, mất bao nhiêu phút) |Bước 2-3, mất 5 phút/yêu cầu |
| Impact (nếu không giải thì sao) |Phản hồi khách hàng chậm; chuyển nhầm bộ phận |
| Success metric (baseline → target) |Thời gian phân loại ticket: 5–15 phút → dưới 2 phút, Tỷ lệ phân loại đúng: đo baseline → mục tiêu trên 90%, Thời gian phản hồi đầu tiên: đo baseline → giảm ít nhất 30%. |
| Phương án không dùng AI |Xây dựng bộ quy tắc phân loại ticket; tạo biểu mẫu yêu cầu chuẩn;|
| Giả thuyết về AI (nếu có) |Sử dụng LLM/NLP để hiểu ngôn ngữ tự nhiên, tự động phân loại ticket, nhận diện mức độ ưu tiên, tìm kiếm thông tin trong kho tri thức và đề xuất câu trả lời cho nhân viên CSKH. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
    Nhận yêu cầu khách hàng -> Đưa cho mô hình phân loại -> Đưa yêu cầu tới bên liên quan
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi có nhu cầu mua hoặc thuê căn hộ, tôi muốn tìm được những căn phù hợp với ngân sách, vị trí, diện tích và tiện ích mong muốn, để không phải tự tìm kiếm và so sánh hàng trăm căn hộ. |
| Actor | Người mua nhà |
| Thời điểm / bối cảnh | Khi khách hàng bắt đầu tìm kiếm căn hộ, có nhu cầu so sánh các dự án hoặc muốn tìm căn phù hợp với khả năng tài chính. |
| Quy trình hiện tại (3–7 bước) | Khách hàng xác định nhu cầu -> Lọc căn hộ -> Kiểm tra tình trạng căn hộ còn bán hoặc cho thuê. -> In danh sách căn hộ cho khách hàng.|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 - 3 Lọc căn hộ, khoảng 5 phút/lần |
| Impact (nếu không giải thì sao) | Khách hàng mất nhiều thời gian tìm nhà |
| Success metric (baseline → target) | Thời gian tìm 3–5 căn phù hợp: 20–45 phút → dưới 5 phút. |
| Phương án không dùng AI | Xây dựng bộ lọc tìm kiếm nâng cao theo giá, vị trí, diện tích, số phòng ngủ, tiện ích và trạng thái căn hộ |
| Giả thuyết về AI (nếu có) | Dùng LLM để hiểu nhu cầu bằng ngôn ngữ tự nhiên, chuyển thành bộ tiêu chí tìm kiếm, đề xuất căn hộ phù hợp và giải thích lý do đề xuất. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
    Nhận yêu cầu -> đưa yêu cầu cho LLM hiểu -> Chuyển thành bộ lọc tìm kiếm -> In ra danh sách căn hộ
```

### Card muốn pitch nhất

- Card số:
- Vì sao:
- Câu hỏi muốn nhóm phản biện:

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
