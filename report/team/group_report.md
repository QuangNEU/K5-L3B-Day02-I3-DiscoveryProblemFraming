# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: I3
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

### Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tóm tắt & Rút trích thông tin | Tóm tắt tài liệu môn học (#4), Tóm tắt kiến thức từ Podcast (#6), Tóm tắt nội dung họp (#7) | Cần xử lý một lượng thông tin dài (text/audio), rút ra các ý chính và action items để tiết kiệm thời gian đọc/nghe. |
| B — Đưa ra quyết định & So sánh | Khó chọn chuyến buýt E03 (#1), Khó so sánh chi phí 2 phòng trọ (#2), Tìm căn hộ theo tiêu chí (#9) | Cần đối chiếu nhiều biến số (độ đông đúc, thời gian, chi phí, tiện ích) để đưa ra lựa chọn hoặc đề xuất tối ưu nhất. |
| C — Đối chiếu & Phân loại dữ liệu | Thủ quỹ đối chiếu chuyển khoản (#3), Gom log realtime tra cứu bug (#5), Phân loại ticket CSKH (#8) | Xử lý dữ liệu nhiễu hoặc rời rạc (tên viết tắt, log rác, yêu cầu khách hàng) để khớp đúng người, đúng chỗ hoặc gom về một nơi. |

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
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **1. Khó chọn chuyến xe buýt E03 theo độ đông** | 5 | 5 | 5 | 5 | 4 | 5 | 5 | **34** |
| **2. Khó so sánh chi phí của 2 phòng trọ**  | 3 | 5 | 4 | 2 | 5 | 4 | 5 | **28** |
| **3. Thủ quỹ đối chiếu chuyển khoản thiếu tên**  | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| **4. Tóm tắt tài liệu môn học / requirement**  | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| **5. Gom log realtime tra cứu bug**  | 5 | 4 | 4 | 4 | 3 | 4 | 4 | **28** |
| **6. Tóm tắt kiến thức từ Podcast**  | 3 | 4 | 3 | 3 | 4 | 4 | 5 | **26** |
| **7. Tóm tắt Nội dung họp**  | 5 | 3 | 5 | 4 | 4 | 4 | 5 | **30** |
| **8. CSKH: Phân loại và chuyển đúng bộ phận**  | 3 | 3 | 4 | 4 | 3 | 4 | 3 | **24** |
| **9. Tìm căn hộ theo tiêu chí khách hàng**  | 4 | 3 | 3 | 3 | 3 | 4 | 3 | **23** |

---

**Candidate được chọn:**
**#1. Khó chọn chuyến xe buýt E03 theo mức độ đông** (của Minh).

**Vì sao chọn:**
- **Nỗi đau thật, tần suất cao:** Hầu hết sinh viên trong nhóm đều gặp cảnh chờ 20 phút rồi phải chen chúc trên tuyến E03 khung 7h-8h sáng. Impact (thời gian chờ, sự mệt mỏi) là rất rõ ràng và dễ phỏng vấn user.
- **Có đất để so sánh các mức AI:** Bài toán này rất tuyệt vời để so sánh: No AI (nhìn app GPS thường), Rule (đặt ngưỡng Fix: >40 người là đông), và AI/ML (Mô hình dự đoán độ đông theo thời gian, trạm, thời tiết).
- **Rủi ro dữ liệu đã có lời giải:** Nhóm chọn phương án dùng *Dữ liệu giả lập (Mock Data)* dựa trên quan sát thực tế và đóng vai là team Product nội bộ của hãng xe buýt. Điều này biến ý tưởng từ "bất khả thi" thành một bài toán Data/ML cực kỳ vừa sức cho thời gian làm lab.

**Vì sao loại các candidate còn lại:**
- Bài *Tóm tắt tài liệu (#4)* và *Thủ quỹ (#3)* có số điểm tương đương (34 điểm). Tuy nhiên, bài "Thủ quỹ" có tần suất diễn ra ít (1-2 lần/kỳ), còn bài "Tóm tắt tài liệu" lại hơi cá nhân. Nhóm muốn chọn bài toán Xe buýt (#1) vì nó mang tính cộng đồng cao, có chứa thách thức về mặt Xử lý Dữ liệu (Data Pipeline) và Machine Learning dự đoán - cực kỳ phù hợp với một đồ án ứng dụng AI.

**Xử lý bất đồng (nếu có):**
Ban đầu nhóm e ngại bài E03 bị thiếu API dữ liệu số lượng khách thật (Feasibility rủi ro cao). Tuy nhiên, sau khi thống nhất hướng pivot: sử dụng thuật toán ML để dự đoán dựa trên dữ liệu quét thẻ giả lập (Mock Data tap-in), cả nhóm đều đồng ý đây là bài toán hay nhất, đủ chiều sâu để trình bày.

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

# 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ thấp, Độ phức tạp trung bình – cao**.

**Vì sao:**
- Độ mơ hồ thấp: Dầu vào (data tap-in, timestamp, trạm) rất rõ ràng, đầu ra cần một con số/phân loại cụ thể (Xanh/Vàng/Đỏ).
- Độ phức tạp trung bình – cao: Có quy luật nhưng đan xen nhiều biến số (người lên thì quẹt thẻ, người xuống không quẹt thẻ, phụ thuộc thời tiết, điểm kẹt xe, trạm trường học...). Không thể tính bằng công thức toán cộng trừ đơn giản.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Chỉ hiển thị vị trí GPS của xe trên app (như hiện tại). | Người dùng chỉ cần biết xe sắp tới chưa để chạy ra bến. | Không giải quyết được nỗi đau "lên xe bị nhồi nhét". | Không |
| **Rule** | Số người = Tổng số lượt tap-in trong chuyến. Đặt rule: >40 lượt là Đỏ (Đông). | Khi mọi người đều tap-out lúc xuống xe (ở VN gần như không có). | Số người chỉ tăng lên chứ không giảm xuống, xe đã trống nhưng app vẫn báo Đỏ. | Không |
| **Workflow (có ML)** | Rule gom log tap-in → ML dự đoán số người xuống để nội suy số người trên xe → Hiện cảnh báo màu trên app → Sinh viên tự quyết định. | Khi cần cân bằng giữa chi phí hệ thống và tính thực tiễn của dữ liệu (không cần camera). | Mô hình ML đoán sai lượng người xuống ở các trạm lớn. | **Chọn** |
| **Agent** | AI phân tích độ đông, tự động điều phối thêm xe buýt dự phòng từ trạm điều hành, hoặc tự book Grab cho khách. | Cần tự động hóa toàn bộ hệ thống giao thông công cộng. | Quá xa vời, chi phí khổng lồ, ngoài tầm kiểm soát của PM/User. | Không |

**Mức chọn:** Workflow (kết hợp Machine Learning / Predictive AI).

**Vì sao không chọn mức đơn giản hơn:** Mức Rule không thể giải bài toán khách xuống xe không quẹt thẻ. Bắt buộc phải có thuật toán Machine Learning học dữ liệu lịch sử để "nội suy" (ước lượng) lượng người xuống tại các trạm trọng điểm (VD: trạm Bách Kinh Xây).


### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Ước lượng số khách đang có trên xe và gán nhãn độ đông: Thoải mái (Xanh), Kín chỗ (Vàng), Quá tải (Đỏ). |
| **Judgment** — con người cân nhắc, quyết định gì? | Sinh viên nhìn nhãn màu, kết hợp với hoàn cảnh (có sắp muộn học không) để quyết định đi chuyến này hay đợi chuyến sau. |
| **Action** — hành động cuối cùng là gì, ai làm? | Sinh viên bước lên xe hoặc ở lại trạm (Người dùng làm). |
| **Outcome** — đo kết quả bằng gì? | Tỉ lệ sinh viên bị nhồi nhét giảm; Trải nghiệm đi xe buýt E03 thoải mái hơn. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Real-time log tap-in từ máy POS, Vị trí trạm hiện tại, Thời gian, Thứ trong tuần. (Giả định: Có sẵn từ Data Warehouse của VinBus). |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Nút report nhanh trên app: "Thực tế xe có đông không?" để người dùng feedback (Crowdsourcing phụ trợ). |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? 
  * Bằng chứng: Augment (Hỗ trợ). Sinh viên vẫn muốn tự ra quyết định. Nếu họ sắp thi cuối kỳ thì xe "Đỏ" cỡ nào họ cũng phải đu lên, AI không được quyền cấm họ lên xe hay tự ý hủy chuyến của họ.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
  * **Báo sót (App báo Xanh/Vắng, nhưng xe Đỏ/Đông) là tệ nhất.** Nếu báo vắng, sinh viên đợi chuyến sau, nhưng lên xe lại bị nhồi nhét, họ sẽ cảm thấy bị lừa và xóa app ngay.
  * Thiết kế xử lý: Mô hình ML sẽ được tinh chỉnh thiên về "An toàn" (tăng độ nhạy với dự đoán số người ở lại trên xe). Thà báo Vàng hơi lố một chút, còn hơn báo Xanh sai sự thật.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên NEU đi xe buýt E03 trong khung giờ cao điểm (7h - 8h sáng). |
| **Quy trình** | Mở app → Xem vị trí xe → (Mới) Xem độ đông đúc → Quyết định ra bến/lên xe/đợi chuyến sau. |
| **Bottleneck** | Quyết định mù mờ vì chỉ thấy vị trí GPS, dẫn đến việc thường xuyên bị kẹt trên những chuyến xe quá tải (mất 20 phút chịu đựng). |
| **Impact** | Trải nghiệm mệt mỏi, stress trước giờ học; không phân bổ được thời gian chờ hợp lý. |
| **Success Metric** (baseline → target, cách đo) | (1) Độ chính xác của phân loại độ đông đạt >80% so với thực tế (đo bằng log đối chiếu). (2) User đánh giá tính hữu ích >4/5 sao qua in-app survey. |
| **Boundary** | AI chỉ gợi ý mức độ đông đúc (Xanh/Vàng/Đỏ), không ép buộc hành vi người dùng, không can thiệp lộ trình xe. |
| **AI intervention point** | Tại màn hình hiển thị thông tin chuyến xe E03 đang đến gần trạm. |
| **Mức chọn** | Workflow (tích hợp ML Prediction). |
| **Rủi ro & người kiểm tra** | Model nội suy sai lượng người xuống dẫn đến sai lệch tích lũy. → Kỹ sư/PM kiểm tra lại model định kỳ bằng đối chiếu camera quay lén hoặc chốt kiểm tra thực tế. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Quy trình | Chỉ xem GPS rồi ra bến | Xem GPS + Độ đông rồi mới ra quyết định | Cập nhật bước can thiệp của AI vào hành trình người dùng. |
| Success Metric | Giảm thời gian chờ xe | Độ chính xác thuật toán >80% | Phản biện: Mục tiêu không phải là "chờ ít đi" (chờ chuyến vắng có khi lâu hơn), mà là "chủ động được quyết định dựa trên thông tin đúng". |

**Tiêu chí đánh giá đầu ra của AI (3 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Tính logic của con số | Số lượng người ước tính trên xe luôn ≥ 0 và ≤ 80 (sức chứa max của xe buýt). | Thuật toán trừ sai dẫn đến số người trên xe bị âm (-5). |
| 2 | Độ trễ hiển thị (Latency) | App cập nhật trạng thái màu trong dưới 3 giây kể từ khi xe rời trạm trước. | App load quá lâu (quay vòng vòng) do ML tính toán chậm. |
| 3 | Mức độ an toàn của dự đoán | Hạn chế tối đa False Negative (Thực tế đông mà báo vắng). | Tỉ lệ báo Xanh nhưng thực tế xe Đỏ vượt quá 10%. |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Thấp (An toàn) | 100% sinh viên đi xe buýt đều sợ cảnh chen chúc, thông tin độ đông là tính năng họ khao khát nhất. |
| **Usability** | Người dùng có dùng được, có hiểu được đầu ra không? | Thấp (An toàn) | Giao diện hiển thị theo thang màu giao thông (Xanh/Vàng/Đỏ) hoặc icon hình người, ai cũng hiểu. |
| **Feasibility** | Có đủ dữ liệu, công cụ để làm không? | Trung bình | Có thể dùng Mock Data (dữ liệu giả lập) để train model trong phạm vi lab. Cần kiến thức cơ bản về Machine Learning Regression. |
| **Viability** | Có hợp chi phí, pháp lý không? Ai vận hành? | Trung bình | Trong thực tế, cần được VinBus/Tramoc mở API log POS. Chi phí huấn luyện model rẻ vì dữ liệu tabular (dạng bảng), không tốn GPU như LLM. |

### 8.2. Kết luận

**Quyết định:** Go (Phạm vi nhỏ / Pilot)

**Lý do:** Không có rủi ro nào ở mức CAO (Nguy hiểm). Bài toán có Value rất lớn, giải quyết được pain point có thật. Vấn đề Feasibility có thể xử lý bằng cách giới hạn phạm vi làm Pilot trên một tập dữ liệu giả lập.

**Nếu Go — pilot nhỏ nhất:**
- Tập trung DUY NHẤT vào tuyến E03, chỉ trong khung giờ 7h-9h sáng.
- Xây dựng tập Mock Data gồm 5000 dòng log tap-in giả lập.
- Train một model RandomForest/XGBoost đơn giản để test độ chính xác trước khi tích hợp vào UI.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):
Nếu test trên Mock Data mà model liên tục dự đoán ra số âm hoặc sai lệch tích lũy quá 30% (so với thực tế quan sát) → Dừng pilot AI, quay về hướng dùng Rule cứng (chỉ đếm số tap-in và cảnh báo nếu vượt ngưỡng).

---

## 9. Hạn chế và hướng tiếp theo

- **Hạn chế:** Tập Mock Data do nhóm tạo ra có thể chưa phản ánh hết những biến động bất thường (như mưa lớn đột xuất, tắc đường sự cố).
- **Hướng tiếp theo:** 
  1. Tổ chức một chiến dịch thu thập Data thật trong 3 ngày (nhóm cử người đứng tại trạm Bách Kinh Xây ghi nhận lượng người lên/xuống) để đối chiếu với model.
  2. Bổ sung tính năng "Crowdsourcing": Cho phép sinh viên bấm nút báo cáo "Đông quá" ngay trên app để model ML tự động cập nhật lại trọng số.

## 10. Tài liệu tham khảo

- Google Maps Help - Hướng dẫn tính năng Độ đông đúc phương tiện công cộng (Transit Crowding).
- [Alighting Estimation for Smart Card Data] Các bài báo nghiên cứu về việc dùng Machine Learning nội suy số người xuống xe từ dữ liệu Tap-in.
