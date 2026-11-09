# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Phạm vi phát triển hướng tới: Tất cả các tuyến xe buýt và các khung giờ di chuyển.
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Nhật Minh | Khi chờ xe buýt, tôi muốn biết mức đông của các chuyến phù hợp với hành trình để chủ động chọn chuyến trong thời gian có thể chờ. | Hành khách trên các tuyến xe buýt, trong đó có Minh. | Bước chờ xe chưa có thông tin về mức đông của các chuyến. Trong trải nghiệm của Minh trên E03, thời gian chờ khoảng 20 phút; chưa tách được thời gian phát sinh do lựa chọn chuyến. | Bạn đã từng bỏ chuyến đông để chờ chuyến sau chưa? Nếu có thông tin về độ đông, bạn sẵn sàng chờ thêm bao lâu? **Người hỏi:**  Nguyễn Minh Quang |
| 2 | Nguyễn Nhật Minh | Khi cân nhắc 2 phòng trọ đã biết giá và các khoản phí, tôi muốn so sánh tổng chi phí hằng tháng để chọn phòng phù hợp ngân sách. | Người tìm phòng trọ, trong đó có Minh. | Bước ước tính và quy đổi các khoản phí thành tổng chi phí có thể so sánh; toàn bộ quá trình khoảng 5 phút, chưa đo riêng bước này. | Bước nào khiến bạn khó tính nhất? **Người hỏi:** Nguyễn Minh Quang |
| 3 | Nguyễn Nhật Minh | Khi thu quỹ lớp qua chuyển khoản, tôi muốn xác định đúng người đóng từng khoản để ghi nhận chính xác và hạn chế hỏi lại. | Thủ quỹ lớp và các thành viên đóng quỹ. | Bước tìm và xác minh tên người đóng khi giao dịch thiếu họ tên. Lần thu của Minh mất khoảng 120 phút tổng cộng; phần dò tên/hỏi lại nằm trong khoảng 60 phút cuối, chưa tách thời gian riêng. | Trong lần thu gần nhất, có bao nhiêu khoản thiếu tên và bạn đã xác minh người gửi như thế nào để tránh ghi nhầm? **Người hỏi:**  Hoàng Đức An |
| 4 | Nguyễn Minh Quang | Khi nhận tài liệu môn học hoặc requirement đồ án dài, tôi muốn nắm ý chính và các phần việc cần làm để hiểu yêu cầu và phân công công việc. | Sinh viên CNTT hoặc trưởng nhóm đồ án. | Bước đọc chi tiết và trích xuất yêu cầu từ tài liệu dài 10–20 trang, khoảng 45 phút. | Bạn kiểm tra thế nào để không bỏ sót yêu cầu? **Người hỏi:** Nguyễn Nhật Minh |
| 5 | Nguyễn Minh Quang | Khi xử lý lỗi liên quan đến luồng dữ liệu realtime, tôi muốn đối chiếu log backend từ nhiều nguồn để tìm nguyên nhân nhanh hơn. | Lập trình viên backend. | Bước dò timestamp và so khớp sự kiện giữa các nguồn log thủ công, khoảng 25 phút. | Gom log theo timestamp đã đủ để tìm lỗi chưa? **Người hỏi:** Hoàng Đức An |
| 6 | Nguyễn Minh Quang | Khi nghe podcast về System Design trên đường đi, tôi muốn ghi lại các từ khóa và kiến trúc chính để ôn tập mà không phải tua lại nhiều lần. | Sinh viên CNTT tự học qua podcast. | Bước nhớ lại nội dung và tua lại đoạn audio đã quên, khoảng 25 phút. | Bạn làm sao để ghi đủ các ý quan trọng? **Người hỏi:** Nguyễn Nhật Minh |
| 7 | Hoàng Đức An | Khi kết thúc buổi họp, tôi muốn nắm các nội dung chính và đầu việc để không quên nội dung và giảm thời gian xem lại. | CEO và nhân viên văn phòng tham gia cuộc họp. | Bước nghe lại bản ghi, đọc ghi chú và xác định đầu việc sau họp, ước tính khoảng 30–60 phút/cuộc họp. | Ai kiểm tra lại các đầu việc sau họp? **Người hỏi:** Nguyễn Minh Quang |
| 8 | Hoàng Đức An | Khi khách hàng gửi yêu cầu hỗ trợ, tôi muốn xác định đúng loại yêu cầu và bộ phận phụ trách để giảm thời gian xử lý thủ công. | Nhân viên chăm sóc khách hàng và quản lý dịch vụ. | Bước đọc, xác định vấn đề và phân loại yêu cầu, khoảng 5 phút/yêu cầu theo Problem Card. | Có bao nhiêu ticket bị chuyển sai bộ phận? **Người hỏi:** Nguyễn Nhật Minh |
| 9 | Hoàng Đức An | Khi cần mua hoặc thuê căn hộ, tôi muốn tìm những căn phù hợp ngân sách, vị trí, diện tích và tiện ích để giảm công sức tìm kiếm và so sánh. | Người tìm mua hoặc thuê căn hộ. | Bước lọc căn hộ và kiểm tra tình trạng còn bán hoặc cho thuê, khoảng 5 phút/lần theo phần bottleneck của Problem Card. | Mốc 5 phút và 20–45 phút khác nhau thế nào? **Người hỏi:** Nguyễn Minh Quang |


### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Tăng tỷ lệ lượt đi xe buýt mà hành khách chọn được chuyến có mức đông phù hợp trong thời gian có thể chờ.
├── Opportunity: Hành khách chưa biết mức đông của chuyến xe trước khi xe đến điểm đón.
├── Opportunity: Khó cân nhắc lên chuyến hiện tại hay chờ chuyến sau khi chưa biết mức đông của chuyến sau.
└── Opportunity: Hành khách cần chọn chuyến phù hợp với khoảng thời gian có thể chờ.
```

Baseline cần được ghi nhận theo tuyến và khung giờ; mức đông được xem là phù hợp cần được làm rõ khi kiểm chứng.

Ví dụ giải pháp không đưa vào các nhánh opportunity: ứng dụng hiển thị độ đông, AI dự báo số hành khách.

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
| 1 | Hành khách trên các tuyến xe buýt thường gặp chuyến đông và xem đây là khó khăn đáng giải quyết. | Value | 5 | 2 | Có — hỏi thêm hành khách ở nhiều tuyến, khung giờ và ghi nhận số lần gặp xe đông. |
| 2 | Biết mức đông trước có thể giúp hành khách điều chỉnh giờ đi hoặc cân nhắc chuyến khác trong thời gian có thể chờ. | Value | 5 | 2 | Có — kiểm tra hành vi thực tế, không chỉ hỏi ý định. |
| 3 | Có thể tiếp cận dữ liệu mức đông của từng chuyến trên các tuyến xe buýt trước khi xe đến điểm đón. | Feasibility | 5 | 1 | Có — kiểm tra ứng dụng hiện có, nguồn dữ liệu từ các đơn vị vận hành và mức độ bao phủ tuyến. |
| 4 | Thông tin mức đông có thể đủ chính xác và cập nhật kịp thời để hành khách lựa chọn. | Feasibility | 5 | 1 | Có — so sánh thông tin hiển thị với quan sát trên các chuyến thực tế. |
| 5 | Hành khách hiểu và sử dụng được các mức đông/vắng trước khi quyết định lên xe. | Usability | 3 | 1 | Kiểm tra sau khi có cách trình bày thông tin để thử. |
| 6 | Việc thu thập, chia sẻ và duy trì dữ liệu có thể thực hiện phù hợp với quyền truy cập và chi phí. | Viability | 4 | 1 | Có — xác minh quyền sử dụng dữ liệu và cách vận hành với nguồn cung cấp. |

*Điểm quan trọng và bằng chứng là đánh giá sơ bộ để nhóm thảo luận: 1 = thấp/ít bằng chứng, 5 = cao/nhiều bằng chứng.*

**Giả định đã thăm dò:** #1 và #2 qua quan sát của một thành viên đi E03 và trao đổi với 2 sinh viên đi xe buýt. Chưa ghi rõ tuyến của hai sinh viên; một người nêu ý định đi sớm, chưa có bằng chứng đã thực sự đổi giờ đi. Các giả định #3–#6 chưa được kiểm chứng trên các tuyến xe buýt trong phạm vi hướng tới.

### 3.2. Kiểm chứng

**Cách kiểm chứng:** Ngày 09/11/2026, nhóm hỏi trực tiếp trên lớp 2 sinh viên ngoài nhóm thường đi xe buýt đến trường. Nhóm cũng ghi nhận trải nghiệm đi E03 của một thành viên.

**Interview Snapshot 1**

| Trường | Nội dung |
|---|---|
| Người được hỏi | Sinh viên ngoài nhóm, đi xe buýt đến trường; chưa ghi rõ tuyến xe. |
| Thời điểm và cách hỏi | Ngày 09/11/2026, hỏi trực tiếp trên lớp. |
| Lần gần nhất | Chuyến xe bạn đi rất đông. |
| Cách xử lý | Vẫn lên xe vì không chắc chuyến sau có vắng hơn. Bạn chủ động căn thời gian ra điểm đón để không phải đợi lâu. |
| Ý chính | Bạn không biết chuyến sau có đông hay không.  |
| Insight | Thiếu thông tin về chuyến sau khiến bạn khó cân nhắc giữa lên xe đông và tiếp tục chờ. |

**Interview Snapshot 2**

| Trường | Nội dung |
|---|---|
| Người được hỏi | Sinh viên ngoài nhóm, đi xe buýt đến trường; chưa ghi rõ tuyến xe. |
| Thời điểm và cách hỏi | Ngày 09/11/2026, hỏi trực tiếp trên lớp. |
| Mức độ quan tâm | Bạn quan tâm xe có đông hay không và muốn biết trước mức độ đông. |
| Ý kiến | Bạn nói sẵn sàng đi sớm nếu biết có chuyến vắng hơn. |
| Lần gần nhất / thời gian chờ | Đi sáng nay/không cần đợi vì căn được giờ. |
| Insight | Thông tin về độ đông có thể giúp hành khách cân nhắc điều chỉnh giờ đi. |

**Tổng hợp:**

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Quan sát của thành viên đi E03 | 1 thành viên | Có chuyến đông và chuyến sau vắng hơn; chưa biết trước mức đông khi chờ xe. Thời gian chờ thường khoảng 20 phút theo ước lượng. | Chưa đủ bằng chứng kết luận thời gian chờ là do thiếu thông tin về độ đông. |
| Phỏng vấn trực tiếp trên lớp | 2 sinh viên ngoài nhóm | Một bạn không biết chuyến sau có vắng hơn không; bạn còn lại quan tâm độ đông và muốn biết trước. | Một bạn vẫn lên xe đông; bạn còn lại căn được giờ nên không phải đợi. Đây là tín hiệu cần xem lại mục tiêu giảm thời gian chờ; chưa đủ cơ sở kết luận họ sẽ chờ thêm để đi chuyến vắng. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Nhóm tập trung vào việc hành khách chưa biết trước mức đông của các chuyến xe buýt phù hợp với hành trình, nên khó chủ động chọn chuyến trong thời gian có thể chờ. Bài toán hướng tới tất cả các tuyến xe buýt. Phản hồi cho thấy cần xem xét cả việc điều chỉnh giờ đi, bên cạnh quyết định lên xe hay chờ chuyến sau.

**Cần hoàn thiện:** Bổ sung kiểm chứng ở nhiều tuyến và khung giờ, ghi rõ tuyến xe, thời gian chờ và tần suất gặp chuyến đông của từng người. Cần kiểm chứng thêm hành vi lựa chọn chuyến, điều chỉnh giờ đi và ghi tín hiệu phản bác nếu có. Dữ liệu hiện tại là bằng chứng ban đầu, chưa đủ để kết luận mức độ phổ biến của vấn đề trên tất cả các tuyến.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| BusMap | [Các tính năng](https://busmap.vn/tinh-nang/); [FAQ](https://busmap.vn/faq/) | Tra cứu tuyến và thời gian xe đến trước khi lên xe. | Trang tính năng mô tả lịch tuyến và thời gian chờ dựa trên GPS; FAQ nêu cách xem xe tại trạm. | Các trang đã đọc chưa mô tả mức đông theo từng chuyến; chưa kiểm tra trực tiếp mức độ hỗ trợ các tuyến xe trên ứng dụng. FAQ lưu ý dữ liệu Hà Nội phụ thuộc kết nối với các đơn vị vận hành. | Thử thông tin giờ đến sẵn có trên các tuyến trước; giờ xe đến không tự cho biết xe đông hay vắng. |
| Google Maps — dự báo độ đông | [Dự báo từ đóng góp hành khách](https://support.google.com/transitpartners/answer/9551309?hl=en); [Nguồn dữ liệu độ đông](https://support.google.com/transitpartners/answer/10106342?hl=en) | Hỗ trợ hành khách cân nhắc độ đông khi tra cứu chuyến đi, tùy nơi có dữ liệu. | Google mô tả dự báo từ phản hồi của người dùng; dữ liệu độ đông cũng có thể đến từ đơn vị vận tải hoặc dự báo nội bộ. | Dự báo không mặc nhiên là số đo thời gian thực; chưa kiểm tra các tuyến và khung giờ nào có hiển thị độ đông. | Kiểm tra mức độ bao phủ các tuyến trên công cụ có sẵn và đối chiếu với quan sát thực tế trước khi đề xuất xây mới. |
| Transit — thông tin độ đông chuyến sắp đến | [Hướng dẫn theo dõi chuyến](https://help.transitapp.com/article/445-how-to-track-departures-on-your-transit-line) | Hiển thị thời gian đến và mức đông của chuyến sắp đến tại khu vực được hỗ trợ. | Theo tài liệu Transit, dữ liệu độ đông có thể đến từ cảm biến của đơn vị vận tải hoặc phản hồi người đi xe. | Phụ thuộc khu vực và nguồn dữ liệu; chưa xác minh mức độ bao phủ các tuyến hoặc độ chính xác tại các điểm đón. | Tham khảo cách kết hợp nguồn dữ liệu và phản hồi hành khách; cần xác minh khả năng tiếp cận dữ liệu từ các tuyến và đơn vị vận hành. |

**Kết luận research:** Đã có công cụ hỗ trợ một phần việc xem giờ đến hoặc mức đông tại nơi có dữ liệu. Với mục tiêu hỗ trợ hành khách trên tất cả các tuyến xe buýt, nhóm cần kiểm tra mức độ bao phủ tuyến, nguồn dữ liệu độ đông và độ chính xác theo tuyến, khung giờ trước khi kết luận nên dùng công cụ sẵn có hay phát triển thêm.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

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
